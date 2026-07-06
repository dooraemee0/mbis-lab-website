---
title: AI Seminar
---

# {% include icon.html icon="fa-solid fa-chalkboard-user" %}AI Seminar

AI seminar records and topics from MBIS Lab members.

{% include section.html %}

{% for item in site.data.activity_ai_seminars %}
{% capture text %}
**{{ item.date }}**  
**Speaker:** {{ item.speaker }}  
**Topic:** {{ item.topic }}

{{ item.summary }}

{% if item.source %}
[Original post]({{ item.source }})
{% endif %}
{% endcapture %}

{% include feature.html image=item.image title=item.title text=text link=item.source %}

{% endfor %}