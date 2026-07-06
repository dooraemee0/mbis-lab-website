---
title: Blog
nav:
  order: 6
  tooltip: Lab activity
---

# {% include icon.html icon="fa-solid fa-calendar-days" %}Activity

News, awards, photos, internal resources, and AI seminar records from MBIS Lab.

{% include section.html %}

{% capture text %}
Lab news, publications, newcomers, graduation, conference acceptance, and other updates.

{% include button.html link="blog/news" text="View News" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/news/miccai-2026.jpg" link="blog/news" title="News" text=text %}

{% capture text %}
Awards and recognitions received by MBIS Lab members.

{% include button.html link="blog/award" text="View Awards" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/award/sehyun-award-ic-ueba-2025.png" link="blog/award" title="Award" text=text flip=true %}

{% capture text %}
Lab photos, conference moments, and group activities.

{% include button.html link="blog/photo" text="View Photos" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/photo/kosombe-2016.png" link="blog/photo" title="Photo" text=text %}

{% capture text %}
Internal resources including S-sharp reservation and MBIS-Git links.

{% include button.html link="blog/s-sharp-reservation" text="Open Resources" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/hero/hero-lab.jpg" link="blog/s-sharp-reservation" title="Internal Resources" text=text flip=true %}

{% capture text %}
AI seminar schedule and topics from MBIS Lab members.

{% include button.html link="blog/ai-seminar" text="View AI Seminars" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/ai-seminar/priyanka-2025-07-15.jpg" link="blog/ai-seminar" title="AI Seminar" text=text %}