---
title: Award
---

# {% include icon.html icon="fa-solid fa-trophy" %}Award

Awards and recognitions received by MBIS Lab members.

{% include section.html %}

{% for item in site.data.activity_awards %}
{% capture text %}
**{{ item.date }}**  
{{ item.summary }}
{% endcapture %}

{% include feature.html image=item.image title=item.title text=text %}

{% endfor %}