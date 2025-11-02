---
# Leave the homepage title empty to use the site title
title:
date: 2025-10-31
type: landing

sections:
  - block: hero
    content:
      title: |
        <h1 style="text-align:center;">👋Welcome to the Laboratory of Regeneration Genomics</h1>
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
        
        Our research program, **'Regeneration Genomics'**, is dedicated to unraveling the gene regulatory mechanisms that drive cell fate changes in development and regeneration. In our quest to decode the fundamental principles of gene regulation, I have been developing several cutting-edge genomic tools, such as **CREST-seq**, **CARGO-BioID**, **HiCAR**, and **scHiCAR** that benefit both our own research and the broader scientific community.
        
        Since the starting of our lab at Duke Cell Biology in September 2018, we have been focused on both human pluripotent stem cells and muscle stem cells and their “niche” in regeneration, aging, and degenerative disorders, combining mechanistic studies with genomic technologies. Over the past five years, our recent discoveries include: (1) the pathological role of macrophage and FAPs in muscular dystrophy and Peripheral Artery Disease (PAD) (**_Genome Medicine_ 2023, _JVS-VS_ 2025, _Nature Communications_, _minor revision_**); (2) single cell epigenomics and mechanistic analyses of muscle stem cell self-renewal fate (**_JCB_ 2023**); (3) the impact of transposable elements on stem cell fate (**_Nature Genetics_ 2023, _Nature Cell Biology_ 2025**); and (4) the development of novel 3D genome, proteomics, and single cell multi-omics tools to map chromatin architecture and protein–DNA interactions (**_Molecular Cell_ 2022, _Nature Genetics_ 2023, _Nature Biotechnology_, in press**). In addition to our own research, our lab have also contributed to over 20 collaborative publications by providing our strong expertise in genomics, stem cell biology, regeneragion, and bioinformatics.
        
        As a team of cell biologists and genomic scientists, we integrate comprehensive molecular, cellular, genomic, and genetic approaches with patient biopsies, organoids, and genetically engineered mouse models. By combining both experimental and computational methods, we aim not only to make fundamental discoveries but also to foster a rigorous and supportive training environment for the next generation of scientists. Our former technicians and undergraduate trainees have entered top graduate and medical schools; our PhD students have received prestigous research awards and advanced to postdoctoral positions at leading U.S. institutions; and our postdoctoral fellows have secured tenure-track faculty appointments or established successful careers in industry.

  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
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
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="/Publication/" cta_text="Publications →" %}}
    design:
      columns: '1'

  - block: contact
    content:
      title: 
      email: diaolab@duke.edu
      phone: 919-684-8553
      address:
        street: 406 Sands Building
        city: Durham
        region: NC
        postcode: '27710'
        country: United States
        country_code: US
---
