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
      text: A GeoAI research group at the National University of Singapore
        <br /><br />
        <div>
        <ul class="network-icon" aria-hidden="true">
          <li>
            <a itemprop="sameAs" href="mailto:ual@nus.edu.sg">
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
      title:
      text: |
        {{% callout note %}}
        **We are recruiting!** Two fully funded PhD positions in urban data science are open (August 2027 and January 2028 intakes). We also welcome postdoctoral candidates through external fellowship schemes at NUS. [Details and how to apply](/opportunities/vacancies/).
        {{% /callout %}}
    design:
      columns: '1'
      spacing:
        padding: ["20px", "0", "20px", "0"]

  
  - block: markdown
    content:
      title: About us
      text:         We are developing quantitative methods and tools that leverage emerging urban and geospatial data and AI to sense the form, function, and human experience of cities.

        Read more <a href="/about/">here</a>.<br /><br />

        Established and directed by {{% mention "filip" %}}, we are proudly based at the <a href="https://cde.nus.edu.sg/arch/">Department of Architecture</a> at the <a href="https://cde.nus.edu.sg">College of Design and Engineering</a> of the <a href="https://www.nus.edu.sg">National University of Singapore</a>, a leading global university centered in the heart of Southeast Asia.
    design:
      columns: '2'

  - block: features
    content:
      title: Research themes
      subtitle: Across these themes, we develop GeoAI methods and release open data and software. See [all our publications](/publication/).
      items:
        - name: Street-level imagery
          icon: street-view
          icon_pack: fas
          description: "Street view imagery as a source for measuring cities at human scale: open datasets, software and methods used across the field. Examples: [SVI review](/publication/2021-land-svi-review/), [Global Streetscapes](/publication/2024-global-streetscapes/), [ZenSVI](/publication/2025-ceus-zensvi/)."
        - name: New urban data
          icon: comments
          icon_pack: fas
          description: "Emerging data sources that conventional techniques miss, from place reviews and street video to thermal and nighttime imagery. Examples: [urban functions from reviews](/publication/2026-ceus-urbanfunctions/), [nighttime lights](/publication/2027-rse-nighttime/), [thermal imagery](/publication/2023-sd-iris/), [street view video](/publication/2027-ceus-svv/)."
        - name: Urban dynamics and change
          icon: history
          icon_pack: fas
          description: "Sensing how cities change over time, and what those changes cause. Examples: [physical urban change](/publication/2025-ceus-urbanchange/), [causal effects on cycling](/publication/2024-tra-examining/), [evolution of urban visual environments](/publication/2023-landup-svi-evolution/)."
        - name: Trustworthy urban data and AI
          icon: balance-scale
          icon_pack: fas
          description: "Quality, bias and uncertainty in the data and models behind urban analytics. Examples: [coverage bias](/publication/2025-ceus-svi-coverage/), [seasonal bias](/publication/2025-ceus-svi-seasonality/), [bias in multimodal LLMs](/publication/2026-npj-bias/), [OSM building quality](/publication/2023-bae-osm-qa/)."
        - name: Human experience of cities
          icon: user-friends
          icon_pack: fas
          description: "How people perceive and experience urban environments, including comfort, greenery and health. Examples: [perception and personality](/publication/2025-natcities-specs/), [urban comfort index](/publication/2025-scs-urban-comfort/), [urban motifs and health](/publication/2026-nathealth-motifs/)."
        - name: 3D city models and digital twins
          icon: city
          icon_pack: fas
          description: "Open 3D urban data, simulations and urban digital twins. Examples: [VoxCity](/publication/2026-ceus-voxcity/), [OpenFACADES](/publication/2025-ijprs-openfacades/), [digital twin challenges](/publication/2023-autcon-dt-challenges/)."
    design:
      columns: '1'

  - block: collection
    content:
      title: News
      subtitle: Updates from our group
      text: Feel free to follow us on <a href="https://www.linkedin.com/company/urban-analytics-lab/">LinkedIn</a> and through our [RSS feed]({{< ref path="/post" outputFormat="rss" >}}).
      count: 4
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
      count: 3
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
      view: compact
      columns: '2'

  - block: contact
    id: contact
    content:
      title: Contact
      text: 
      email: ual@nus.edu.sg
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
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: 'https://www.linkedin.com/company/urban-analytics-lab/'
    
      # Automatically link email and phone or display as text?
      autolink: true

    design:
      columns: '2'

---