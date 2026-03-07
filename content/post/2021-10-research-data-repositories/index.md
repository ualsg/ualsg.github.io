---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Exploration of research data repositories"
subtitle: ""
summary: "A non-exhaustive list of research data repositories and a comparison of them."
authors: [yoong-shin]
tags: [research data, data repositories, open data, data management planning, research data management]
categories: []
date: 2021-10-25T09:34:24+08:00
lastmod: 2021-10-25T09:34:24+08:00
featured: false
draft: false
show_related: true
pager: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Photo by [benjamin lehman](https://unsplash.com/@benjaminlehman?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/data-archive?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
  "
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

It is inevitable these days that researchers depend heavily on various kinds and sources of data.  They usually start from one or more sources of input data, and some generate datasets that are contributed as open data, available to the public upon the publication of papers. In some cases, these open data may be in multiple versions as data being updated, or new data is added. Customisable access control may be a requirement if the research data is part of the peer-review process as the research paper. Thus, it is critical when choosing a data repository, we evaluate it against our use case and data management workflow and requirements.   

While searching for a data repository solution for our projects, we find the information regarding research data repositories and open data repositories are scattered over the internet. We decided to compile a list of repositories that we found relevant to our field, perform a comparison among them. We hope that other research groups will find this exploration useful when deciding how to share open data arising from their projects.

In general, there are four categories of research data repository options: 

1) data repositories associated with academic institutes, 
1) generic open data repositories, 
1) open data registry backed by private companies, and 
1) self-hosted 
   
There is an endless list of options for each of these categories, so we have selected a few major ones in each to compare and contrast. The comparison is performed based on the following aspects that are important to us:

- supported file format
- file size limitation
- total storage space limitation
- version control
- access control
- data license requirements
- cost


### Academic Data Repositories

These repositories are usually set up within an academic institute to host the research publications and/or research data of research labs in the institute. While such systems are set up within the institute, some, like Dataverse at Harvard University and ICPSR at the University of Michigan, are open to host publications and data contributed by researchers from other academic institutes.  

Here we compare ScholarBank@NUS, Dataverse@Harvard and ICPSR@UMich. 

{{< figure src="academic-repos.jpg" title="Comparison of academic repositories. Click [here](academic-repos.jpg) for the image in full-size." numbered="false" lightbox="true" >}}

### General Research Data Repositories

Other than the academic research repositories, there other types of general research data repositories. These are generally partnered with publishers, associated with government sectors, or backed by non-profits organisations. 

In comparison with the academic institute backed research repositories, most of these repositories could offer free data deposition/maintenance services, while some take donations, or offer membership/subscription for higher allowance of storage. Below is the comparison between FigShare, Dryad, Zenodo, Open Science Framework (OSF), Pangeae and Mendeley Data.  

{{< figure src="generic-repos.jpg" title="Comparison of general repositories. Click [here](generic-repos.jpg) for the image in full-size." numbered="false" lightbox="true" >}}


### Open Data Repositories Backed by Private Companies

Many private companies have also shown support in the Open Data movement and offer hosting 
and registry of various datasets. The terms and conditions for these data repositories are not 
usually publicly accessible, and need to be negotiated with the company who backed them 
respectively. 

Here are the options we looked into open data solution offered by Amazon Web Services, Google 
Cloud, and Microsoft. 

{{< figure src="private-repos.jpg" title="Comparison of repositories provided by private companies. Click [here](private-repos.jpg) for the image in full-size." numbered="false" lightbox="true" >}}


### Self-Hosting

Lastly, there is always the option to self-host the research data. This option may offer more flexibility, freedom and ease to update the dataset as we wish, but it requires the development and maintenance of a data access portal, and technical maintenance of a web server, in addition to research data management. Depending on the simplicity of the data access portal, advanced features such as download statistics, version control and user access module could require effort to implement.  


### Summary

Although this list is not complete with all the research data repositories available, we hope this provides enough viable options for our future research and those who are looking for open data repository solutions. We also welcome other suggestions that we may have overlooked. 

For those who are interested in more detail, the comparison can be found in a spreadsheet [here](https://docs.google.com/spreadsheets/d/1XTWrlJrfxWs1I5_fEZjnw0H_H5qDtiAmafvTh4QRBhg/edit?usp=sharing). 

