---
title: OpenFACADES
summary: An open framework for architectural caption and attribute data enrichment via street view imagery.
authors: [xiucheng]
profile: true  # Show author profile?
date: 2025-11-02T09:30:16+08:00
lastmod: 2025-11-02T09:30:16+08:00

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false
---

# An open framework for architectural caption and attribute data enrichment via street view imagery

OpenFACADES, developed by {{% mention "xiucheng" %}}, is an open-source framework designed to enrich building profiles with objective attributes and semantic descriptors by leveraging multimodal crowdsourced data and large vision-language models. It provides tools for integrating diverse datasets, automating building facade detection, and generating detailed annotations at scale.

The code, models, and data are openly available on [GitHub](https://github.com/seshing/OpenFACADES), and it is supported by a Google Colab and documentation.

![](1.png "General framework for integrating multimodal crowdsourced data to establish a street-level building dataset and develop multimodal models. Data: (c) Mapillary and OpenStreetMap contributors.")

This open toolkit acquires individual building images from Mapillary and uses open-source LLMs for annotation. Specifically: 
1. The pipeline can geolocate, collect, and filter holistic building images from panoramic street view images around the world, integrating them with open building data into a structured dataset. 
1. We compiled a global dataset of 31,180 annotated building images from seven cities and 1.2M auto-labeled images, enriched with geospatial attributes (e.g., type, floors, age, material) and descriptive captions. 
1. We fine-tuned and openly released LLMs that demonstrate strong robustness and generalization across cities.

![](6.png "Comparison of OSM building data (left) and the building attributes inferred using our method (right) in Washington D.C., illustrating attributes: building type, surface material, number of floors, and age. Data: (c) OpenStreetMap contributors.")


## Paper and attribution

A [paper](https://doi.org/10.1016/j.isprsjprs.2025.10.014) describing the project was published in the _ISPRS Journal of Photogrammetry and Remote Sensing_.
Please refer to it for detailed information.

If you use OpenFACADES in a scientific context, please cite the paper:

> Liang X, Xie J, Zhao T, Stouffs R, Biljecki F (2025): OpenFACADES: An open framework for architectural caption and attribute data enrichment via street view imagery. ISPRS Journal of Photogrammetry and Remote Sensing 230: 918-942. [<i class="ai ai-doi-square ai"></i> 10.1016/j.isprsjprs.2025.10.014](https://doi.org/10.1016/j.isprsjprs.2025.10.014) [<i class="far fa-file-pdf"></i> PDF](/publication/2025-ijprs-openfacades/2025-ijprs-openfacades.pdf)</i>

```bibtex
@article{2025_ijprs_openfacades,
  author = {Liang, Xiucheng and Xie, Jinheng and Zhao, Tianhong and Stouffs, Rudi and Biljecki, Filip},
  doi = {10.1016/j.isprsjprs.2025.10.014},
  journal = {ISPRS Journal of Photogrammetry and Remote Sensing},
  pages = {918--942},
  title = {OpenFACADES: An open framework for architectural caption and attribute data enrichment via street view imagery},
  volume = {230},
  year = {2025}
}
```



## Authors / Research group

The project was led by {{% mention "xiucheng" %}} and conducted in the [Urban Analytics Lab](/) at the National University of Singapore (NUS).
The full list of people involved is listed in the paper.

## Funding and Acknowledgements

This research is part of the project Large-scale 3D Geospatial Data for Urban Analytics, which is supported by the National University of Singapore under the Start Up Grant.
This research is part of the project Multi-scale Digital Twins for the Urban Environment: From Heartbeats to Cities, which is supported by the Singapore Ministry of Education Academic Research Fund Tier 1.
The first author acknowledges the NUS Graduate Research Scholarship granted by the National University of Singapore (NUS).
We thank the members of the NUS Urban Analytics Lab for the discussions.
We also acknowledge the contributors of OpenStreetMap, Mapillary and other platforms for providing valuable open data resources and code that support street-level imagery research and applications.
