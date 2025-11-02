---
# Leave the homepage title empty to use the site title
title:
date: 2025-09-13
type: landing

sections:
  - block: hero
    content:
      title: Urban Analytics Lab
      image:
        filename: urbanity3.png
      text: A research group at the National University of Singapore
        <br /><br />
        <div>
        <ul class="network-icon" aria-hidden="true">
          <li>
            <a itemprop="sameAs" href="mailto:filip@nus.edu.sg">
              <i class="fas fa-envelope big-icon"></i>
            </a>
          </li>
          <li>
            <a itemprop="sameAs" href="https://www.linkedin.com/company/urban-analytics-lab/" target="_blank" rel="noopener">
              <i class="fab fa-linkedin big-icon"></i>
            </a>
          </li>  
          <li>
            <a itemprop="sameAs" href="https://scholar.google.com/citations?user=jGqm4kEAAAAJ&hl=en" target="_blank" rel="noopener">
              <i class="ai ai-google-scholar big-icon"></i>
            </a>
          </li>  
          <li>
            <a itemprop="sameAs" href="https://www.researchgate.net/profile/Filip_Biljecki" target="_blank" rel="noopener">
              <i class="ai ai-researchgate big-icon"></i>
            </a>
          </li>
          <li>
            <a itemprop="sameAs" href="https://github.com/ualsg" target="_blank" rel="noopener">
              <i class="fab fa-github big-icon"></i>
            </a>
          </li>
        </ul>
        </div>
    design:
      background:
        color: 'black'
        text_color_light: true
  
  - block: markdown
    content:
      title: About us
      text: <div style="padding:56.25% 0 0 0;position:relative;">
        <iframe src="https://player.vimeo.com/video/764033095?h=f100addf1d&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen>
        </iframe>
        </div>
        <script src="https://player.vimeo.com/api/player.js"></script>
        <br />

        We are introducing innovative methods, datasets, and software to derive new insights in cities and advance data-driven urban planning, digital twins, and geospatial technologies in establishing and managing the smart cities of tomorrow. 

        Converging multidisciplinary approaches inspired by recent advancements in computer science, geomatics and urban data science, and influenced by crowdsourcing and open science, we conceive cutting-edge techniques for urban sensing and analytics at the city-scale.
        Watch the <a href="https://vimeo.com/764033095">video</a> above or read more <a href="/about/">here</a>.<br /><br />

        Established and directed by {{% mention "filip" %}}, we are proudly based at the <a href="https://cde.nus.edu.sg/arch/">Department of Architecture</a> at the <a href="https://cde.nus.edu.sg">College of Design and Engineering</a> of the <a href="https://www.nus.edu.sg">National University of Singapore</a>, a leading global university centered in the heart of Southeast Asia.
        We are also affiliated with the <a href="https://bschool.nus.edu.sg/real-estate/">Department of Real Estate</a> at the <a href="https://bschool.nus.edu.sg">NUS Business School</a>.
    design:
      columns: '2'

  - block: collection
    content:
      title: News
      subtitle: Updates from our group
      text: Feel free to follow us on <a href="https://www.linkedin.com/company/urban-analytics-lab/">LinkedIn</a> and through our [RSS feed]({{< ref path="/post" outputFormat="rss" >}}).
      count: 7
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: compact
      columns: '2'

  - block: people
    content:
      title: People
      text: We are an ensemble of scholars from diverse disciplines and countries, driving forward our shared research goal of making cities smarter and more data-driven. Since 2019, we have been fortunate to collaborate with many talented alumni, whose invaluable contributions have shaped and enriched our research group, and set the scene for future developments. The full list of our members is available [here](/people). <br /><br />

      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - People
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: false

  - block: collection
    content:
      title: Recent publications
      subtitle: Full list of publications is [here](/publication/).
      text:
      count: 5
      filters:
        author: ''
        category: ''
        featured_only: false
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: publication
    design:
      view: card
      columns: '2'

  - block: contact
    id: contact
    content:
      title: Contact
      text: 
      email: filip@nus.edu.sg
      phone: 
      address:
        street: SDE4, NUS College of Design and Engineering, 8 Architecture Dr
        city: Singapore
        region: Singapore
        postcode: '117564'
        country: Singapore
        country_code: SG
      coordinates:
        latitude: '1.29695'
        longitude: '103.77026'
      directions: 
      office_hours:
      appointment_url: ''
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: X
          link: 'https://twitter.com/urbanalyticslab'
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: 'https://www.linkedin.com/company/urban-analytics-lab/'
    
      # Automatically link email and phone or display as text?
      autolink: true

    design:
      columns: '2'

---