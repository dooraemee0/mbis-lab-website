---
title: ACTIVITY
nav:
  order: 5
  tooltip: Lab news, awards, and activities
---

# {% include icon.html icon="fa-solid fa-bullhorn" %}Activity

News, awards, and activities from MBIS Lab.

{% include section.html %}

{% capture news %}
### {% include icon.html icon="fa-solid fa-newspaper" %}[News](news)

Latest news and announcements from the lab.
{% endcapture %}

{% capture award %}
### {% include icon.html icon="fa-solid fa-trophy" %}[Award](award)

Awards and honors received by lab members.
{% endcapture %}

{% include cols.html col1=news col2=award %}

{% capture photo %}
### {% include icon.html icon="fa-solid fa-images" %}[Photo](photo)

Photos from lab events and gatherings.
{% endcapture %}

{% capture ssharp %}
### {% include icon.html icon="fa-solid fa-calendar-check" %}[S-sharp reservation](s-sharp-reservation)

S-sharp equipment reservation and schedule.
{% endcapture %}

{% include cols.html col1=photo col2=ssharp %}

{% capture git %}
### {% include icon.html icon="fa-brands fa-git-alt" %}[MBIS-Git](mbis-git)

Lab code repositories and Git resources.
{% endcapture %}

{% capture seminar %}
### {% include icon.html icon="fa-solid fa-chalkboard-user" %}[AI seminar](ai-seminar)

AI seminar schedule and materials.
{% endcapture %}

{% include cols.html col1=git col2=seminar %}
