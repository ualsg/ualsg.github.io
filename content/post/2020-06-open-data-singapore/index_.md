---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Guide for open urban data in Singapore"
subtitle: "Our curated inventory of data relevant for geospatial and urban analyses"
summary: "Our curated inventory of data relevant for geospatial and urban analyses"
authors: [admin, filip]
tags: [open data, singapore, guide, index, long reads]
categories: []
date: 2020-06-24T08:04:48+08:00
lastmod: 2021-11-04T08:32:48+08:00
featured: true
draft: false
show_related: true
pager: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Photo by [Stephanie Yeh](https://unsplash.com/@cheez612) on [Unsplash](https://unsplash.com/photos/q2akltiB_XY)."
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

{{% callout note %}}
TL;DR: In the spirit of academia and open science, we’re making our notes on open data in Singapore public, and intend to keep them updated.
Feel free to visit in future to check for updates as the list grows.
{{% /callout %}}

## Introduction

In our research and teaching activities that are focused on Singapore, we rely almost entirely on open data, enabling reproducibility and fostering open science.
We created a guide for open urban datasets to help navigate through all the resources.

While [Data.gov.sg](https://data.gov.sg) (the open data portal of the Singapore Government) is thorough and it is the starting and ending point to obtain many useful datasets, it might take time to get an overview and the availability of open data goes beyond that.
Furthermore, there are some particularities that may not be evident at first and which we elaborate on in the text (e.g. some datasets are available at multiple locations with slight differences).

This index may be useful to novices to get an overview of what's available in Singapore, but also to seasoned urban scientists who may learn about datasets they might not have been aware of.

The data sources can be grouped into the following categories.

- [Data.gov.sg](https://data.gov.sg) -- the Government's Open Data portal, containing almost 2000 datasets on myriads of topics from dozens of public organisations. Many datasets are regularly updated. There are some GIS datasets too, and also APIs providing real-time data.
- Government resources that are outside the realm of Data.gov.sg, e.g. there may be additional datasets not deposited in the central government repository, some that are slightly different, or those with newer updates. For example, [LTA's DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall.html) and [SingStat](https://www.singstat.gov.sg/find-data/search-by-a-z) have some additional resources, or datasets that are available on [Data.gov.sg](https://data.gov.sg) but they are arranged in various, potentially more appropriate forms (e.g. detailed time series instead of separate datasets). Such resources include several APIs as well.
- [OpenStreetMap](https://www.openstreetmap.org/) -- needless to mention for geospatial data, but surprisingly often overlooked.
OSM appears to have a very high level of quality in Singapore and rapid updates. Its data quality assessment was subject of recent research efforts conducted at our Lab (see [here]({{< ref "/post/2020-08-osm-singapore-building-data-quality/index.md" >}}) and [here]({{< ref "/post/2020-09-3dgeoinfo-3d-asean-paper/index.md" >}})).
- Data by research groups, companies, community, ...

This list is by no means a complete inventory of open datasets useful for urban analytics covering the city-state.
While there are other instances not mentioned here, these are the datasets we consider useful for our work, have used in our work, or we bookmarked them to consider using them in future.


## The List

### Building and housing data

* [HDB Property Information](https://data.gov.sg/dataset/hdb-property-information) contains data on each public housing block in Singapore (address, number of flats, year of completion, number of storeys, breakdown by flat type, ...).
It also includes non-residential blocks such as multi-storey carparks.
It does not contain building footprints though.
We used this dataset as one of the input datasets to generate [3D building models]({{< ref "/post/2019-08-hdb-3d/index.md" >}}).
* Geometric footprints of HDB buildings is available [here](https://data.gov.sg/collections/2033/view).
* Data on non-HDB buildings (landed houses, condos, commercial buildings...) is not as complete and it is scattered around, but [URA's data portal](https://www.ura.gov.sg/realEstateIIWeb/supply/search.action) is a good starting point for exploration.
* For open data on all building footprints the best bet is OpenStreetMap, it has [nearly 100% completeness with rapid updates]({{< ref "/post/2020-08-osm-singapore-building-data-quality/index.md" >}}), but attribute data may lack.
Data.gov.sg contains [a dataset representing building footprints](https://data.gov.sg/dataset/master-plan-2014-building), but for some reason it is not complete, covering only a subset of buildings several years ago.
It still might be useful though.
* Check out [Roofpedia](/project/roofpedia/), our project that maps solar panels and green roofs on buildings, which includes open data on Singapore, together with several other cities.
* You may also be interested in our project [Global Building Morphology Indicators](/project/gbmi/), which covers SG.

{{< figure src="danist-FXeaLbv2DQU-unsplash.jpg" title="Photo by [贝莉儿 DANIST](https://unsplash.com/@danist07) on [Unsplash](https://unsplash.com/photos/FXeaLbv2DQU)." lightbox="true" >}}


### 3D city models

Unfortunately, 3D city models are not released as open data, except the one [we generated covering only HDBs]({{< ref "/post/2019-08-hdb-3d/index.md" >}}).
The recently [released OneMap3D](https://www.sla.gov.sg/articles/press-releases/2020/launch-of-onemap3d-beta-at-singapore-geospatial-week-2020) provides a [web viewer of the nation-wide 3D city model](https://www.onemap3d.gov.sg/), but the data cannot be downloaded, thus, it does not qualify as [open data](https://opendatahandbook.org/guide/en/what-is-open-data/).

Worth mentioning is that OpenStreetMap has [a relatively high level of completeness of building heights and floors]({{< ref "/post/2020-09-3dgeoinfo-3d-asean-paper/index.md" >}}), in comparison to other countries, so in some locations it can be used to generate 3D data.

### Real estate transactions

* There is [a dataset](https://data.gov.sg/dataset/resale-flat-prices) on resale HDB flats transactions, including the address, storey level, price, remaining lease, etc.
* [Median rent by town and flat type (HDB)](https://data.gov.sg/dataset/median-rent-by-town-and-flat-type), available by quarter since 2005.
* [Data on vacancies](https://www.singstat.gov.sg/find-data/search-by-theme/industry/building-real-estate-construction-and-housing/latest-data) at the SingStat's portal.
* Private residential properties transactions (incl. rentals) are [available through URA](https://www.ura.gov.sg/realEstateIIWeb/transaction/search.action).
The same agency also releases [data on commercial properties](https://www.ura.gov.sg/Corporate/Property/Property-Data/Commercial-Properties).

Although not open data, it is worth mentioning that NUS staff and students have access to [more detailed data](https://www.ura.gov.sg/realis) through a subscription.

### Demographics

If you need demographic data, you will probably head to Data.gov.sg, where you will find [scores of datasets](https://data.gov.sg/search?groups=society) at different levels (planning area, subzones) and from different years, so it might take time to navigate their landscape.
For example, you may find:
* [Households by Monthly Household Income and Household Size](https://data.gov.sg/dataset/households-by-monthly-household-income-and-household-size)
* [Resident Working Persons Aged 15 Years and Over by Planning Area and Gross Monthly Income from Work, 2015](https://data.gov.sg/dataset/resident-working-persons-aged-15-years-over-by-planning-area-gross-monthly-income-from-work-2015?resource_id=e4c209d3-4a07-426a-baeb-a7026d09241c)
* [Resident Population by Planning Area/Subzone and Type of Dwelling, 2015](https://data.gov.sg/dataset/resident-population-by-planning-area-subzone-and-type-of-dwelling-2015)
* [Resident Population by Single Year of Age, Ethnic Group and Sex, 2015](https://data.gov.sg/dataset/resident-population-by-single-year-of-age-ethnic-group-and-sex-2015)
* [Singapore Residents by Subzone and Type of Dwelling, Jun 2017](https://data.gov.sg/dataset/singapore-residents-by-subzone-and-type-of-dwelling-jun-2017)

Some of them, like the last example, are available in a geospatial format.

However, the best place to get demographic data may be through [SingStat](https://www.singstat.gov.sg/find-data/search-by-theme/population/geographic-distribution/latest-data), which lists them for a clear overview and has detailed time series datasets, so you don't have to join multiple datasets.

Worth mentioning here is also the SLA's [OneMap API](https://docs.onemap.sg) that enables retrieving various demographic data on the planning area level.

Note that most demographic datasets do not include foreigners who are not permanent residents, which represent a sizeable portion of the population.


### Energy consumption

To the extent of our knowledge, the most granular dataset available is the Data.gov.sg dataset [Average Monthly Household Electricity Consumption by URA Planning Area & Dwelling Type](https://data.gov.sg/dataset/average-monthly-household-electricity-consumption-by-ura-planning-area-and-dwelling-type-2013).


### Transportation and mobility

There are dozens of datasets in this category, mostly acquired and curated by [LTA](https://www.lta.gov.sg/).

#### Bus stops, train stations, and routes

The location of bus stops and train stations is available at multiple locations: [OpenStreetMap](https://openstreetmap.org), [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/static-data.html), and [Data.gov.sg](https://data.gov.sg) (note that there are multiple datasets related to this topic, e.g. train stations as [points](https://data.gov.sg/dataset/sdcp-mrt-station-point) and [polygons](https://data.gov.sg/dataset/master-plan-2014-rail-station), there is even one on [MRT/LRT exits](https://data.gov.sg/dataset/lta-mrt-station-exit)).
Furthermore, rail lines are available at [Data.gov.sg](https://data.gov.sg/dataset/master-plan-2014-rail-line), but they can also be extracted from [OpenStreetMap](https://openstreetmap.org).

Besides data on bus stops, the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) contains data on bus routes, bus services, and real-time bus arrivals. 
You may want to check [BusRouter SG](https://busrouter.sg) (together with its sister project [RailRouter SG](https://railrouter.sg)) for an awesome web visualisation of this data.
Furthermore, there is a [Github repo](https://github.com/yinshanyang/singapore-gtfs) with the data stored according to the [General Transit Feed Specification](https://en.wikipedia.org/wiki/General_Transit_Feed_Specification).


#### Parking data

Parking data is available in real-time for more than 2000 carparks in Singapore, managed by multiple agencies.
One particularity that may go unnoticed is that there are actually two APIs.
One is offered at the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) -- it returns detailed availability by carpark, and some information about each such as coordinates.
The second one, linked on the Developer section at [Data.gov.sg](https://data.gov.sg/developer) is similar, but it enables querying historical data forgoing some information about the carparks such as location.
We used this dataset in our [analysis on mobility during the circuit breaker]({{< ref "/post/2020-04-covid-19-singapore-impact-urban-data/index.md" >}}).

You can join the carpark availability data with the dataset [HDB Carpark Information](https://data.gov.sg/dataset/hdb-carpark-information) to get a few more columns not returned by the APIs.
Note that the location of carparks is simply represented as a point, while the [HDB Map Services](https://services2.hdb.gov.sg/web/fi10/emap.html) shows them as shapes.
However, the latter is not available for download.


#### Origin and destination data, and passenger volume by station/stop

The [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) has a few APIs that enable downloading public transport (bus, train) traffic every month. 
For example, it contains the number of passengers that have travelled between two stations, with a breakdown by type of day (weekday/weekend) and hour.
Data is available for the past three months.
Do note that the entire trip is not available; it's limited to the transportation mode.
For example, if a traveller takes a bus to an MRT station and continues the journey with a train, these are considered as separate trips and cannot be connected in the data.

Regarding MRT/LRT stations, there are two dynamic APIs, both available via the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html).
One returns real-time platform crowdedness level for the MRT/LRT stations of a particular train network line, while the other 
provides a forecast for the same at 30 minutes intervals.

{{< figure src="euan-cameron-3Es_ZsAxj_Q-unsplash.jpg" title="Photo by [Euan Cameron](https://unsplash.com/@euanacameron) on [Unsplash](https://unsplash.com/photos/3Es_ZsAxj_Q)." lightbox="true" >}}


#### Current travel times and speeds

Another API available thanks to the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) returns the estimated travel times of expressways.
It might be useful for studying the volume of traffic.
It doesn't look that it enables querying historical data, though.

A related API, _Traffic Speed Bands_, also on the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html), returns current traffic speeds on roads.

#### Routing

Routing (fetching the distance, estimated travel time, and the geometry of the route) between two points is available through the [OneMap API](https://docs.onemap.sg).
OpenStreetMap is also useful here, e.g. check out the [Open Source Routing Machine](http://project-osrm.org) and [Openrouteservice](https://openrouteservice.org).
There are interfaces for Python and R, e.g. we used [osrm](https://cran.r-project.org/web/packages/osrm/index.html) in teaching.

Although not strictly open, rather commercial (but they offer a free tier), here it is inescapable to mention the trio of APIs under the [Google Maps Platform](https://developers.google.com/maps/documentation): Directions API, Distance Matrix API, and Roads API, which are of high quality and a lot can be done within the free monthly quota they offer.


#### Taxi availability

The availability of taxis is also available on the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html).
The API returns the location of each taxi that is currently available.
The data does not include hired/busy taxis.
Check out the [TaxiRouter SG](https://taxirouter.sg), which visualises this data in real-time, together with the [taxi stands](https://data.gov.sg/dataset/lta-taxi-stop).


#### Traffic images

Traffic images are available through the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html).

#### Transportation mode

[Data.gov.sg](https://data.gov.sg/search?q=mode+of+transport) contains several datasets on the usual mode of transport used by residents according to surveys.

#### Mobility trends

[Apple Mobility Trends Reports](https://www.apple.com/covid19/mobility), [Google Community Mobility Reports](https://www.google.com/covid19/mobility/), and [CityMapper Mobility Index](https://citymapper.com/cmi) all include Singapore.

[CITYDATA](https://citydata.ai) has released [Singapore mobility trip patterns as open data](https://univercity.ai/mobility-trip-patterns-for-singapore/). 

#### Assorted

Both the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html) and [SingStat](https://www.singstat.gov.sg/find-data/search-by-theme/industry/transport/latest-data) have more datasets worth having a look at, e.g. number of cars in SG at a fine temporal scale (updated monthly).


### Map / Geospatial data (general)

Besides OpenStreetMap which is [quite complete and of high quality for a wide range of features]({{< ref "/post/2020-08-osm-singapore-building-data-quality/index.md" >}}), well worth mentioning is the Geospatial Whole Island dataset available through the [LTA DataMall](https://www.mytransport.sg/content/mytransport/home/dataMall/dynamic-data.html).
It contains a bunch of different features related to transportation, e.g. road crossings, traffic lights, taxi stands, and cycling paths.

Further, [Data.gov.sg](https://data.gov.sg) contains some datasets such as the [boundaries of administrative areas](https://data.gov.sg/dataset/master-plan-2019-subzone-boundary-no-sea), [master plan land use](https://data.gov.sg/dataset/master-plan-2019-land-use-layer) (containing the [Gross Plot Ratio](https://www.ura.gov.sg/Corporate/Guidelines/Development-Control/Non-Residential/Commercial/Gross-Plot-Ratio)), and [cadastral land parcels](https://data.gov.sg/dataset/sla-cadastral-land-parcel).
The [series of datasets by NParks](https://data.gov.sg/dataset?q=&organization=national-parks-board) hosted on Data.gov.sg deserves special attention: it covers a wide range of [park](https://data.gov.sg/dataset/parks)-related features under their purview, e.g. [boundaries of activity areas](https://data.gov.sg/dataset/nparks-activity-area), [locations of play/fitness equipment](https://data.gov.sg/dataset/nparks-playfitness-equipment), [bbq pits](https://data.gov.sg/dataset/nparks-bbq-pits), [the shape of the park connector loop](https://data.gov.sg/dataset/park-connector-loop), and [carpark lots](https://data.gov.sg/dataset/nparks-car-park-lots) (however, do note that the NParks' carparks do not appear to be covered by the LTA's API mentioned above).

For trees, check out [ExploreTrees.SG](https://github.com/cheeaun/exploretrees-sg), derived from [Trees.SG](http://trees.sg).

Finally, you may be interested in the [high-resolution map of Singapore’s terrestrial ecosystems](https://doi.org/10.6084/m9.figshare.8267510) that was developed by the research team of the [Natural Capital Singapore](http://www.naturalcapital.sg) and released as open data.
There is also a [paper](https://doi.org/10.3390/data4030116) published.


### Aerial imagery

There are no open data high-resolution resources we are aware of.
Satellite imagery is available for academia through the [Planet's Education and Research Programme](https://www.planet.com/markets/education-and-research/), which we are a member of and which is accessible to other academics as well. 

### Point clouds (LiDAR), terrain data

Pretty much none, except terrain data of coarse resolution such as [SRTM](https://www2.jpl.nasa.gov/srtm/).
Please see also [this page](https://ugl.sg/2022/10/03/dem-of-singapore-srtm/) from the [NUS Urban Green Lab](https://ugl.sg).

### Street-level imagery

Google Street View has pretty good coverage of Singapore (it even includes [hawker centres](https://www.channelnewsasia.com/news/singapore/google-hawker-centres-stalls-street-view-maps-trekkers-11764968)), and the data is downloadable through their [API](https://developers.google.com/maps/documentation/streetview/intro) (check the T&C though).
[Mapillary](https://www.mapillary.com) and [KartaView](https://kartaview.org/) are also worth considering.



### Airbnb

[Inside Airbnb](http://insideairbnb.com) has Airbnb data on Singapore, updated monthly.
It includes listings and their reviews.


### Other

There are some datasets, which albeit we have not used much so far, are worth mentioning and keeping in mind.
The honourable mentions are:

* Weather data, which is available through [Data.gov.sg](https://data.gov.sg/developer): real-time weather readings, Pollutant Standards Index (PSI), Ultra-violet Index (UVI), etc.
* [Eating establishments by NEA](https://data.gov.sg/dataset/eating-establishments) -- quite comprehensive dataset on all places allowed to sell food in Singapore.
You may also be interested in [data on hawker centres](https://data.gov.sg/dataset/hawker-centres) and [supermarkets](https://data.gov.sg/dataset/supermarkets).
* [Skyrise Greenery dataset](https://data.gov.sg/dataset/nparks-skyrise-greenery) shows the indicative location of rooftop and vertical greenery.



## Notes and considerations

### Tabular data / geocoding

While much of the data represents _something that happens somewhere_ (e.g. real estate transactions), many datasets are not available in a GIS format.
They are rather released as [CSVs](https://en.wikipedia.org/wiki/Comma-separated_values) (e.g. real estate transaction datasets contain an address representing each transaction, but not the coordinates nor the dataset is in a geo-format).
To convert (geocode) the address into coordinates, may we suggest to use the [OneMap API](https://docs.onemap.sg), [Nominatim](https://nominatim.org), or [Google Maps API](https://cloud.google.com/maps-platform/).

### Web services

There are a few web services containing various interesting datasets (e.g. [OneMap](https://www.onemap.sg/main/v2/), [OneMap3D](https://www.onemap3d.gov.sg/), [HDB Map Services](https://services2.hdb.gov.sg/web/fi10/emap.html), [URA SPACE](https://www.ura.gov.sg/maps/), [Trees.sg](http://trees.sg)), but not all of them can be downloaded, so they are not considered as [open data](https://opendatahandbook.org/guide/en/what-is-open-data/).
Nevertheless, they may still be useful for viewing.

### Social media

The [Twitter API](https://developer.twitter.com/en/docs) enables downloading their data for Singapore, but given that the social network is not very popular here, and the data comes with restrictions (so it is technically not open data), its functionality is not that great.

### Licence, validity and quality of data

The usual caveats:
* Check when the dataset has been updated. Some datasets are not updated, a new dataset is released instead as a new instance, not superseding the old one. 
* Check the licence, e.g. for Data.gov.sg have a look at the [Singapore Open Data Licence](https://data.gov.sg/open-data-licence).
* Do not forget to attribute the data source in your use and mention the year when it was created/updated.
* Some geospatial datasets may not pass all validity checks (e.g. they might have self-intersecting polygons), presenting a problem when they are used in spatial analyses.
You can try fixing them using [prepair](https://github.com/tudelft3d/prepair).

### Further reading

You might also want to check out [this page](https://nusgis.org/data/) by NUS Geography collaborator [Yingwei Yan](https://discovery.nus.edu.sg/19079-yingwei-yan). 

### Have a suggestion for an entry? Spotted an error?

[Get in touch](/#contact).






