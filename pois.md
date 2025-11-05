---
layout: page
title: Αναρριχητικά πεδία
permalink: /pois/
---

<style>
  .pois-wrap {
    display: grid;
    grid-template-columns: 1fr 400px;
    gap: 2rem;
    align-items: start;
  }
  .pois-card {
    border-radius: 14px;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
    overflow: hidden;
  }
  .pois-card img {
    width: 100%;
    height: auto;
    display: block;
    object-fit: cover;
    transition: transform 0.3s ease;
  }
  .pois-card img:hover {
    transform: scale(1.05);
  }
  .pois-cap {
    padding: 0.6rem 0.9rem;
    font-weight: 600;
    text-align: center;
  }
  @media (max-width: 820px) {
    .pois-wrap {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="pois-wrap">
  <!-- ΛΙΣΤΑ -->
  <ul>
    {% for p in site.pois %}
      <li style="margin-bottom: .5rem;">
        <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <!-- ΕΙΚΟΝΑ ΔΕΞΙΑ -->
  <figure class="pois-card">
    <img
      src="{{ '/assets/img/Doukades1.jpg' | relative_url }}"
      alt="Αναρριχητικό πεδίο Δουκάδες"
      loading="lazy">
    <figcaption class="pois-cap">Αναρριχητικό πεδίο Δουκάδες</figcaption>
  </figure>
</div>
