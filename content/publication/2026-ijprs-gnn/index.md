---
title: Heterogeneous graph neural networks for building attribute prediction from
  hierarchical urban features and cross-view imagery

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- xiucheng
- winston
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-02-20'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-02-21T01:23:55.830334Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*ISPRS Journal of Photogrammetry and Remote Sensing*'
publication_short: ''

doi: 10.1016/j.isprsjprs.2026.02.016

abstract: 'Data on building properties are essential for a variety of urban applications, yet such information remains scarce in many parts of the world. Recent efforts have leveraged instruments such as machine learning (ML), computer vision (CV), and graph neural networks (GNNs) to assess these properties at scale by leveraging urban features or visual information. However, extracting holistic representations to infer building attributes from multi-modal data across multiple spatial scales and vertical building characteristics remains a significant challenge. To bridge this gap, we present a innovative framework, that captures both hierarchical urban features and cross-view visual information through a heterogeneous graph. First, we construct a heterogeneous graph that incorporates multi-dimensional urban elements — buildings, streets, intersections, and urban plots — to comprehensively represent multi-scale geospatial features. Second, we automatically crop images of individual buildings from both very high-resolution satellite and street-level imagery, and introduce feature propagation on semantic similarity graphs to supplement missing facade information. Third, feature fusion is applied to integrate both morphological and visual features, with holistic representations generated for building attribute prediction. Systematic experiments across three global cities demonstrate that our method outperforms existing CV, ML, and homogeneous GNN-based models, achieving classification accuracies of 86% to 96% across 10 to 12 distinct building types, with mean F1 scores ranging from 0.70 to 0.73. The framework demonstrates robustness to class imbalance and produces more distinctive embeddings for ambiguous categories. In additional task of inferring building age, the method delivers similarly strong performance. This framework advances scalable approaches for filling gaps in building attribute data and offers new insights into modeling holistic urban environments. Our dataset and code are available openly at: https://github.com/seshing/HeteroGNN-building-attribute-prediction.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/seshing/HeteroGNN-building-attribute-prediction'
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
