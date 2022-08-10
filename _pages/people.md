---
layout: page
permalink: /people/
title: people
description: members of the lab
nav: true
nav_order: 2

profile:
  align: right
  image: profile.jpg
  image_cicular: false # crops the image to make it circular
#   address: >
#     <p>1601 Trinity Street, 5.202</p>
#     <p>Austin, TX 78712</p>
---

<article>
  {% if page.profile -%}
  <div class="profile float-{%- if page.profile.align == 'left' -%}left{%- else -%}right{%- endif -%}">
    {%- if page.profile.image %}
      {%- assign profile_image_path = page.profile.image | prepend: 'assets/img/' -%}

      {% if page.profile.image_cicular %}
        {%- assign profile_image_class = "img-fluid z-depth-1 rounded-circle" -%}
      {% else %}
        {%- assign profile_image_class = "img-fluid z-depth-1 rounded" -%}
      {% endif %}

      {% include figure.html
      path=profile_image_path
      class=profile_image_class
      alt=page.profile.image -%}
    {% endif -%}
    {%- if page.profile.address %}
    <div class="address">
      {{ page.profile.address }}
    </div>
    {%- endif %}
  </div>
  {%- endif %}

  <div class="clearfix">

Joshua Chang, M.D., Ph.D., is an assistant professor in the Department of Neurology and a courtesy assistant professor in the Department of Population Health.

Chang completed his Bachelor of Science and his Master of Engineering degrees at the Massachusetts Institute of Technology in electrical engineering and computer science, focusing on signal processing and artificial intelligence. His master’s dissertation was completed at the MIT Lincoln Laboratory in missile tracking using different radar modalities.

Before pursuing an M.D./Ph.D. at the University of Massachusetts Medical School, he worked as a software engineer at the Broad Institute and Harvard’s School of Public Health and Center for Health Decision Science. At UMass, he completed a thesis in quantitative health sciences and neurology under the supervision and mentorship of David Paydarfar, designing and developing adaptive control algorithms to optimize stimulus waveforms for implantable medical devices. He continues his research at Dell Medical School, studying ways to leverage artificial intelligence to better improve population health through health care across diagnostics, therapeutics and predictive analytics.
</div>
