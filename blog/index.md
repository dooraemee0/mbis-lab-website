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
Lab news, publications, newcomers, graduation, <br>conference acceptance, and other updates.

{% include button.html link="blog/news" text="View News" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/news/lab_news.png" link="blog/news" title="News" text=text %}

{% capture text %}
Awards and recognitions received by MBIS Lab members.

{% include button.html link="blog/award" text="View Awards" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/award/lab_award.png" link="blog/award" title="Award" text=text flip=true %}

{% capture text %}
Lab photos, conference moments, and group activities.

{% include button.html link="blog/photo" text="View Photos" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/photo/lab_photo.png" link="blog/photo" title="Photo" text=text %}

{% capture text %}
Internal resources including S-sharp reservation and MBIS-Git links.

{% include button.html link="blog/resources" text="Open Resources" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/resource.png" link="blog/resources" title="Internal Resources" text=text flip=true %}

{% capture text %}
AI seminar schedule and topics from MBIS Lab members.

{% include button.html link="blog/ai-seminar" text="View AI Seminars" icon="fa-solid fa-arrow-right" flip=true style="bare" %}
{% endcapture %}
{% include feature.html image="images/blog/ai-seminar/seminar.png" link="blog/ai-seminar" title="AI Seminar" text=text %}

<style>
/* Center-align all text and buttons in the Activity feature sections */
.feature {
  text-align: center;
}

.feature h1,
.feature h2,
.feature h3,
.feature p,
.feature div,
.feature span {
  text-align: center;
}

.feature .button-wrapper,
.feature .button,
.feature a {
  justify-content: center;
  margin-left: auto;
  margin-right: auto;
}

/* Keep feature descriptions readable */
.feature p {
  max-width: 640px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.8;
}

/* Prevent overly wide images from visually spilling out */
.feature img {
  max-width: 100%;
  object-fit: contain;
}
</style>