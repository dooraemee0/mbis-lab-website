---
title: Member
---

[{% include icon.html icon="fa-solid fa-arrow-left" %}People](../)

# {% include icon.html icon="fa-solid fa-user-group" %}Member

## Researchers

<div class="researchers-grid" markdown="1">
{% include list.html data="members" component="portrait" filter="group == 'postdoc'" %}
</div>

{% include section.html %}

## Ph.D. Students

{% include list.html data="members" component="portrait" filter="group == 'phd'" %}

{% include section.html %}

## M.S. Students

{% include list.html data="members" component="portrait" filter="group == 'ms'" %}

{% assign undergrads = site.members | where: "group", "undergraduate" %}
{% if undergrads.size > 0 %}
{% include section.html %}

## Undergraduate

{% include list.html data="members" component="portrait" filter="group == 'undergraduate'" %}
{% endif %}

{% include section.html %}

## {% include icon.html icon="fa-solid fa-bullhorn" %}Join Us!

**(Ph.D. or M.S. student + undergraduate research opportunities)**

A number of exciting research projects are available in our laboratory for
motivated students. Those interested in our group may stop by the lab or email
Prof. Jae Youn Hwang at [jyhwang@dgist.ac.kr](mailto:jyhwang@dgist.ac.kr).

<!-- TODO: optionally add a "WANTED" image here, e.g. images/people/wanted.png -->
