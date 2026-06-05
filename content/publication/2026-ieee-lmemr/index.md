---
title: Learning Fine-Grained Urban Mobility Dynamics Through Large Model-Enhanced
  Multimodal Representations

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- tianhong
- Jianbin Li
- Jinzhou Cao
- Wei Tu
- filip
- Shengao Yi
- Zhilu Yuan

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-05-29'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-06-05T09:58:14.608733Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*IEEE Transactions on Intelligent Transportation Systems*'
publication_short: ''

doi: 10.1109/tits.2026.3696956

abstract: 'Accurately predicting fine-grained urban mobility is essential for optimizing transportation, accessibility, and urban management. However, existing approaches often depend on dynamic data such as trajectories or signaling records, which are sparsely available across cities, thereby limiting their applicability and generalizability to new urban contexts. To address these limitations, this study proposes a Large Model Enhanced Multimodal Representations (LMEMR) framework to learn hourly grid-level mobility dynamics solely from static geospatial data—including remote sensing imagery, building data, street view imagery, and points of interest—which are widely accessible. Large vision–language models are employed to generate natural-language descriptions of each modality, enriching the data with human-understandable semantics. A dual-level contrastive learning strategy aligns raw and textual features both within and across modalities, mitigating semantic gaps and enhancing multimodal consistency. Spatial dependencies are modeled through a graph attention network, and temporal dynamics are captured via a transformer encoder to produce 24-hour mobility sequences. Results from Shenzhen demonstrate that LMEMR outperforms the baseline CLIP model, achieving an $R^{2}$ of 0.856and an 18.07% reduction in MAE. Ablation experiments confirm the effectiveness of semantic enhancement, spatial graph reasoning, and cross-modal fusion. Overall, this research reveals the potential of static multimodal data for dynamic mobility inference, offering a scalable, interpretable, and privacy-friendly solution for smart city planning and management.'

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

