---
title: What we deliver
permalink: /what-we-deliver/
layout: primary
lead: We partner with federal agencies to build, buy, and share digital services that improve the user experience of government.
content_wide: true
content_focus: false
redirect_from:
  - /consulting/
banner_cta: false
gridless: true
---

<div class="usa-grid">
  <section class="usa-section">
    <div class="usa-section-bottom">
      <div class="small-caps small-caps-no-margin">Projects</div>
      <h3>Proven experience helping agencies across the government deliver better value to the American public</h3>
      <p>With help from 18F, agencies have moved manual paper processes online, greatly increased data access and usability, saved millions on cloud hosting, and implemented new acquisition techniques. Here are a few examples of the projects we’ve worked on with more than 50 offices and agencies.</p>
    </div>
    <div class="usa-flex usa-flex-wrap">
      {% assign projects_list = site | find_collection: 'projects' | weighted_sort: 'project_weight', 'title' %}
      {% for project in projects_list %}
        {% include card.html
         image_src=project.image
         image_alt=project.image_accessibility
         image_icon=project.image_icon
         tagline=project.title
         description=project.excerpt
         link=project.permalink
        %}
      {% endfor %}
    </div>
  </section>
</div>

<div class="usa-section background-gray">
  <section class="usa-grid">

    </div>
  </section>
</div>
