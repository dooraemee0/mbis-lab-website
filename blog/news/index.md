---
title: News
---

# {% include icon.html icon="fa-solid fa-newspaper" %}News

Lab news, publications, newcomers, graduation, conference acceptance, and other updates from MBIS Lab.

{% include section.html %}

{% for item in site.data.activity_news %}
{% capture text %}
**{{ item.date }}**  
{{ item.summary }}
{% endcapture %}

{% include feature.html image=item.image title=item.title text=text %}

{% endfor %}