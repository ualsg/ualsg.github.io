---
title: 'Open Urban Simulations All the Way: Extending VoxCity to CityGML and Project
  PLATEAU'

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- kunihiko
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2026-09-28'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2026-10-10T13:33:15.275124Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*ISPRS Annals of the Photogrammetry, Remote Sensing and Spatial Information
  Sciences*'
publication_short: ''

doi: 10.5194/isprs-annals-xii-4-w1-2026-137-2026

abstract: 'CityGML is a prominent standard for semantic 3D city models, and a growing number of open 3D city models are available in this format worldwide. It supports urban simulations, such as assessing microclimate and visual environments, but its potential has not been fully realized due to a lack of free and open-source simulation software compatible with CityGML. Consequently, when data is available in CityGML, it commonly serves its purpose as an exchange format and is converted to other formats. This creates a major bottleneck for the widespread adoption of urban environment simulations since preparing simulation-ready models often entails fixing geometries and resolving conversion issues. To address this shortcoming, we introduce an extension to the open-source Python package “VoxCity” that offers seamless functionality to parse CityGML files, fill in missing data by integrating open geospatial data, generate voxel-based meshes, and perform urban environment simulations. It is one of the few open-source software solutions that are CityGML-compliant. We demonstrate the framework using CityGML data for Tokyo and Osaka from Project PLATEAU— which covers more than 250 cities in Japan—through two use cases: (1) window green views, and (2) pedestrian sunlight exposure. Our package, VoxCity, and the newly developed extension are freely available at https://github.com/kunifujiwara/VoxCity and https://github.com/kunifujiwara/VoxCityGML, respectively. We believe that this framework will facilitate the application of CityGML in urban environment simulations by reducing the time and effort required.'

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
