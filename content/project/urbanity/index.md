---
title: Urbanity
summary: A network-based Python package and an open global dataset of feature-rich urban networks for understanding and modelling urban complexity.
authors: [winston]
profile: true  # Show author profile?
date: 2026-10-30T10:30:16+08:00
lastmod: 2026-10-30T10:30:16+08:00

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false
---

# A network-based Python package and open dataset for feature-rich urban network analytics

Urbanity, developed by {{% mention "winston" %}}, is a network-based Python package that automates the construction of feature-rich (contextual and semantic) urban networks anywhere and at any geographical scale. It enriches OpenStreetMap networks with heterogeneous urban information, such as street view imagery, building morphology, population (including sub-groups), and points of interest, supporting descriptive, modelling, and predictive analyses of cities, as well as comparative studies between them.

The code is openly available on [GitHub](https://github.com/winstonyym/urbanity) under the MIT licence, and it is supported by Google Colab notebooks and [documentation](https://urbanity.readthedocs.io/en/latest/) with tutorials on tasks such as road network classification and building use classification.

## Software

The features of Urbanity include:
+ Rapid city-scale network generation
+ Seamless computation of metric, topological, contextual, and semantic network indicators
+ Node and edge spatial context computation
+ Areal statistics for arbitrary urban subzones
+ Validity checks for OpenStreetMap attribute completeness (number of buildings, percentage with height, percentage with levels, etc.)
+ Primal planar, dual, and spatial graph generation

## Dataset

Using Urbanity, we released an open network dataset covering 50 major cities in 29 countries. It enhances OpenStreetMap networks with more than 40 indicators from open global sources, including streetscape semantic features extracted from more than four million street view images, building morphology, urban population, and points of interest. The dataset is available on [Figshare](https://doi.org/10.6084/m9.figshare.22124219) under the CC BY 4.0 licence.
It is accompanied by an interactive web-based dashboard to explore and compare urban networks, whose source code is available on [GitHub](https://github.com/winstonyym/urbdash).

![](1.png "Workflow for generating the Urbanity network dataset and dashboard: open data are harmonised and integrated into feature-rich urban networks. Data: (c) OpenStreetMap contributors, Mapillary, Meta, GADM. Basemap: Mapbox.")

![](2.png "Examples from the dataset: (a) building footprint proportion around network nodes in ten cities; (b) selected indicators for Tokyo.")

## Papers and attribution

Two papers describe the project, both published open access: one presents the method and the software, and the other the dataset and the dashboard.
Please refer to them for detailed information.

If you use Urbanity in a scientific context, please cite the first paper; if you use the dataset or the dashboard, please cite the second one:

> Yap W, Stouffs R, Biljecki F (2023): Urbanity: automated modelling and analysis of multidimensional networks in cities. npj Urban Sustainability 3: 45. [<i class="ai ai-doi-square ai"></i> 10.1038/s42949-023-00125-w](https://doi.org/10.1038/s42949-023-00125-w) [<i class="far fa-file-pdf"></i> PDF](/publication/2023-npjus-urbanity/2023-npjus-urbanity.pdf)</i> <i class="ai ai-open-access-square ai"></i>

> Yap W, Biljecki F (2023): A Global Feature-Rich Network Dataset of Cities and Dashboard for Comprehensive Urban Analyses. Scientific Data 10: 667. [<i class="ai ai-doi-square ai"></i> 10.1038/s41597-023-02578-1](https://doi.org/10.1038/s41597-023-02578-1) [<i class="far fa-file-pdf"></i> PDF](/publication/2023-sd-urbanitydata/2023-sd-urbanitydata.pdf)</i> <i class="ai ai-open-access-square ai"></i>

```bibtex
@article{2023_npjus_urbanity,
  author = {Yap, Winston and Stouffs, Rudi and Biljecki, Filip},
  doi = {10.1038/s42949-023-00125-w},
  journal = {npj Urban Sustainability},
  title = {Urbanity: automated modelling and analysis of multidimensional networks in cities},
  volume = {3},
  number = {45},
  year = {2023}
}

@article{2023_sd_urbanitydata,
  author = {Yap, Winston and Biljecki, Filip},
  doi = {10.1038/s41597-023-02578-1},
  journal = {Scientific Data},
  title = {A Global Feature-Rich Network Dataset of Cities and Dashboard for Comprehensive Urban Analyses},
  volume = {10},
  pages = {667},
  year = {2023}
}
```

## Authors / Research group

The project was led by {{% mention "winston" %}} and conducted in the [Urban Analytics Lab](/) at the National University of Singapore (NUS).

## Funding and Acknowledgements

This research is part of the project Large-scale 3D Geospatial Data for Urban Analytics, which is supported by the National University of Singapore under the Start Up Grant R-295-000-171-133.
Winston Yap acknowledges the NUS Graduate Research Scholarship granted by the National University of Singapore.
We thank the members of the NUS Urban Analytics Lab for the discussions.
We gratefully acknowledge the contributions of the open-source community.
