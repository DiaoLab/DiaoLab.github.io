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

  - block: markdown
    content:
      title: <h1 style="text-align:center;">Research</h1>
      text: |
        
        <img src="media/research.jpg" alt="Research" style="float:right; margin: 0 0 15px 20px; width:40%; border-radius:12px; opacity:0.85;">
        
                Our research program, **'Regeneration Genomics'**, seeks to understand the gene-regulatory mechanisms that drive cell-fate transitions during development and regeneration, and how disruption of these mechanisms contributes to degenerative disease. We also develop cutting-edge genomic technologies that benefit both our own research and the broader scientific community.

        Since establishing the lab in Duke Cell Biology in September 2018, we have focused on human pluripotent stem cells, muscle stem cells, and their microenvironment in development, regeneration, aging, and degenerative disease. Over the past five years, our work has contributed to three major areas: (1) delineating the function and regulation of non-coding regulatory DNA, including transposable elements, in controlling pluripotent and muscle stem cell fate (**_JCB 2023_**; **_Nature Genetics 2023_**; **_Nature Cell Biology 2025_**); (2) uncovering how muscle stem-cell niche populations, including macrophages and fibro-adipogenic progenitors (FAPs), contribute to muscular dystrophy and peripheral artery disease (**_Genome Medicine 2023_**; **_JVS-VS 2025_**; **_Cell Stem Cell 2026_**; **_Nature Communications, revision_**); and (3) developing new 3D-genome, proteomic, and single-cell multi-omic technologies to map chromatin architecture and protein–DNA interactions (**_Molecular Cell 2022_**; **_Nature Genetics 2023_**; **_Nature Biotechnology 2026_**).

        As a team of cell biologists and genomic scientists, we integrate molecular, cellular, genomic, genetic, and computational approaches with patient biopsies, organoids, and genetically engineered mouse models. Our goal is not only to make fundamental discoveries about gene regulation and regenerative biology, but also to translate these insights into innovative therapeutic strategies. Equally important, we are committed to providing a rigorous and supportive training environment for the next generation of scientists, including undergraduate students, graduate students, and postdoctoral fellows.

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
