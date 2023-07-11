---
layout: page
title: electroceuticals
description: Understanding how electrical stimulation can be optimized as a medical therapeutic
img: assets/img/12.jpg
importance: 1
category: computational modeling
---

### Description
There is considerable interest in leveraging electrical stimulation as a medical therapeutic. This has led to an interest in “electroceutical” therapies. While there has been a lot of success and FDA-approved devices (including deep brain stimulation for Parkinson’s disease, vagus nerve stimulation for epilepsy, retinal ganglion stimulation for retinopathy), the underlying mechanisms are not fully understood. Much of the focus today is on the use of rectangular waveforms, but our lab hypothesizes that non-traditional, customized waveforms can produce more energetically-efficient and selective stimulation. We are working on developing novel algorithms to find these more efficient waveform, as well as discovering the mechanisms underlying how these non-traditional waveforms are unlocking different access mechanisms for selective stimulation.

### Relevant Publications
<div class="publications">
    {% bibliography -f papers -q @*[project=electroceuticals]* -t _layouts/bib2.html %}
</div>

### Relevant Repositories
<!-- code for GitHub repositories -->
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}