---
title: 'Trustworthy Transfer Learning in GeoAI: Assessing Pretrained Models for Rooftop
  Solar PV Mapping Under Geographic Domain Shift'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- Tahsin Hossain
- Tan Yigitcanlar
- Niklas Tilly
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-10-29'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-10-29T13:35:00.000000Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Journal of Geovisualization and Spatial Analysis*'
publication_short: ''

doi: 10.1007/s41651-026-00293-0

abstract: 'The increasing availability of pretrained Geospatial Artificial Intelligence (GeoAI) models has accelerated the operational adoption of deep learning within geographic information systems. However, models developed in one geographic region frequently experience performance degradation when deployed elsewhere because of geographic domain shift. Although transfer learning is widely used to improve cross-regional model performance, it remains unclear whether improved predictive accuracy alone provides sufficient evidence for trustworthy deployment. This study investigates this question using rooftop solar photovoltaic mapping in Brisbane, Australia, as an operational case study. Esri’s pretrained US Solar Panel Detection model was locally calibrated through transfer learning and evaluated using both development and independent local test datasets within Brisbane. Local calibration substantially improved detection performance, increasing recall from 38.5% to 84.1% on the development dataset, with similar improvements observed on the independent 10-grid test dataset, indicating effective local adaptation within the sampled Brisbane environments. However, independent evaluation and qualitative error analysis revealed persistent false positives, missed detections, and geometric segmentation errors, highlighting residual uncertainty and the limitations of model performance within the evaluated geographic context. These findings suggest that transfer learning can substantially improve detection performance and provide useful evidence for assessing operational trustworthiness, although predictive improvements alone are insufficient to establish trustworthy deployment. By integrating complementary evidence relating to robustness, reliability, generalisation, transparency, and residual uncertainty, this study provides an evidence-based operational approach for assessing pretrained GeoAI models and informing responsible deployment decisions in geographically distinct environments.'

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

