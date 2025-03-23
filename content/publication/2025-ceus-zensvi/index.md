---
title: 'ZenSVI: An open-source software for the integrated acquisition, processing
  and analysis of street view imagery towards scalable urban science'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- koichi
- Yihan Zhu
- mahmoud
- xiucheng
- zicheng
- yujun
- tianhong
- rui-ma
- kunihiko
- ouyang-jiani
- matias
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2025-03-20'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2025-03-23T03:42:50.017414Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Computers, Environment and Urban Systems*'
publication_short: ''

doi: 10.1016/j.compenvurbsys.2025.102283

abstract: 'Street view imagery (SVI) has been instrumental in many studies in the past decade to understand and characterize street features and the built environment. Researchers across a variety of domains, such as transportation, health, architecture, human perception, and infrastructure have employed different methods to analyze SVI. However, these applications and image-processing procedures have not been standardized, and solutions have been implemented in isolation, often making it difficult for others to reproduce existing work and carry out new research. Using SVI for research requires multiple technical steps: accessing APIs for scalable data collection, preprocessing images to standardize formats, implementing computer vision models for feature extraction, and conducting spatial analysis. These technical requirements create barriers for researchers in urban studies, particularly those without extensive programming experience. We developed ZenSVI, a free and open-source Python package that integrates and implements the entire process of SVI analysis, supporting a wide range of use cases. Its end-to-end pipeline includes downloading SVI from multiple platforms (e.g., Mapillary and KartaView) efficiently, analyzing metadata of SVI, applying computer vision models to extract target features, transforming SVI into different projections (e.g., fish-eye and perspective) and different formats (e.g., depth map and point cloud), visualizing analyses with maps and plots, and exporting outputs to other software tools. We demonstrated its use in Singapore through a case study of data quality assessment and clustering analysis in a streamlined manner. Our software improves the transparency, reproducibility, and scalability of research relying on SVI and supports researchers in conducting urban analyses efficiently. Its modular design facilitates extensions of the package for new use cases. This package is openly available at https://github.com/koito19960406/ZenSVI, and it is supported by documentation including tutorials (https://zensvi.readthedocs.io/en/latest/examples/index.html).'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/koito19960406/ZenSVI'
url_dataset: ''
url_poster: ''
url_project: 'https://zensvi.readthedocs.io/en/latest/index.html'
url_slides: ''
url_source: ''
url_video: ''

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

# Publication image
# Add an image named `featured.jpg/png` to your page's folder then add a caption below.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects: ['internal-project']` links to `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []
---

