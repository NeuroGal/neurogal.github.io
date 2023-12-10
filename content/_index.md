---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About me
      username: admin       # Choose a user profile to display (a folder name within `content/authors/`)
  - block: skills
    content:
      title: Skills
      text: ''
      username: admin       # Choose a user to display skills from (a folder name within `content/authors/`)
    design:
      columns: '1'
  - block: markdown # or use list? check https://docs.hugoblox.com/getting-started/page-builder/
    id: recent
    content:
      title: Recent Activity
      text: '- Thing 1 testing'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Publications # change to 'Recent Publications' ?
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false # true
    design:
      columns: '2'
      view: citation
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
    #  text: |-
    #    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      # email: gal.vishne@gmail.com
#      phone: 888 888 88 88
#      appointment_url: 'https://calendly.com'
      address:
        street: Edmond J. Safra Campus, The Hebrew University
        city: Jerusalem
       # region: CA
        postcode: '9190401'
        country: Israel
        country_code: IL
      directions: The Suzanne and Charles Goodman Brain Sciences Building
#      office_hours:
#        - 'Monday 10:00 to 13:00'
#        - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '31.7713' 
        longitude: '35.19663'   
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/neuro_gal'
      autolink: true       # Automatically link email and phone or display as text?
      form: # "mailto:your-email@example.com"       # Email form provider
        provider: formspree
        formspree: 
          id: xjvqdozo
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'



#        - icon: skype
#          icon_pack: fab
#          name: Skype Me
#          link: 'skype:echo123?call'
#        - icon: video
#          icon_pack: fas
#          name: Zoom Me
#          link: 'https://zoom.com'
---
