---
layout: page
title: Αναρριχητικά πεδία
permalink: /pois/
---

<div style="display: flex; align-items: flex-start; gap: 2rem;">

  <!-- ΛΙΣΤΑ ΜΕ ΤΑ ΠΕΔΙΑ -->
  <ul style="flex: 1;">
    {% for p in site.pois %}
      <li style="margin-bottom: 0.5rem;">
        <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <!-- ΕΙΚΟΝΑ ΔΕΞΙΑ -->
  <img src="{{ '/assets/img4/Doukades1.jpg' | relative_url }}" 
       alt="Αναρριχητικό πεδίο Δουκάδες" 
       style="width: 40%; border-radius: 12px; box-shadow: 0 2px 10px rgba(0,0,0,0.2);" />
</div>
