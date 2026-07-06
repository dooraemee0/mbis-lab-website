---
title: Projects
nav:
  order: 3
  tooltip: Research projects and systems
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

MBIS Lab develops biomedical systems and computational methods for medical imaging, healthcare monitoring, and AI-based medical data analysis.

{% include tags.html tags="multimodal-imaging, mobile-healthcare, deep-learning, ultrasound, endoscopy, ECG" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filter="group == 'featured'" %}

{% include section.html %}

## More

{% include list.html component="card" data="projects" filter="!group" style="small" %}
