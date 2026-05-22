---
title: Global Streetscapes - A comprehensive dataset of 10 million street-level images
  across 688 cities for urban science and analytics

# Authors
# A YAML list of author names
# If you created a profile for a user (e.g. the default `admin` user at `content/authors/admin/`), 
# write the username (folder name) here, and it will be replaced with their full name and linked to their profile.
authors:
- yujun
- matias
- maxim-khomiakov
- winston
- ouyang-jiani
- koichi
- zeyu
- tianhong
- filip

# Author notes (such as 'Equal Contribution')
# A YAML list of notes for each author in the above `authors` list
author_notes: []

date: '2024-07-16'

# Date to publish webpage (NOT necessarily Bibtex publication's date).
publishDate: '2024-07-16T11:57:11.847477Z'

# Publication type.
# A single CSL publication type but formatted as a YAML list (for Hugo requirements).
publication_types:
- article-journal

# Publication name and optional abbreviated publication name.
publication: '*ISPRS Journal of Photogrammetry and Remote Sensing*'
publication_short: ''

doi: 10.1016/j.isprsjprs.2024.06.023

abstract: 'Street view imagery (SVI) is instrumental for sensing urban environments, benefitting numerous domains such as urban morphology, health, greenery, and accessibility. Billions of images worldwide have been made available by commercial services such as Google Street View and crowdsourcing services such as Mapillary and KartaView where anyone from anywhere can upload imagery while moving. However, while the data tend to be plentiful, have high coverage and quality, and are used to derive rich insights, they remain simple and limited in metadata as characteristics such as weather, quality, and lighting conditions remain unknown, making it difficult to evaluate the suitability of the images for specific analyses. We introduce Global Streetscapes — a dataset of 10 million crowdsourced and free-to-use SVIs sampled from 688 cities across 210 countries and territories, enriched with more than 300 camera, geographical, temporal, contextual, semantic, and perceptual attributes. The cities included are well balanced and diverse, and are home to about 10% of the world’s population. Deep learning models are trained on a subset of manually labelled images for eight visual-contextual attributes pertaining to the usability of SVI — panoramic status, lighting condition, view direction, weather, platform, quality, presence of glare and reflections, achieving accuracy ranging from 68.3% to 99.9%, and used to automatically label the entire dataset. Thanks to its scale and pre-computed standard semantic information, the data can be readily used to benefit existing use cases and to unlock new applications, including multi-city comparative studies and longitudinal analyses, as affirmed by a couple of use cases in the paper. Moreover, the automated processes and open-source code facilitate the expansion and updates of the dataset and encourage users to create their own datasets. With the rich manual annotations, some of which are provided for the first time, and diverse conditions present in the images, the dataset also facilitates assessing the heterogeneous properties of crowdsourced SVIs and provides a benchmark for evaluating future computer vision models. We make the Global Streetscapes dataset and the code to reproduce and use it publicly available in https://github.com/ualsg/global-streetscapes.'

# Summary. An optional shortened abstract.
summary: ''

tags: []

# Display this page in a list of Featured pages?
featured: false

# Links
url_pdf: ''
url_code: 'https://github.com/ualsg/global-streetscapes'
url_dataset: 'https://github.com/ualsg/global-streetscapes'
url_poster: ''
url_project: '/project/global-streetscapes/'
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

