---
title: S-sharp reservation
---

# {% include icon.html icon="fa-solid fa-calendar-check" %}S-sharp reservation

This page keeps the previous MBIS internal reservation resource available from the new website.

{% include section.html %}

{% for item in site.data.activity_resources %}
{% if item.title == "S-sharp reservation" %}
{% capture text %}
{{ item.description }}

{% include button.html link=item.link text="Open original page" icon="fa-solid fa-arrow-up-right-from-square" %}
{% endcapture %}

{% include feature.html image="images/hero/hero-lab.jpg" title=item.title text=text link=item.link %}
{% endif %}
{% endfor %}