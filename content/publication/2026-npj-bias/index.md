---
title: 'Geographic and perceptual bias in multimodal LLMs: evidence from a global
  dataset spanning more than 200 cities'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- Hyebin Kim
- Xuan Li
- matias
- filip
- Sugie Lee

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-08-28'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-09-13T09:50:31.834606Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*npj Urban Sustainability*'
publication_short: ''

doi: 10.1038/s42949-026-00466-2

abstract: 'Multimodal large language models (MLLMs) are increasingly deployed for urban informatics applications, from objective built environment attribute extraction to subjective assessments. However, do MLLMs apply the same standards across regions while executing these urban-related tasks? Are MLLMs reliable and neutral judges? Do they adapt without criticizing, raising concerns about equitable deployment and further hidden bias? Here, we present a geographic red-teaming framework for diagnosing geographic biases in MLLMs applied to image object detection and urban visual perception. Using annotated imagery from more than 200 cities as a standardized benchmark, we demonstrate that MLLMs exhibit significant geographic disparities in both object detection accuracy and perceptual assessments across different regions. Quantitatively, perceptual scores for attributes such as Wealthy and Beautiful dropped by an average of 80% for African cities after geo-referencing, whereas regions such as Asia and North America showed score increases of 26%. A spatial-scale sensitivity test further showed that coordinates, city, country, and continent information produced broadly similar directional shifts, while combined geographic cues generated the strongest perceptual changes. Among the multiple state-of-the-art models, GPT-4o showed the lowest perceptual bias. Our geographic red-teaming stress-tests MLLM performance across underrepresented urban environments, revealing consistent patterns of bias that mirror training-data imbalances. We also provide quantitative metrics for measuring geographic equity in model outputs and establish recommendations for responsible MLLM deployment in urban research. These findings highlight critical limitations in current multimodal AI systems and demonstrate the urgent need for geographically inclusive model development to prevent the perpetuation of urban inequalities through automated analysis systems.'

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

