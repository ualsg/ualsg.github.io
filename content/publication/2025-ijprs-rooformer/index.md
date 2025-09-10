---
title: 'RooFormer: Reconstructing detailed 3D roof models from high-resolution remote sensing imagery using transformer'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- yu-dayu
- Fan Ye
- Peng Yue
- Min Chen
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2025-07-10'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2025-07-16T12:58:28.263029Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*ISPRS Journal of Photogrammetry and Remote Sensing*'
publication_short: ''

doi: 10.1016/j.isprsjprs.2025.06.010

abstract: 'Building roofs are essential for various geographical analyses such as solar potential analysis and urban microclimate simulation. Despite growing demand, reconstructing detailed 3D roofs remains challenging due to the complexity of roof geometries and variations in architectural styles. This paper introduces RooFormer, an end-to-end learning framework for reconstructing detailed and textured 3D roof models in mesh format from high-resolution imagery. RooFormer consists of a MaskFormer branch, which identifies and focuses on roof features, and a MeshFormer branch, which predicts detailed roof meshes. In the MeshFormer branch, a local self-attention mechanism is employed to understand mesh features, and a positional embedding layer is designed to integrate geometric and texture features. In addition, to measure the geometric similarity between predicted meshes and ground truth, we develop a loss function that integrates terms from both image and mesh spaces. Compared to existing 3D metrics, the proposed geometric loss term more accurately reflects the geometric differences in meshes. Experiments show that its normalized height error of 0.014 is lower than the 0.034 error of state-of-the-art methods. Visually, the reconstruction accurately reflects the geometric contours and structures of roofs, even with slight occlusions. We also demonstrate its generalization by testing it across various areas. The framework promises to enable richer building modeling and analysis for a wide range of digital city applications.'

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

