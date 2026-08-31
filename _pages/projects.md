---
layout: page
title: research
permalink: /projects/
description: Research projects at the PRN PAIN Lab.
nav: true
nav_order: 2
display_categories: [research, education]
horizontal: false
---

<style>.card-img-top{aspect-ratio:1/1!important;object-fit:cover!important;object-position:center center!important;}</style>

Our research focuses on improving pediatric pain assessment, management, and outcomes through innovative technologies and evidence-based practice. We combine expertise in nursing science, computer science, industrial engineering, and data science to develop solutions that address gaps in pain care for vulnerable populations.

Current projects include **MIDAS** (Modeling Inter-individual Differences to Address Pain of Sickle Cell Disease), an NIH-funded initiative using machine learning to predict and prevent chronic pain in sickle cell disease, and **PRAMS** (Pain Recognition and Assessment Monitoring System), an NSF-funded project developing AI-driven neonatal pain detection using federated learning. We also maintain the **Pediatric Pain PRN Curriculum**, an open-access resource for evidence-based pediatric pain education.

<div style="background-color: #9ccc65; padding: 1.5rem 2rem; margin: 2rem 0 0 0;">
<h2 style="margin: 0; font-size: 1.75rem; font-weight: 400; color: #000; font-family: Georgia, 'Times New Roman', serif;">Pediatric Healthcare Providers Knowledge and Attitude Survey Regarding Pediatric Pain</h2>
</div>
<div style="border: 2px solid #2a5a8a; border-top: none; padding: 2rem 2.5rem; margin: 0 0 2rem 0; background: var(--global-bg-color); color: var(--global-text-color); font-family: Georgia, 'Times New Roman', serif; font-size: 0.95rem; line-height: 1.35; font-weight: 400;">

<p style="margin-bottom: 1.4rem; font-weight: 700;">This statement serves as permission to use and duplicate the ©2019 Renee Manworren: Pediatric Healthcare Providers' Knowledge and Attitudes Survey Regarding Pain for clinical, educational, and research purposes.  It does not authorize any changes to the survey, except changes to the demographic questions to reflect your study subjects.</p>

<p style="margin-bottom: 1.4rem;">You can direct healthcare providers and/or students to access the survey by <a href="https://utaedu.questionpro.com/a/TakeSurvey?tt=5lEwPCvYG6wECHrPeIW9eQ%3D%3D" style="color: #0064b1;">clicking here to take the test</a> or <strong>the button below.</strong> If you print and use the tool on paper to migrate this into your own secure survey system, please note that it uses branching logic (changes by prescriber, care of patients with cancer, and profession). You can trial the survey without storing the data by including "Manworren" in the unique identifier field.</p>

<p style="margin-bottom: 1.4rem;">Permission for the use of this survey has been granted to hundreds of organizations in the United States, as well as institutions in the United Kingdom, Ireland, Australia, South Africa, Canada, &amp; New Zealand. These surveys have been translated by researchers and educators in China, Greece, Indonesia, Iran, Iraq, Israel, Italy, Korea, Malaysia, Mongolia, Norway, Peru, Philippines, Portugal, Qatar, Switzerland, Taiwan, and Vietnam for use with healthcare professionals in these countries. Publications on the survey have been cited by authors from 42 countries across 6 continents, indicating widespread dissemination (source: Scopus).</p>

<p style="margin-bottom: 1.4rem;"><em>The manuscript on the validity and reliability of the survey was published:</em><br>
<em>Manworren, RCB &amp; LaPrise, J. Development of the Pediatric Healthcare Providers' Knowledge and Attitudes Survey Regarding Pain. Pediatr Nurs. 2021; 47(6):275–291.</em></p>

<p style="margin-bottom: 0; font-weight: 700;">If you would like to translate the tool or make other changes, please contact Dr. Manworren at <a href="mailto:renee.manworren@tamu.edu" style="color: #0064b1;">renee.manworren@tamu.edu</a>.</p>

</div>

<div style="text-align: center; margin-bottom: 2.5rem;">
<a href="https://utaedu.questionpro.com/a/TakeSurvey?tt=5lEwPCvYG6wECHrPeIW9eQ%3D%3D" style="display: inline-block; border: 2px solid var(--global-text-color); padding: 0.3rem 2rem; font-family: Arial, Helvetica, sans-serif; font-size: 0.95rem; font-weight: 700; text-decoration: none; color: var(--global-text-color); letter-spacing: 0.03em;">CLICK HERE TO TAKE THE TEST</a>
</div>

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
