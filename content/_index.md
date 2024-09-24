---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  # Split the titles into separate blocks
  - block: markdown
    content:
      title: 'Research Focus'
      subtitle: ''
      text: |-
        I am a computational scientist working at the intersection of generative AI and materials science. My academic research explores advanced machine learning techniques, including supervised and unsupervised learning models for novel material discovery. I apply these methods using CV and NLP, particularly leveraging large language models (LLMs) to develop innovative solutions in materials science. I also utilize techniques like density functional theory (DFT) to support my work in materials design and property prediction. You can find my publications within the website or via my Google Scholar link.
    design:
      columns: 1
      css_style: "width: 48%; padding-right: 20px; text-align: left;"

  - block: markdown
    content:
      title: 'Professional Experience'
      subtitle: ''
      text: |-
        Over the past five years, I have gained extensive industry experience in machine learning and computational imaging. As a Senior Machine Learning Engineer at Wavebreak Media, I led projects focused on visual content generation and enhancement. I developed and deployed machine learning models for tasks like text-to-image generation, super-resolution, and 3D asset reconstruction. In this role, I used tools such as AWS, Google Cloud, Flask, Docker, MySQL, and OpenSearch to build scalable AI systems that optimized user experience and data retrieval for millions of assets.
          
          Prior to this, I worked as a Computational Imaging Engineer at Aselsan and Arçelik, where I developed sophisticated optical systems for both defense and consumer electronics. I applied advanced computational techniques, including Fourier optics and ray tracing, to design imaging and display systems, further enhancing my expertise in computational methods and real-world engineering applications.
    design:
      columns: 1
      css_style: "width: 48%; padding-left: 20px; text-align: left;"
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
---
