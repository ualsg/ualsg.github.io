---
title: Roofpedia
summary: Mapping Roofscapes with AI
authors: [abraham, filip]
profile: true  # Show author profile?
date: 2021-03-27T19:30:16+08:00
lastmod: 2021-03-27T19:30:16+08:00

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true
---

{{< roofpedia >}}

## Roofpedia -- Mapping Roofscapes with AI

### Explore Sustainable Roofscapes Around the World

Roofpedia is an open registry of sustainable roofscapes around the world.
It uses deep convolutional neural network to detect sustainable roof typologies from satellite images.
Footprints of buildings identified with solar panels or rooftop greenery are tagged automatically, and the results are visualized above for a score of cities.

While most studies so far have been focused on estimating the potential of rooftops, Roofpedia enables us to understand the current and actual status of the rooftops, i.e. how many of them are currently occupied with solar panels and/or extensive greenery.
Such information advances the state of the art, complements existing studies (including those estimating the potential), and it is useful for several purposes, e.g. gauging the efficiency of government policies, tracking and monitoring pledges by businesses, verifying the use of subsidies, estimating the current carbon offsetting capacity of cities and benchmarking them (see below), and determining how much of the potential has already been realised.

The nature of our project is open --- data and code are released openly, and the project is modular, enabling the addition of new geographies and roof typologies.
Further, the paper has been published as an open access publication.

{{< figure src="featured.jpg" title="Roofpedia in a nutshell." >}}

## The Roofpedia Index

We introduce a measure of the penetration of sustainable roof typologies in major cities around the world.
Solar roofs and Green roofs mapped by Roofpedia are compared against the total number of buildings and areas of the buildings in a city. Aggregate scores are calculated for both solar and green coverage and cities are ranked with an combined score.

The results are given in the table below.
You may click on cities to visit them on map.

| **Rank** | **City**                           | **Solar Score** | **Green Score** | **Overall Score** |
| -------- | ---------------------------------- | --------------- | --------------- | ----------------- |
| 1        | [Zurich][Zurich]                   | 81              | 100             | 91                |
| 2        | [Berlin][Berlin]                   | 57              | 51              | 54                |
| 3        | [Las Vegas][Las Vegas]             | 86              | 9               | 48                |
| 4        | [Phoenix][Phoenix]                 | 75              | 13              | 44                |
| 5        | [Melbourne][Melbourne]             | 74              | 11              | 43                |
| 6        | [New York][New York]               | 42              | 28              | 35                |
| 7        | [Copenhagen][Copenhagen]           | 45              | 22              | 34                |
| 8        | [Paris][Paris]                     | 42              | 18              | 30                |
| 9        | [San Diego][San Diego]             | 24              | 14              | 19                |
| 10       | [Los Angeles][Los Angeles]         | 20              | 6               | 13                |
| 11       | [San Jose][San Jose]               | 12              | 13              | 13                |
| 12       | [Seattle][Seattle]                 | 13              | 6               | 10                |
| 13       | [Portland][Portland]               | 10              | 3               | 7                 |
| 14       | [Luxembourg City][Luxembourg City] | 7               | 4               | 6                 |
| 15       | [San Francisco][San Francisco]     | 9               | 2               | 6                 |
| 16       | [Vancouver][Vancouver] [^1]             | 0               | 0               | 0                 |
| *        | [Singapore][Singapore] [^2]            | 75              | -               | -                 |

 
[^1]: Vancouver is green! Just not roof green compared to the top cities in the list.
[^2]: Due to the lack of high quality satellite imagery for rooftop greenery, Green Score for Singapore is not calculated.

More cities are getting added to Roofpedia as their aerial or satellite imagery become available.
If you'd like to contribute images to expand Roofpedia, please [email](mailto:abrahamwu@u.nus.edu) {{% mention "abraham" %}}, the lead developer.

## Data and code

