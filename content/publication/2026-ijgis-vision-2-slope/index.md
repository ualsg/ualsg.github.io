---
title: 'Vision2Slope: estimating urban road slopes with street view imagery'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- yang-chen
- zicheng
- Hao Li
- Wufan Zhao
- Xin Yang
- Guoan Tang
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-04-16'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-04-19T10:22:53.318405Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*International Journal of Geographical Information Science*'
publication_short: ''

doi: 10.1080/13658816.2026.2656269

abstract: 'Road slopes shape mobility patterns and drive the reliability of urban simulations. Yet in most cities, road-level slope information remains scarce. We introduce Vision2Slope, a framework that leverages panoramic street view imagery to estimate road slopes using computer vision techniques. The workflow consists of three steps: (i) projecting panoramic images into road-aligned views; (ii) semantic-prompted image deskewing to correct geometric distortion induced by camera orientation; and (iii) a two-level slope estimation strategy that extracts point- and segment-level slope and relief characteristics from road-edge geometry and iterative regression to reduce outliers. Using Google Street View images from San Francisco and New York City, the framework estimates slopes for over 60,000 locations and 17,000 street segments. Point- and segment-level MAEs are 0.81°/0.57° and 0.72°/0.78°, respectively, with segment relief errors of 1.70 and 1.66 m. Conditional bias analysis reveals the influence of street-level environmental features on estimation accuracy. The proposed framework significantly outperforms the omnipresent 30 m digital elevation models and maintains robustness under simulated changes in camera orientation and imaging conditions. As an open and scalable workflow, Vision2Slope emphasizes the potential of street view imagery for cost-effective, detailed urban road slope mapping, enriching foundational data for vertical-aware urban analytics.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/CubicsYang/Vision2Slope'
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

