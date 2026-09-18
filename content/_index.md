---
# Leave the homepage title empty to use the site title
title:
date: 2025-10-31
type: landing

sections:
  - block: hero
    content:
      title: |
        <h1 style="text-align:center;">Welcome to the Laboratory of Regeneration Genomics</h1>
  - block: markdown
    content:
      text: |
        <section style="display: flex; align-items: center; justify-content: space-between; max-width: 1200px; margin: auto; gap: 40px;">
          
          <div style="flex: 1; ">
            <p style="font-size: 1.15rem; line-height: 1.6; text-align: justify;">
              Our research aims to unravel the gene regulatory mechanisms that drive cell fate changes during development and tissue regeneration, and to understand how these mechanisms are disrupted in diseases including aging and degenerative disorders. Our long-term goal is to translate these mechanistic insights into innovative regenerative therapeutics. Through our efforts to decode fundamental gene regulatory mechanism, we have also been developing cutting-edge -omics technologies, which benefit both our own research and the broad scientific community.
            </p>
          </div>

          <div id="lab-slides" style="flex: 1; position: relative; overflow: hidden; max-width: 600px;">
            <img src="media/lab4.jpg" style="width:100%; display:block;">
            <img src="media/lab3.jpg" style="width:100%; display:none;">
            <img src="media/lab2.jpg" style="width:100%; display:none;">
            <img src="media/lab1.jpg" style="width:100%; display:none;">
          </div>
          
        </section>

        <script>
          let slides = document.querySelectorAll("#lab-slides img");
          let index = 0;
          setInterval(() => {
            slides[index].style.display = "none";
            index = (index + 1) % slides.length;
            slides[index].style.display = "block";
          }, 3000);
        </script>

  - block: people
    content:
      title: Lab Member
      user_groups:
        - Lab Member
      sort_by: weight
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: false
      columns: '3'

  #- block: collection
  #  content:
  #    title: Latest News
  #    subtitle:
  #    text:
  #    count: 5
  #    filters:
  #      author: ''
  #      category: ''
  #      exclude_featured: false
  #      publication_type: ''
  #      tag: ''
  #    offset: 0
  #    order: desc
  #    page_type: post
  #  design:
  #    view: compact
  #    columns: '1'

  - block: markdown
    content:
      title: <h1 style="text-align:center;">Join Our Team </h1>
      text: |
        
        We are always looking for motivated and curious researchers at all stages (undergraduate and PhD students, postdoctoral fellows) to join our team. Please email Dr. Diao (Yarui.diao@duke.edu) with your CV/resume and a brief description of your research interests.
    
        **We welcome rotation students interested in genomics, epigenetics, stem cells, and tissue regeneration.**

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./papers/" cta_text="Publications →" %}}
    design:
      columns: '1'

  - block: contact
    content:
      title:
      email: diaolab@duke.edu
      #phone: 919-684-8553
      address:
        street: 403 Sands Building
        city: Durham
        region: NC
        postcode: '27710'
      country: United States
      country_code: US
    
---