Full data and code of Roofpedia can be accessed at its [GitHub repo](https://github.com/ualsg/Roofpedia).

## Paper and attribution

A [paper](https://doi.org/10.1016/j.landurbplan.2021.104167) describing the project was published in _Landscape and Urban Planning_.

If you use Roofpedia in a scientific context, please cite the paper:

```bibtex
@article{2021_land_roofpedia,
  author = {Abraham Noah Wu and Filip Biljecki},
  doi = {10.1016/j.landurbplan.2021.104167},
  journal = {Landscape and Urban Planning},
  pages = {104167},
  title = {Roofpedia: Automatic mapping of green and solar roofs for an open roofscape registry and evaluation of urban sustainability},
  url = {https://doi.org/10.1016%2Fj.landurbplan.2021.104167},
  volume = {214},
  year = 2021
}
```


[Zurich]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.94/47.37444/8.52924

[Berlin]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.93/52.51752/13.3837

[Las Vegas]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.5/36.13763/-115.15459

[Phoenix]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.5/33.43687/-112.03097

[Melbourne]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.98/-37.81802/144.94817

[New York]:https://api.mapbox.com/styles/v1/iceofsky1/cki2tjlpr60yz19p95fcqr9h9.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q

[Copenhagen]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.93/55.68293/12.56875

[Paris]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.94/48.85579/2.34247

[San Diego]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.8/32.71559/-117.1766

[Los Angeles]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.64/34.04272/-118.19739

[San Jose]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.7/37.33137/-121.88839

[Seattle]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12/47.60711/-122.33685

[Portland]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.5/45.52039/-122.67767

[San Francisco]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12.5/37.77993/-122.42131

[Vancouver]:https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#12/49.26528/-123.11271

[Luxembourg City]:  https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#13.49/49.61314/6.12884

[Singapore]: https://api.mapbox.com/styles/v1/iceofsky1/ckkaqwtr500v317r01y46xp6r.html?fresh=true&title=view&access_token=pk.eyJ1IjoiaWNlb2Zza3kxIiwiYSI6ImNraTF4ejIxaDBxNGgycm1zd3ZvMThwOGMifQ.-QrGKalxvWk3sY7BqDbI1Q#11.35/1.3625/103.7974



## Limitations, issues, and future work

Roofpedia is an experimental research prototype, which leaves much opportunity for improvement and future work.

As with all other machine learning workflows, the results are not always 100% accurate.
Much of the performance of the predictions (e.g. classification of whether a building has a solar panel on its rooftop) depends on the quality of the input imagery.
Therefore, some buildings are misclassified, especially in imagery in which it is difficult even for humans to discern rooftop greenery and photovoltaics, resulting in false positives and false negatives.
However, when these results are aggregated at the city-scale, the results tend to be more accurate.

For future work, we hope to add more cities to our collection and add the temporal aspect to the project, tracking the evolution of greenery and solar panels through time.


## People

### Lead research and development
{{% mention "abraham" %}}

### Principal investigator
{{% mention "filip" %}}

### Research group
Urban Analytics Lab, National University of Singapore (NUS)

## Acknowledgements

Roofpedia is made possible by using the following packages:

* [PyTorch](https://pytorch.org/)
* [GeoPandas](https://geopandas.org/)
* [Robosat](https://github.com/mapbox/robosat) -- 
loading of slippy map tiles for training and mask to feature function is borrowed from robosat

This research is part of the project Large-scale 3D Geospatial Data for Urban Analytics, which is supported by the National University of Singapore under the Start-Up Grant R-295-000-171-133.

We gratefully acknowledge the sources of the used input data.
For more information, please see the aforementioned [paper](https://doi.org/10.1016/j.landurbplan.2021.104167).

Some of the aspects of the project and its name — Roofpedia — are inspired by [Treepedia](http://senseable.mit.edu/treepedia), an excellent project by the [MIT Senseable City Lab](https://senseable.mit.edu) to measure and map the amount of street greenery in cities from the pedestrian perspective, and compare cities around the world.
