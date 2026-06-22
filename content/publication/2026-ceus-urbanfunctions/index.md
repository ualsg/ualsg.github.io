---
title: 'Inferring urban functions from Google Maps reviews: A multi-scale, multi-modal
  and cross-city approach'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- liu-haixiao
- sijie
- mahmoud
- yihan
- xiaobing-wei
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-06-22'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-06-22T10:36:02.127816Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Computers, Environment and Urban Systems*'
publication_short: ''

doi: 10.1016/j.compenvurbsys.2026.102475

abstract: 'Characterising and classifying urban functions is a long-standing research focus in urban studies and plays a critical role in urban management and community renewal. However, traditional point-of-interest (POI) categories rely on predefined labels that are often inconsistent across cities and may not fully capture how places are described, represented, or experienced in user-generated data. Further, point-based representations are highly sensitive to spatial aggregation scales, which limits their ability to capture areal functional characteristics and relative differences in POI activity intensity. To address these challenges, we propose a unified framework that, for the first time, leverages place reviews from Google Maps, a form of user-generated geographic information, as a previously untapped POI-linked extended data stream for urban functional inference and classification. Specifically, we employ pre-trained BERT and Vision Transformer models to embed textual and visual information from place reviews, enabling POIs in Singapore and Hong Kong to be represented and clustered within a shared functional embedding space. We then incorporate the weighted volume of place reviews as an indicator of relative POI activity intensity to construct category intensity vectors for spatial units, and demonstrate their effectiveness through cross-city similarity matching tasks. Finally, urban functional classification is conducted across three spatial scales: a 1 km hexagonal grid, administrative areas, and traffic analysis zones (TAZs), using graph neural networks combined with k-means clustering, producing results that preserve spatial continuity and robustness. The proposed framework provides a data-driven approach that highlights the value of place reviews as a complementary data source to conventional POIs and offers a reliable urban functional classification that works across different cities.'

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

