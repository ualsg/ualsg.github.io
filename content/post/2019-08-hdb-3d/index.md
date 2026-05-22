---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Release of 3D building open data of HDBs in Singapore"
subtitle: ""
summary: "We have generated a dataset of all public housing buildings and we are releasing it as open data"
authors: ["filip"]
tags: ["analyses", "long reads", "3D city model", "HDB", "CityJSON", "Open data"]
categories: []
date: 2019-08-25T09:19:45+08:00
lastmod: 2019-08-25T09:19:45+08:00
featured: false
draft: false
show_related: true
pager: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []


links:
  - icon_pack: fab
    icon: github
    name: "Github (dataset)"
    url: 'https://github.com/ualsg/hdb3d-data'

  - icon_pack: fab
    icon: twitter
    name: Follow us
    url: 'https://twitter.com/urbanalyticslab'
---

![](featured.png)

Cities around the world are increasingly releasing their 3D city models as open data.
Researchers and practitioners in different disciplines are using 3D geoinformation to carry out [a variety of spatial analyses](https://doi.org/10.3390/ijgi4042842).

At NUS we have been working on generating a 3D city model of all public housing (HDB) buildings in Singapore, by conflating different open datasets.
Public housing accommodates the predominant majority of Singapore's population, so the dataset covers most of the nation's residential buildings.

We are happy to announce that we are [releasing its first version as open data](https://github.com/ualsg/hdb3d-data), hopefully benefiting researchers who previously did not have access to such data.
To the extent of our knowledge, this is the first large-scale open dataset of 3D buildings in Singapore.

We offer two formats:

* [CityJSON](https://www.cityjson.org)
* [OBJ](https://en.wikipedia.org/wiki/Wavefront_.obj_file)

Both can be downloaded on our [Github repository](https://github.com/ualsg/hdb3d-data).
While the dataset covers almost all buildings and it is semantically rich, please note that this is the first version and it is still work in progress with errors (e.g. some locations are wrongly associated due to addressing issues) and with a long todo list, please read more about the known issues at our Github [repo](https://github.com/ualsg/hdb3d-data).

The dataset can also be viewed through Mapbox:

<script src='https://api.tiles.mapbox.com/mapbox-gl-js/v1.2.1/mapbox-gl.js'></script>
<link href='https://api.tiles.mapbox.com/mapbox-gl-js/v1.2.1/mapbox-gl.css' rel='stylesheet' />
<div id='map'></div>
<script>
mapboxgl.accessToken = 'pk.eyJ1IjoiZmlsaXBiIiwiYSI6ImJtaER3cUEifQ.PsDMGtN7hWbbZRON0HveLQ';
var map = new mapboxgl.Map({
style: 'mapbox://styles/filipb/cjzqf8edw0j171ct08lpcx1hr',
center: [103.724315, 1.349543],
zoom: 15.5,
pitch: 45,
bearing: -17.6,
container: 'map',
antialias: true,
attributionControl: false
}).addControl(new mapboxgl.AttributionControl({
        customAttribution: "&copy; NUS Urban Analytics Lab &copy; HDB &copy; OneMap"}));
</script>


### Method

We have used extrusion, a straightforward and common way to generate 3D models.
It uses information about the height of each object (usually obtained from airborne laser scanning; lidar) and the geometry of the footprint.
This method results in [LoD1 (block) models](https://doi.org/10.1016/j.compenvurbsys.2016.04.005).

While this method is simple and building footprints are nowadays widely available (we have used [OpenStreetMap](https://www.openstreetmap.org)), it is hampered by the lack of open data on the heights of objects.
There is no publicly available lidar dataset covering Singapore.

Therefore, as a proxy for the height, we have used the number of storeys of each block, which is available as [open data in Singapore](https://data.gov.sg/dataset/hdb-property-information).
Although prone to errors, this method has been [very popular](https://doi.org/10.1016/j.compenvurbsys.2017.01.001) around the world and benefited a myriad of researchers.


### Data sources

We have used the following datasets:

* [2D building footprints from OpenStreetMap](https://www.openstreetmap.org)
* [HDB Property Information](https://data.gov.sg/dataset/hdb-property-information)

We linked the two using [OneMap's geocoder](https://docs.onemap.sg).
While OpenStreetMap's completeness in Singapore is high and in most cases it is sufficient to generate a 3D model, height (and/or number storeys) and the address information are not available for all buildings, and thus HDB's dataset was used along with OneMap's API to link the two.
Furthermore, HDB's dataset contains a lot of attributes for each block, not available in OpenStreetMap, greatly increasing the semantic richness of the dataset.
More information about the workflow is available at [our Github repo](https://github.com/ualsg/hdb3d-code), where we have released the code as open-source as well.


### Geometry

There is not much to say about the geometry.
It is in LoD1, and thanks to the hard work of the OpenStreetMap community, the footprints look pretty good.
Have a look yourself:

{{< figure src="hdb3d-c1_att.png" lightbox="true" >}}

{{< vimeo 355799290 >}}

### Attributes

The dataset is semantically rich thanks to coupling the two datasets ([OpenStreetMap](https://www.openstreetmap.org) and the [Housing and Development Board open data on property information](https://data.gov.sg/dataset/hdb-property-information)).

The resulting CityJSON dataset includes several attributes, such as address and number of units in each block (even decomposed by number of rooms thanks to the open data of HDB).
Check the left pane of the screenshot from [azul](https://itunes.apple.com/nl/app/azul/id1173239678?mt=12) for an example block in Bukit Merah:

{{< figure src="azul-hdb.png" title="Data viewed in azul (free macOS software for CityJSON) showing the attributes for a block in Bukit Merah." lightbox="true" >}}

For the list of attributes please scroll down to the metadata section.

Please note that the OBJ file contains only the geometry since it's a 3D computer graphics format.

### Download

If all this sounds good to you, the dataset is available on our [<i class="fab fa-github"></i> Github repo](https://github.com/ualsg/hdb3d-data).
The datasets are below 100MB in size thanks to the compactness of the CityJSON and OBJ formats.

{{< hl >}}Terms of use: if using the data, please mention the following data sources: NUS Urban Analytics Lab, HDB Singapore, OpenStreetMap contributors, and OneMap.
If you are using it for a nice publication, please cite the following [paper](https://doi.org/10.5194/isprs-annals-VI-4-W1-2020-37-2020):{{< /hl >}} 

```
@article{2020_3dgeoinfo_3d_asean,
  author = {Biljecki, F},
  doi = {10.5194/isprs-annals-vi-4-w1-2020-37-2020},
  journal = {ISPRS Annals of Photogrammetry, Remote Sensing and Spatial Information Sciences},
  pages = {37--44},
  title = {{Exploration of open data in Southeast Asia to generate 3D building models}},
  volume = {VI-4/W1-2020},
  year = {2020}
}
```

Feel free to drop us an email if you do something interesting with the dataset.


### Code

The code used to generate the data is [available as open-source](https://github.com/ualsg/hdb3d-code) as well.


### Metadata


| Key           | Value                    |
| ------------------| ------------------------------ |
| Coordinate system | SVY21 / Singapore TM ([EPSG:3414](https://epsg.io/3414)) |
| Unit | m |
| Number of buildings   | 12119   |
| [Level of Detail](https://doi.org/10.1016/j.compenvurbsys.2016.04.005)   | 1.2 |
| geographicalExtent |  [11474, 28055, 0, 45327, 48759, 142] |
| geographicLocation | Singapore, Republic of Singapore |
| Dataset version | 2019-08-25 |
| OSM input data version | 2019-07-18 |
| HDB input data version | 2019-07-05 |

As shown above, the dataset is semantically quite rich thanks to the input datasets.
The attributes from OpenStreetMap are prefixed with `osm_`, while the ones from the HDB dataset are prefixed with `hdb_`.
Please note that some information is duplicated in both datasets.
We have included both sets of information just in case.
The list of the usual attributes is as follows (but not limited to):

| Key | Description | Example |
| --- | --- | --- |
| osm_id | ID of the geometry in OpenStreetMap | `way/440545194` |
| osm_timestamp | Time of update of the 2D geometry in OSM | `2016-09-04T05:06:21` |
| osm_building | General tag for buildings | `residential` |
| osm_addr_city | [Various address information](https://wiki.openstreetmap.org/wiki/Key:addr) | `Singapore` |
| osm_residential | A general tag for additional information | `HDB` |
| ... | ... |  |
| hdb_blk_no | HDB block number | `95B` |
| hdb_street | Street name | `HENDERSON ROAD` |
| hdb_residential | Residential building (Boolean) | `Y` |
| hdb_year_completed | Year of completion | `2018` |
| hdb_bldg_contract_town | Town | `BM` |
| hdb_total_dwelling_units | Number of units | `286` | 
| hdb_4room_sold | Number of 4-room sold flats | `104` |
| ... | ... |  |
| height | Estimated height in m | `113.3` |

For the metadata sourced from the [HDB Property Information](https://data.gov.sg/dataset/hdb-property-information) you may want to check the information found in the original dataset.
For OSM metadata, there is also a [dedicated page](https://wiki.openstreetmap.org/wiki/Key:building).

The dataset includes all types of HDB buildings, incl. commercial and carparks.
There are around 12 thousand HDB buildings in Singapore:

![](hdb3d-c3_att.png)
More technical details are available on our Github repositories for [data](https://github.com/ualsg/hdb3d-data) and [code](https://github.com/ualsg/hdb3d-code).


### Further reading (updated September 2020)

A [paper](/publication/2020-3-dgeoinfo-3-d-asean/) has been published:
> Biljecki F (2020): Exploration of open data in Southeast Asia to generate 3D building models. _ISPRS Annals of Photogrammetry, Remote Sensing and Spatial Information Sciences._ VI-4/W1-2020: 37-44. [<i class="ai ai-doi-square ai"></i> 10.5194/isprs-annals-vi-4-w1-2020-37-2020](https://doi.org/10.5194/isprs-annals-vi-4-w1-2020-37-2020) [<i class="far fa-file-pdf"></i> PDF](/publication/2020-3-dgeoinfo-3-d-asean/2020-3-dgeoinfo-3-d-asean.pdf) <i class="ai ai-open-access-square ai"></i>

### Point of contact

Feel free to get in touch if you have questions or use the data for an interesting purpose.
If you find an error or have a suggestion, Github issues are a preferred mode of communication.

### NUS students

Are you an NUS student who is interested working on topics such as this one?
There are related [master thesis topics](/opportunities/student-projects) that may be of your interest.

