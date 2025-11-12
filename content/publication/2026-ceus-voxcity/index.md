---
title: 'VoxCity: A seamless framework for open geospatial data integration, grid-based
  semantic 3D city model generation, and urban environment simulation'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- kunihiko
- Ryuta Tsurumi
- Tomoki Kiyono
- zicheng
- xiucheng
- binyu
- winston
- koichi
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2025-11-06'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2025-11-12T14:51:46.362823Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*Computers, Environment and Urban Systems*'
publication_short: ''

doi: 10.1016/j.compenvurbsys.2025.102366

abstract: 'Three-dimensional urban environment simulation is a powerful tool for informed urban planning. However, the intensive manual effort required to prepare input 3D city models has hindered its widespread adoption. To address this challenge, we present VoxCity, an open-source Python package that provides a one-stop solution for grid-based 3D city model generation and urban environment simulation for cities worldwide. VoxCity’s ‘generator’ subpackage automatically downloads building heights, tree canopy heights, land cover, and terrain elevation within a specified target area, and voxelizes buildings, trees, land cover, and terrain to generate an integrated voxel city model. The ‘simulator’ subpackage enables users to conduct environmental simulations, including solar radiation and view index analyses. Users can export the generated models using several file formats compatible with external software, such as ENVI-met (INX), Blender, and Rhino (OBJ). We generated 3D city models for eight global cities, and demonstrated the calculation of solar irradiance, sky view index, and green view index. We also showcased microclimate simulation and 3D rendering visualization through ENVI-met and Rhino, respectively, through the file export function. Additionally, we reviewed openly available geospatial data to create guidelines to help users choose appropriate data sources depending on their target areas and purposes. VoxCity can significantly reduce the effort and time required for 3D city model preparation and promote the utilization of urban environment simulations. This contributes to more informed urban and architectural design that considers environmental impacts, and in turn, fosters sustainable and livable cities. VoxCity is released openly at https://github.com/kunifujiwara/VoxCity.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/kunifujiwara/VoxCity'
url_dataset: 'https://github.com/kunifujiwara/VoxCity'
url_poster: ''
url_project: 'https://github.com/kunifujiwara/VoxCity'
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

