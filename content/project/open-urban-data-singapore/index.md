---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Guide for open urban data in Singapore"
subtitle: "Our curated inventory of data relevant for geospatial and urban analyses"
summary: "Our curated inventory of data relevant for geospatial and urban analyses"
authors: [admin, filip]
tags: [open data, singapore, guide, index, long reads]
categories: []
date: 2026-03-15T08:04:48+08:00
lastmod: 2026-03-15T10:00:00+08:00
featured: true
draft: false
show_related: true
pager: true

# Featured image
image:
  caption: "Photo by [Stephanie Yeh](https://unsplash.com/@cheez612) on [Unsplash](https://unsplash.com/photos/q2akltiB_XY)."
  focal_point: ""
  preview_only: false

projects: []
---

TL;DR: In the spirit of academia and open science, we're making our notes and observations on open data in Singapore public.

## Introduction

In our research and teaching activities that are focused on Singapore, we rely largely on open data, enabling reproducibility and fostering open science.
We created a guide on open urban datasets of relevance to help navigate all the resources.

This article may be useful to novices to get an overview of what's available in Singapore, but also to seasoned urban data scientists who may learn about datasets they might not have been aware of.
Some of the datasets listed here are used in our teaching activities, e.g. in our coursework at NUS as part of the [Master of Urban Planning](https://cde.nus.edu.sg/arch/programmes/master-of-urban-planning/) programme.

This list is by no means exhaustive, and it is also subjective, as it reflects our own research interests. 
Different research groups will have different needs and priorities, and may find some other datasets relevant too.

### Data source landscape

The data sources can be broadly grouped as follows.


- **Singapore's open data portal**: [data.gov.sg](https://data.gov.sg) is the central portal of the Singapore Government, bringing thousands of datasets released by dozens of public agencies under one roof.
It is managed by [Open Government Products](https://www.open.gov.sg), a division of [GovTech](https://www.tech.gov.sg). In Mar 2026, there has been [a nice article in The Straits Times about them](https://www.straitstimes.com/life/inside-ogp-a-little-known-tech-unit-of-the-singapore-government-where-staff-decide-what-to-build).
Most datasets mentioned here can be found on [data.gov.sg](https://data.gov.sg).
The portal was launched in early 2010s, and in the past years, it has further evolved, e.g. giving more prominence to [geospatial datasets](https://data.gov.sg/datasets?formats=GEOJSON|KML|SHP|KMZ&sort=relevancy&resultId=d_dbfabf16158d1b0e1c420627c0819168), implementing interactive viewing of data (including geospatial ones), and allowing you to be notified when datasets you use are updated or changed. New datasets are continuously added, and you can follow updates from their team on social media.
- **Open data portals of specific organisations of the Government**:
In addition, some statutory boards have their own portals.
For example, [LTA's DataMall](https://datamall.lta.gov.sg/content/datamall/en.html), [SLA's OneMap](https://www.onemap.gov.sg/apidocs/), and [SingStat](https://www.singstat.gov.sg/find-data/get-latest-data) host additional datasets or provide the same data in different, sometimes more granular formats (e.g. detailed time series, APIs).
- **OpenStreetMap**: [OpenStreetMap](https://www.openstreetmap.org/) has a high level of quality in Singapore with rapid updates. Its data quality was the subject of some research efforts in our Lab (see [here]({{< ref "/post/2020-08-osm-singapore-building-data-quality/index.md" >}}) and [here]({{< ref "/post/2020-09-3dgeoinfo-3d-asean-paper/index.md" >}})). OSM data for Singapore can be downloaded from [Geofabrik](https://download.geofabrik.de/) or queried using [Overpass Turbo](https://overpass-turbo.eu/). [Overture Maps](https://overturemaps.org) (which is linked to OSM) looks increasingly interesting too.
- **Research/academic datasets**: Data released by research groups (including ours) alongside publications, often deposited on services such as Figshare, Zenodo, or GitHub.
- **Community projects**: Independent developers who build tools and release derived data.
- **Global open datasets with Singapore coverage**: Of course, one should not forget global datasets (e.g. Copernicus) that cover the city-state as well.

## The List

### Building / housing data

{{< figure src="mike-enerio-h6gNSO2Cb0U-unsplash.jpg" title="Photo by [Mike Enerio](https://unsplash.com/@mikeenerio) on [Unsplash](https://unsplash.com/photos/bird-eye-view-photography-of-high-rise-buildings-h6gNSO2Cb0U)." lightbox="true" >}}

About footprints and attributes:

* For all building footprints your best bet is [OpenStreetMap](https://www.openstreetmap.org/), which has [nearly 100% completeness with rapid updates]({{< ref "/post/2020-08-osm-singapore-building-data-quality/index.md" >}}), though attribute data may be [limited]({{< ref "/post/2023-04-bae-openstreetmap-buildings/index.md" >}}). 
* Geometric footprints of [existing HDB buildings](https://data.gov.sg/datasets/d_16b157c52ed637edd6ba1232e026258d/view) are available on data.gov.sg.
There is also a dataset of [public Housing projects that are currently under construction](https://data.gov.sg/datasets/d_930e662ac7e141fe3fd2a6efa5216902/view), which is useful if you need to know about future buildings though at the time of writing the underlying data dates from 2018.
Conversely, [HDB closed buildings (100% vacant)](https://data.gov.sg/datasets/d_fa7159e32843947846e4d756d1aa4d7f/view) includes buildings that have been vacated, e.g. for [SERS redevelopment](https://en.wikipedia.org/wiki/Selective_En_bloc_Redevelopment_Scheme).
On that note, complete historical data on any building type (i.e. buildings that once existed but have since been demolished) is not available openly to the extent of our knowledge. Historical OSM data could be the only option.
* [HDB Property Information](https://data.gov.sg/datasets/d_17f5382f26140b1fdae0ba2ef6239d2f/view) contains descriptive information on buildings managed by HDB (with their address, number of units including granular information on their type, year of completion, number of storeys, ...), which is not available in the dataset above, so you could combine both to get a wide array of information about public housing. Like the above mentioned datasets, it also includes non-residential blocks such as multi-storey carparks. There are more than 13k buildings covered by this data, which accommodate more than 80% of residents, so it's definitely of relevance. We used this dataset as one of the input datasets to generate [3D building models]({{< ref "/post/2019-08-hdb-3d/index.md" >}}).
* Data on buildings other than HDB (landed houses, condos, commercial buildings...) is not as complete.
data.gov.sg contains another [dataset representing building footprints](https://data.gov.sg/datasets/d_e8e3249d4433845bdd8034ae44329d9e/view) as part of the URA Master Plan, but it is not complete, covering only a subset of buildings, and most of them are HDBs.

You might want to consider [OpenFACADES](/project/openfacades/), an open framework for architectural caption and attribute data enrichment via street view imagery, developed at our group.

What about 3D building data? Open 3D city models are not available.
Some notes:

* [OneMap 3D](https://www.onemap3d.gov.sg/) provides a web viewer of the nation-wide 3D city model, and while the data cannot be downloaded (and thus it isn't [open data](https://opendatahandbook.org/guide/en/what-is-open-data/)), it may be of interest.
* OpenStreetMap has [a relatively high level of completeness of building heights and floors]({{< ref "/post/2020-09-3dgeoinfo-3d-asean-paper/index.md" >}}) in comparison to other countries, so in some locations it can be used to generate 3D data through extrusion.
* Using some of the datasets mentioned earlier, some years ago, we generated and released as open data a [3D city model covering all HDB buildings]({{< ref "/post/2019-08-hdb-3d/index.md" >}}) (in CityJSON and OBJ formats). Data and code are on our [GitHub repository](https://github.com/ualsg/hdb3d-data). Note that this is an old side project, so the data is not fresh.


### Address data and geocoding

Singapore uses a relatively straightforward and well-structured [addressing system](https://en.wikipedia.org/wiki/Postal_codes_in_Singapore) based on postal codes, each of which is unique to a building (unlike many other countries where a postal code covers an area).

There is no single downloadable open dataset of all addresses and postal codes in Singapore, but address data can be retrieved through the [OneMap API](https://www.onemap.gov.sg/apidocs/), which supports geocoding (address/postal code to coordinates) and vice-versa (reverse geocoding).
The API is free and does not require registration.
There are also Python and R wrappers, such as [onemapsgapi](https://cran.r-project.org/web/packages/onemapsgapi/) for R.

Community-maintained dumps of postal code data obtained from OneMap exist on GitHub, such as [this one](https://github.com/xuancong84/singapore-address-heatmap), though these may not always be up to date.

Datasets rarely contain postal codes directly but worth to note is that the aforementioned dataset with footprints on [existing HDB buildings](https://data.gov.sg/datasets/d_16b157c52ed637edd6ba1232e026258d/view) contains their postal codes.

[Nominatim](https://nominatim.org) (OpenStreetMap's geocoder) is an alternative for geocoding. 

### Real estate transactions

{{< figure src="hongbin-A5-PwZF3CrY-unsplash.jpg" title="Photo by [Hongbin](https://unsplash.com/@hbsun2013) on [Unsplash](https://unsplash.com/photos/an-aerial-view-of-a-city-with-tall-buildings-A5-PwZF3CrY)." lightbox="true" >}}

Similarly like in the above section, most of the data available comes from HDB and it is deposited on data.gov.sg:

* [HDB Resale flat prices](https://data.gov.sg/collections/189/view) contains transactions, including the address, storey level, price, remaining lease, floor area, etc. of resale HDB flats. This dataset is regularly updated and extends back to 1990, so quite a period is covered.
* [Renting out of flats](https://data.gov.sg/datasets/d_c9f57187485a850908655db0e8cfe651/view) contains individual HDB monthly rents from January 2021 onwards, including town, block, street, and flat type. The data is indicative (owner-declared) and not verified by the statutory board.
* [Median rent by town and flat type (HDB)](https://data.gov.sg/datasets/d_23000a00c52996c55106084ed0339566/view) is an aggregated dataset but unlike the one above, it contains data since 2005.
* Commercial properties transactions (incl. rentals) is available [thanks to URA](https://eservice.ura.gov.sg/property-market-information/pmiCommercialTransactionSearch).
* URA also provides data on private residential property transactions.

Although not open data, it is worth mentioning that NUS staff and students have access to [more detailed data through URA's REALIS](https://eservice.ura.gov.sg/reis/index).


### Demographics / census

{{< figure src="john-t-OedmBcmHS9Q-unsplash.jpg" title="Photo by [John T](https://unsplash.com/@john_thng) on [Unsplash](https://unsplash.com/photos/four-person-playing-kite-on-grass-field-OedmBcmHS9Q)." lightbox="true" >}}

On [data.gov.sg](https://data.gov.sg) you will find [scores of datasets](https://data.gov.sg/datasets?topics=economy&agencies=SINGSTAT&resultId=d_b2adcabcfc9c4352f3086f1a61f77bc0) at different levels (planning area, subzones) and from different years. For example, you can find datasets on households by income and size, resident population by planning area, dwelling type, age, and ethnic group, among many others. Some of them are available in a geospatial format.

Another important venue for demographic data is [SingStat](https://www.singstat.gov.sg/find-data/explore-data-themes/population), which has [detailed time series datasets with geographic distribution](https://www.singstat.gov.sg/find-data/explore-data-themes/population/geographic-distribution/latest-news-data).
Note that many demographic datasets do not include foreigners who are not permanent residents, which represent a sizeable portion of the population.

SLA's [OneMap API](https://www.onemap.gov.sg/apidocs/) also enables retrieving various demographic data at the planning area and subzone level.

For researchers at Singapore's universities, SingStat runs the [Anonymised Microdata Access Programme (AMAP)](https://www.singstat.gov.sg/data-tools-services/anonymised-microdata-access-programme-amap), which enables them access to more detailed data.
This is not open data and access must be approved (and it is also not free), but it is worth knowing about for those who need more granular analyses than publicly available datasets allow.

### Energy consumption / sustainability

Some notable entries:

* The [Energy Market Authority (EMA)](https://www.ema.gov.sg/resources/singapore-energy-statistics) publishes electricity generation and consumption statistics. There are also some EMA datasets like [Average Monthly Household Electricity Consumption by URA Planning Area & Dwelling Type](https://data.gov.sg/datasets/d_634194a40f36e5bc11a942ab0164fa9d/view) released on data.gov.sg, but they are not up to date.
* [Solar PV Installations by URA Planning Region](https://data.gov.sg/datasets/d_cd4f91f7a1ebb2b7ceb1a70c0dbb706d/view), released by EMA. 
* [Green Mark buildings](https://data.gov.sg/datasets/d_da116ef216e3fb501846e1c9faf7e683/view) (a geospatial dataset by BCA), which can be useful for research on sustainable buildings.
* EV charging points is available through the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html).

### Transportation / mobility

{{< figure src="euan-cameron-3Es_ZsAxj_Q-unsplash.jpg" title="Photo by [Euan Cameron](https://unsplash.com/@euanacameron) on [Unsplash](https://unsplash.com/photos/3Es_ZsAxj_Q)." lightbox="true" >}}

There are dozens of datasets in this category, mostly acquired and curated by [LTA](https://www.lta.gov.sg/), available as static and dynamic datasets (API).

#### Bus stops, train stations, and routes

The location of bus stops and train stations is available at multiple locations: [OpenStreetMap](https://openstreetmap.org), [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/static-data.html), and [data.gov.sg](https://data.gov.sg) (note that there are multiple datasets related to this topic, e.g. train stations as points and polygons, and even [MRT/LRT exits](https://data.gov.sg/datasets/d_b39d3a0871985372d7e1637193335da5/view)). Rail lines are [available at data.gov.sg](https://data.gov.sg/datasets/d_222bfc84eb86c7c11994d02f8939da8d/view), and can also be extracted from OpenStreetMap.

Besides data on bus stops, the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html) contains data on bus routes, bus services, and real-time bus arrivals.

You may want to check [BusRouter SG](https://busrouter.sg) (together with its sister projects [RailRouter SG](https://railrouter.sg) and [TaxiRouter SG](https://taxirouter.sg)) for nice interactive web visualisations of this data -- all by [Chee Aun](https://github.com/cheeaun), who also maintains the underlying data in GitHub repos ([sgbusdata](https://github.com/cheeaun/sgbusdata), [busrouter-sg](https://github.com/cheeaun/busrouter-sg), etc.).
Furthermore, there is a [GitHub repo](https://github.com/yinshanyang/singapore-gtfs) with data formatted according to the [General Transit Feed Specification (GTFS)](https://en.wikipedia.org/wiki/General_Transit_Feed_Specification).

#### Parking data

Parking data is available in real-time for more than 2000 carparks in Singapore, managed by multiple agencies. There are actually two APIs: one at the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html) (returns detailed availability including coordinates) and another via [data.gov.sg](https://data.gov.sg) (enables querying historical data but without providing carpark's coordinates). You can join the carpark availability data with the [HDB Carpark Information](https://data.gov.sg/datasets?query=hdb+carpark+information) dataset to get additional attributes.

#### Origin-destination (OD) data and passenger volumes

The [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html) has APIs that enable downloading public transport (bus, train) OD data every month. For example, it contains the number of passengers that have travelled between two stations, in a granular manner by type of day (weekday/weekend) and hour. Data is available for the past three months. Historical data is not available. Do note that the entire trip is not available; it is limited to the transportation mode.

About MRT/LRT stations, worth noting that there are dynamic APIs, both via the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html), which return real-time platform crowdedness level and forecast at 30-minute intervals.

#### Travel times, speeds, and routing

* The [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html) provides estimated travel times on expressways and current traffic speeds on roads through the _Traffic Speed Bands_ API.
* Routing (distance, estimated travel time, and route geometry) between two points is available through the [OneMap API](https://www.onemap.gov.sg/apidocs/).
* OpenStreetMap-based alternatives include the [Open Source Routing Machine (OSRM)](http://project-osrm.org) and [Openrouteservice](https://openrouteservice.org). There are interfaces for Python and R, e.g. we used [osrm](https://cran.r-project.org/web/packages/osrm/index.html) in teaching.
* Although not strictly open (rather commercial with a free tier), the [Google Maps Platform](https://developers.google.com/maps/documentation) APIs remain of high quality and a lot can be done within the free monthly quota.

#### Taxi availability

{{< figure src="shawn-Y1H83J5IQog-unsplash.jpg" title="Photo by [Shawn](https://unsplash.com/@shawnanggg) on [Unsplash](https://unsplash.com/photos/black-porsche-911-on-road-during-daytime-Y1H83J5IQog)." lightbox="true" >}}

The availability of taxis is another interesting API found on the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html). The API returns the location of each taxi that is currently available (not hired/busy taxis). Check out the [TaxiRouter SG](https://taxirouter.sg), which visualises this data in real-time.

#### Traffic images

Traffic images from cameras across Singapore are available through the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/dynamic-data.html).

#### Trajectory data

[Grab-Posisi](https://engineering.grab.com/grab-posisi) is a large-scale GPS trajectory dataset by Grab, covering Singapore (and Jakarta). It contains around 84,000 trajectories with over 80 million GPS pings, collected in April 2019 at a 1-second sampling rate. It includes contextual attributes such as accuracy, bearing, speed, device type (Android/iOS), and driving mode (car/motorcycle). An extended version, [Grab-Posisi-L](https://dl.acm.org/doi/10.1145/3397536.3422218), adds ground-truth map-matching labels for benchmarking.
It is not an open dataset, but it is available by request.

#### Assorted

Both the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en.html) and [SingStat](https://www.singstat.gov.sg/find-data/search-by-theme/industry/transport/latest-data) have more datasets worth exploring, e.g. number of registered vehicles, public transport ridership trends, usual mode of transport from surveys, cycling infrastructure, and active mobility data.


### Map / Geospatial data (general)

OpenStreetMap is pretty good for most kinds of features (e.g. parks, roads, footpaths).

Well worth mentioning is also the Geospatial Whole Island dataset available through the [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en/static-data.html). It contains a variety of features related to transportation, e.g. road crossings, traffic lights, taxi stands, and cycling paths.

[data.gov.sg](https://data.gov.sg) hosts some key geospatial datasets including:

* Master Plan 2025 datasets such as [land use](https://data.gov.sg/datasets/d_a8c3546b26712e35021f3a681d0353ae/view) and [subzone boundaries](https://data.gov.sg/datasets/d_7a36470accc937bd7752ba6f829b74c1/view). These supersede the earlier Master Plan 2019 datasets (which remain available for historical comparison). Search data.gov.sg for [`"master plan 2025"`](https://data.gov.sg/datasets?query=%22master+plan+2025%22) to find the complete set.
* [The entire cadastral map of Singapore](https://data.gov.sg/datasets/d_e7395d743076a2bcc487b0d12b9bf33b/view) (by SLA).
* The [series of datasets by NParks](https://data.gov.sg/datasets?agencies=NPARKS&resultId=d_77d7ec97be83d44f61b85454f844382f) deserves being mentioned as well: they cover a wide range of park-related features, e.g. [park boundaries](https://data.gov.sg/datasets/d_77d7ec97be83d44f61b85454f844382f/view), [BBQ pits](https://data.gov.sg/datasets/d_5e5442d0766b00d2d09fd6f7768362a6/view), [park connector loop](https://data.gov.sg/datasets/d_a69ef89737379f231d2ae93fd1c5707f/view), and [carparks](https://data.gov.sg/datasets/d_d5594e4c43e838380155f05f53f58567/view) (note that NParks' carparks do not appear to be covered by LTA's API mentioned earlier).
* Keep in mind that data.gov.sg allows you to [filter](https://data.gov.sg/datasets?formats=GEOJSON|KML|SHP|KMZ&sort=relevancy&resultId=d_dbfabf16158d1b0e1c420627c0819168) all geospatial datasets.

[TreesSG](http://trees.sg) contains locations and information about nearly a million trees, but cannot be downloaded.
Check out [ExploreTrees.SG](https://exploretrees.sg), along with the underlying data in the [sgtreesdata GitHub repo](https://github.com/cheeaun/sgtreesdata), which contains data scraped from this service.

On that note, you might also want to consider computing the amount of greenery at the street level using street view imagery, i.e. the Green View Index.
Our open-source tool [ZenSVI](/project/zensvi/) can help with that -- it automates the entire pipeline from downloading SVI to computing greenery indicators and other urban metrics.

The [high-resolution map of Singapore's terrestrial ecosystems](https://doi.org/10.6084/m9.figshare.8267510), developed by the research team of [Natural Capital Singapore](https://naturalcapital.ethz.ch/home/), is released as open data (with accompanying [paper](https://doi.org/10.3390/data4030116)).

### Aerial and satellite imagery

There are no government-released high-resolution aerial imagery datasets we are aware of as open data.
The closest you can get is coarse resolution satellite imagery that are open, e.g. [Sentinel](https://s2maps.eu/).
Perhaps of relevance: [Planet's Education and Research Programme](https://www.planet.com/markets/education-and-research/) provides high-resolution daily imagery for academic use (restricted).

### Point clouds (LiDAR), terrain data

Similarly, open LiDAR data for Singapore remains unavailable.
Some terrain data options:

* [Copernicus DEM](https://dataspace.copernicus.eu/explore-data/data-collections/copernicus-contributing-missions/collections-description/COP-DEM) provides 30 m resolution global elevation data. [FABDEM](https://gee-community-catalog.org/projects/fabdem/) is a forest- and building-removed version of it.
* [SRTM](https://www.earthdata.nasa.gov/data/instruments/srtm) remains available but at coarser resolution.

### Street-level imagery

{{< figure src="airlangga-jati-ZUN8oFRqhLA-unsplash.jpg" title="Photo by [Airlangga Jati](https://unsplash.com/@airlanggajati) on [Unsplash](https://unsplash.com/photos/a-white-building-with-multicolored-windows-on-the-side-of-it-ZUN8oFRqhLA)." lightbox="true" >}}

* [KartaView](https://kartaview.org/) is a crowdsourced street-level imagery platform managed by [Grab](https://www.grab.com/), a Singapore-based company, which has also been contributing to the data. The imagery has extensive coverage and it is available openly.
* [Mapillary](https://www.mapillary.com) (owned by Meta) provides crowdsourced street-level imagery under an open licence.
* [Global Streetscapes](/project/global-streetscapes/) is our dataset of 10 million crowdsourced street-level images sampled from 688 cities worldwide (including Singapore), enriched with hundreds of attributes covering weather, quality, lighting conditions, and more. Published also as a [journal paper]({{< ref "/publication/2024-global-streetscapes/index.md" >}}).
* Nighttime street-level imagery: while SVI is almost exclusively captured during daytime, our {{% mention "zicheng" %}} has collected and released an open dataset of [nighttime panoramic SVIs across Singapore](https://github.com/zichengfan/Nighttime-SVI). This work, published in [a paper]({{< ref "/publication/2024-scs-night-svi/index.md" >}}), opens up a new paradigm for sensing urban lighting landscapes from a human perspective.
* [SPECS](/project/specs/) -- Street Perception Evaluation Considering Socioeconomics, is our recent open project that contains data on how people (including in Singapore) perceive images of streets.

Need help acquiring or analysing street view imagery? Check out [ZenSVI](/project/zensvi/), our open-source Python package for that.


### Environment / climate data

Weather data is available through [data.gov.sg](https://data.gov.sg) APIs.

Check out also [the website of Meteorological Service Singapore](https://www.weather.gov.sg/home/).

### Biodiversity and nature

{{< figure src="sergio-sala-VbB6HYunm04-unsplash.jpg" title="Photo by [Sergio Sala](https://unsplash.com/@sergiosala) on [Unsplash](https://unsplash.com/photos/aerial-view-of-trees-river-and-architectural-landmark-VbB6HYunm04)." lightbox="true" >}}

* [iNaturalist](https://www.inaturalist.org/) observations for Singapore can be queried through its API.
* The above mentioned [NParks datasets on data.gov.sg](https://data.gov.sg/datasets?agencies=National+Parks+Board) include data on heritage trees and more.
* [A high-resolution canopy height model of the Earth](https://langnico.github.io/globalcanopyheight/) at 10 m resolution might be of interest.

### Eating establishments and amenities

{{< figure src="ethan-hu-NRTptNBkLLw-unsplash.jpg" title="Photo by [Ethan Hu](https://unsplash.com/@ethanhjy) on [Unsplash](https://unsplash.com/photos/people-standing-in-front-of-store-during-daytime-NRTptNBkLLw)." lightbox="true" >}}

* [Eating establishments by NEA](https://data.gov.sg/datasets/d_1f0313499a17075d13aae6ed3e825bc6/view) -- a comprehensive geospatial dataset on all places licensed to sell food in Singapore.
* [Hawker centres](https://data.gov.sg/datasets/d_4a086da0a5553be1d89383cd90d07ecd/view) and [supermarkets](https://data.gov.sg/datasets/d_cac2c32f01960a3ad7202a99c27268a0/view) datasets on data.gov.sg.
* OpenStreetMap and Overture are options to consider.

### Airbnb / tourism

{{< figure src="ilham-wicaksono-ML2q8zCfUik-unsplash.jpg" title="Photo by [Ilham Wicaksono](https://unsplash.com/@ilhamwicaksono) on [Unsplash](https://unsplash.com/photos/people-walking-near-buildings-ML2q8zCfUik?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)." lightbox="true" >}}

* [Inside Airbnb](http://insideairbnb.com) has Airbnb data on Singapore, scraped periodically. It includes listings and their reviews. Do note that Airbnb in Singapore is allowed only [for longer stays](https://www.channelnewsasia.com/commentary/singapore-airbnb-housing-prices-illegal-rent-overtourism-4469006), so the listings are limited in comparison to some other places.
* Some of the datasets [released by the Singapore Tourism Board](https://data.gov.sg/datasets?agencies=STB&resultId=1621) may be of interest, e.g. locations of [tourist attractions](https://data.gov.sg/datasets/d_0f2f47515425404e6c9d2a040dd87354/view).

## Notes and considerations

### Social media data

The landscape of social media data has changed dramatically since the first time this guide was written in 2020.
The Twitter/X API is now not so attractive for research use.
In general, social media data for Singapore should be approached with caution given both the access restrictions and the relatively low usage of some platforms locally.
Some researchers have released global aggregated datasets like [this one](https://www.globalsentiment.mit.edu/dataset).

### Web services (view-only)

There are a few web services containing various interesting datasets (e.g. [OneMap](https://www.onemap.sg/main/v2/), [HDB Map Services](https://services2.hdb.gov.sg/web/fi10/emap.html), [URA SPACE](https://eservice.ura.gov.sg/maps/?service=GLSRELEASE&site=1018)), but not all of them can be downloaded, so they are not considered as [open data](https://opendatahandbook.org/guide/en/what-is-open-data/). Nevertheless, they may still be useful for viewing and visual exploration.

### APIs and historical data

A common limitation with some of the datasets is that they do not have historical data, or only retain a limited window.
For example, the LTA DataMall's origin-destination and passenger volume APIs only provide data for the past three months, thus, if you don't download it regularly, it's gone.
Another example is lack of data on demolished buildings and other features that do not exist anymore.

### Licence, validity and quality of data

The usual caveats:
* Check when the dataset has been updated. Some datasets are not updated in place; a new dataset is released instead as a new instance.
* Check the licence, e.g. for data.gov.sg have a look at the [Singapore Open Data Licence](https://data.gov.sg/open-data-licence). When publishing, remember to attribute the data source and mention the year when it was created/updated.
* Some geospatial datasets may not pass all validity checks (e.g. they might have self-intersecting polygons). You can try fixing them using [prepair](https://github.com/tudelft3d/prepair).

### Further reading

You might also want to check out:

* [Open Geospatial Data SG](https://nusgis.org/data/) by NUS Geography collaborator [Yingwei Yan](https://discovery.nus.edu.sg/19079-yingwei-yan), which covers similar ground.

## Our tools and datasets

We [publish](/data-code) most of our code and data openly.
A full list is available on our [data and code page](/data-code/).
Here are some resources:

* [VoxCity](/project/voxcity/) -- a Python package for open geospatial data integration, 3D city model generation, and urban environment simulation.
* [Global Streetscapes](/project/global-streetscapes/) -- 10M street-level images including Singapore, with 346 attributes.
* [ZenSVI](/project/zensvi/) -- open-source SVI acquisition, processing and analysis toolkit.
* [Urbanity](https://github.com/winstonyym/urbanity) -- a feature-rich urban network dataset covering Singapore and 50+ cities.
* [Global Building Morphology Indicators](/project/gbmi/) -- building morphology data covering SG.

## What about the rest of Southeast Asia?

While this guide is focused on Singapore, some of our research covers the wider region.
Southeast Asia presents a more varied and challenging landscape for open urban data.

A few pointers:

* OpenStreetMap remains the single most important source of open geospatial data across the region, though coverage and quality vary greatly between countries and between urban and rural areas. We explored this topic in our [paper on 3D building data in ASEAN]({{< ref "/post/2020-09-3dgeoinfo-3d-asean-paper/index.md" >}}).
* KartaView has particularly extensive street-level imagery coverage in the region -- arguably the best open source of open SVI for the region. Further, there is [an open dataset](https://kartaview.org/landing/open-imagery) released by Grab focusing on a few cities with expanded street view coverage.
* [Google Open Buildings](https://sites.research.google/open-buildings/) provides building footprint data across Southeast Asian countries.
* Our [Global Streetscapes](/project/global-streetscapes/) includes imagery from several cities across Southeast Asia.
* Individual countries have their own open data portals with varying levels of maturity -- for example, [data.go.id](https://data.go.id/) (Indonesia), [data.gov.ph](https://data.gov.ph/) (Philippines), and [data.go.th](https://data.go.th/) (Thailand).
* The Philippines is one of the rare countries with open [nation-wide open lidar data](https://lipad.dream.upd.edu.ph).

### Have a suggestion for an entry? Spotted an error?

[Get in touch](/#contact).
