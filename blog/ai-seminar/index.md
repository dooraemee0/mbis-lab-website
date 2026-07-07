---
title: AI Seminar
---

<p class="page-back"><a href="{{ '/blog/' | relative_url }}">← Activity</a></p>

# {% include icon.html icon="fa-solid fa-brain" %}AI Seminar

AI seminar schedule and topics from MBIS Lab members.

{% include section.html %}

{% for item in site.data.activity_ai_seminars %}
{% capture text %}
**{{ item.date }}**  
{{ item.summary }}
{% endcapture %}

{% include feature.html image=item.image title=item.title text=text %}

{% endfor %}

<style>
.page-back {
  margin: 24px 0 48px;
  font-size: 1.1rem;
}
.page-back a {
  color: #0098d8;
  text-decoration: underline;
}
</style>