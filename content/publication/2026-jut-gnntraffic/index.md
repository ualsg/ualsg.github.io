---
title: A Graph-Based Human-Centered GeoAI for Understanding Street-Level Environment
  and Traffic Accident Frequency with Street View Imagery

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- pengyuan
- winston
- yujun
- binyu
- Rudi Stouffs
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-07-14'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-07-17T08:39:15.395011Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Journal of Urban Technology*'
publication_short: ''

doi: 10.1080/10630732.2026.2665592

abstract: 'Traffic accidents are a major global concern, highlighting the need for advanced traffic analysis and predictive techniques. The emergence of crowdsourced street view imagery (SVI) platforms has transformed public participation in collecting urban data, initiating the development of human-centered traffic analytics. This article investigates the relationship between visual urban understanding derived from Mapillary SVI and the frequency of urban traffic accidents. We analyzed SVI’s visual complexities using the Mask2Former image segmentation model and provided spatial reasoning of the urban objects (e.g., cars, buildings, trees) by estimating visual distances between those objects and the drivers using Dist-YOLOv5. These distances were encapsulated as edge weights, with urban objects and the drivers as nodes, creating human-centered graphs at each SVI location. We propose a framework that integrates a graph-based deep learning approach, GAT-LSTM, to capture the spatial-temporal dynamics of these urban objects for modeling traffic-accident frequency. Our results indicate that this model outperforms a traditional machine learning method by over 70 percent in mean absolute percentage error (MAPE) and demonstrates superior performance compared to other deep learning-based methods. Additionally, we introduce a two-step Explainable AI (XAI) method to identify key factors associated with roads with higher traffic accident rates, thereby improving the interpretability and practicality of our research for understanding the urban safety environment.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/PengyuanLiu1993/SensingUrbanTraffic'
url_dataset: ''
url_poster: ''
url_project: ''
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

