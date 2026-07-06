---
title: Photo
---

# {% include icon.html icon="fa-solid fa-camera" %}Photo

Lab photos, conference moments, and group activities.

{% include section.html %}

{% for item in site.data.activity_photos %}
{% capture text %}
**{{ item.date }}**  
{{ item.summary }}

{% if item.source %}
[Original post]({{ item.source }})
{% endif %}
{% endcapture %}

{% include feature.html image=item.image title=item.title text=text link=item.source %}

{% endfor %}