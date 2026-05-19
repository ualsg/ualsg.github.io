---
title: "Modeling adolescents' perception of cycling safety: A new approach using graph
  neural networks and street view imagery"

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- xiaobing-wei
- filip
- pengyuan
- binyu
- Nico Van de Weghe
- Haosheng Huang

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-05-14'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-05-19T12:58:20.233876Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Computers, Environment and Urban Systems*'
publication_short: ''

doi: 10.1016/j.compenvurbsys.2026.102454

abstract: 'Perceived cycling safety remains a critical determinant of bicycle use among adolescents. Previous studies have highlighted the role of street environments in shaping safety perceptions, but most rely on spatial attributes (e.g., road infrastructure, land-use indices) and rarely incorporate the cyclists’ visual perspective. This study proposes a multidimensional framework that integrates visual and spatial representations of urban streets to model perceived cycling safety. By embedding fine-grained visual indicators derived from street view imagery into the road network, this novel framework captures 31 features across six environmental dimensions. Existing studies typically model perceived cycling safety using only a road’s own attributes, neglecting the influence of nearby roads. To address this limitation, we develop an improved Graph Convolutional Network that incorporates geographic context. It integrates layer-wise attention and an adaptive loss function to handle class imbalance and capture spatial dependencies. Explainable artificial intelligence (XAI) techniques are applied to interpret feature importance within the spatial context, moving beyond linear assumptions of traditional models. The framework is applied to a perception survey focusing on adolescents in Ghent, Belgium. The proposed model achieves an overall accuracy of 83.1%, outperforming all baselines and presenting a major advancement in this domain. XAI analysis reveals that both texture complexity and color monotony of the built environment tend to reduce perceived cycling safety, while tree coverage has a positive effect. Overall, the framework offers an interpretable and scalable approach for mapping street-level safety perception, providing actionable insights for cycling-oriented urban design and the development of sustainable transport planning.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: ''
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

