---
title: People
nav:
  order: 4
  tooltip: Professor, members, and alumni
---

# {% include icon.html icon="fa-solid fa-users" %}People

MBIS Lab is composed of researchers and students working together on biomedical
imaging, signal processing, artificial intelligence, and healthcare system research.

{% include section.html %}

{% capture professor %}
### {% include icon.html icon="fa-solid fa-user-tie" %}[Professor]({{ "/members/professor" | relative_url }})

Meet our principal investigator.
{% endcapture %}

{% capture member %}
### {% include icon.html icon="fa-solid fa-user-group" %}[Member](member)

Current researchers and students.
{% endcapture %}

{% capture alumni %}
### {% include icon.html icon="fa-solid fa-user-graduate" %}[Alumni](alumni)

Former members of the lab.
{% endcapture %}

{% include cols.html col1=professor col2=member col3=alumni %}