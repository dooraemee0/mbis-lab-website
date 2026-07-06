---
title: Research
nav:
  order: 1
  tooltip: Research areas and projects
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

MBIS Lab develops biomedical imaging systems, mobile healthcare devices, and AI-based biomedical image analysis methods for next-generation diagnosis, monitoring, and treatment.

Our research focuses on multimodal biomedical systems, mobile healthcare systems, and deep learning-based image analysis and enhancement.

{% include section.html %}

## Research Areas

{% include search-info.html %}

{% include list.html data="research" component="card" %}

{% include section.html %}

## Featured Projects

{% include list.html data="projects" component="card" filter="group == 'featured'" %}

{% include section.html %}

## More Projects

{% include list.html data="projects" component="card" filter="!group" style="small" %}
