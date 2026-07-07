---
title: Internal Resources
---

<p class="page-back"><a href="{{ '/blog/' | relative_url }}">← Activity</a></p>

# {% include icon.html icon="fa-solid fa-folder-open" %}Internal Resources

Internal resources for MBIS Lab members.

{% include section.html %}

<div class="resource-grid">

  <div class="resource-card">
    <div class="resource-image-wrap">
      <img src="{{ '/images/blog/s-sharp-reservation.jpg' | relative_url }}" alt="S-sharp reservation">
    </div>

    <div class="resource-content">
      <h2>S-sharp reservation</h2>
      <p>
        Use the S-sharp reservation page to check the current reservation status and reserve the shared S-sharp system.
      </p>

      <a class="resource-button" href="https://moonhwanlee.notion.site/S-sharp-reservation-2d557e39ed9880b8bd6ed8e4cfc4086d" target="_blank" rel="noopener">
        예약하기
        <span>↗</span>
      </a>
    </div>
  </div>

  <div class="resource-card">
    <div class="resource-image-wrap">
      <img src="{{ '/images/blog/mbis-git.jpg' | relative_url }}" alt="MBIS-Git">
    </div>

    <div class="resource-content">
      <h2>MBIS-Git</h2>
      <p>
        Access MBIS Lab repositories, shared project codes, and collaborative development resources through the MBIS-Git organization.
      </p>

      <a class="resource-button" href="https://github.com/MBIS-Git" target="_blank" rel="noopener">
        Open MBIS-Git
        <span>↗</span>
      </a>
    </div>
  </div>

</div>

<style>
.page-back {
  margin: 24px 0 48px;
  font-size: 1.1rem;
}
.page-back a {
  color: #0098d8;
  text-decoration: underline;
}

.resource-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 36px;
  margin: 48px auto 0;
  max-width: 1100px;
}

.resource-card {
  background: #ffffff;
  border-radius: 18px;
  box-shadow: 0 12px 36px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  border: 1px solid rgba(0, 0, 0, 0.06);
}

.resource-image-wrap {
  width: 100%;
  background: #f7f9fc;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 18px;
}

.resource-image-wrap img {
  width: 100%;
  height: 560px;
  object-fit: contain;
  display: block;
  border-radius: 12px;
}

.resource-content {
  padding: 28px 30px 34px;
  text-align: center;
}

.resource-content h2 {
  margin: 0 0 16px;
  font-size: 1.45rem;
  font-weight: 700;
}

.resource-content p {
  margin: 0 auto 26px;
  line-height: 1.75;
  color: #333;
  max-width: 430px;
}

.resource-button {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 12px 22px;
  border-radius: 8px;
  background: #0098d8;
  color: #ffffff !important;
  text-decoration: none;
  font-weight: 700;
  transition: transform 0.15s ease, box-shadow 0.15s ease, background 0.15s ease;
}

.resource-button:hover {
  background: #007fba;
  transform: translateY(-1px);
  box-shadow: 0 8px 18px rgba(0, 152, 216, 0.25);
}

@media (max-width: 900px) {
  .resource-grid {
    grid-template-columns: 1fr;
  }

  .resource-image-wrap img {
    height: 480px;
  }
}
</style>