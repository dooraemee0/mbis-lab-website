---
title: MBIS-Git
---

# {% include icon.html icon="fa-brands fa-github" %}MBIS-Git

This page keeps the previous MBIS Git resource available from the new website.

{% include section.html %}

{% for item in site.data.activity_resources %}
{% if item.title == "MBIS-Git" %}
{% capture text %}
{{ item.description }}

{% include button.html link=item.link text="Open original page" icon="fa-solid fa-arrow-up-right-from-square" %}
{% endcapture %}

{% include feature.html image="images/hero/hero-lab.jpg" title=item.title text=text link=item.link %}
{% endif %}
{% endfor %}