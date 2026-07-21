---
title: Award
---

<p class="page-back"><a href="{{ '/blog/' | relative_url }}">← Activity</a></p>

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

<style>
.page-back {
  margin: 24px 0 48px;
  font-size: 1.1rem;
}
.page-back a {
  color: #0098d8;
  text-decoration: underline;
}

/* Award certificates come in mixed portrait/landscape orientations —
   show each at its natural aspect ratio instead of the shared 3:2 crop. */
.feature-image {
  aspect-ratio: auto;
  overflow: visible;
  box-shadow: none;
}

.feature-image img {
  width: 100%;
  height: auto;
  object-fit: contain;
  border-radius: var(--rounded);
  box-shadow: var(--shadow);
}
</style>