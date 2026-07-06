---
title: Alumni
---

[{% include icon.html icon="fa-solid fa-arrow-left" %}People](../)

# {% include icon.html icon="fa-solid fa-user-graduate" %}Alumni

{% include section.html %}

<div class="alumni-list">
{% for person in site.data.alumni %}
  <div class="alumni-item">
    {% assign img = person.image | default: "images/fallback.svg" %}
    <img class="alumni-photo" src="{{ img | relative_url }}" alt="{{ person.name }}" loading="lazy">
    <div class="alumni-info">
      <div class="alumni-name">
        {{ person.name }}{% if person.degree %} <span class="alumni-degree">({{ person.degree }})</span>{% endif %}
      </div>
      {% if person.department %}<div class="alumni-dept">{{ person.department }}</div>{% endif %}
      {% if person.current %}<div class="alumni-current">Current: {{ person.current }}</div>{% endif %}
    </div>
  </div>
{% endfor %}
</div>

<style>
  .alumni-list {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .alumni-item {
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 15px;
    background: var(--light-gray, #f5f5f5);
    border-radius: var(--rounded, 8px);
  }
  .alumni-photo {
    width: 90px;
    height: 90px;
    object-fit: cover;
    border-radius: var(--rounded, 8px);
    flex-shrink: 0;
    background: #e0e0e0;
  }
  .alumni-info { flex: 1; }
  .alumni-name {
    font-weight: bold;
    font-size: 1.1rem;
    margin-bottom: 4px;
  }
  .alumni-degree { font-weight: normal; color: var(--gray, #666); }
  .alumni-dept, .alumni-current {
    color: var(--gray, #555);
    font-size: 0.95rem;
    line-height: 1.4;
  }
  @media (max-width: 600px) {
    .alumni-item { flex-direction: column; text-align: center; }
  }
</style>
