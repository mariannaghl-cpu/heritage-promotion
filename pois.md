---
layout: page
title: Αναρριχητικά πεδίο
permalink: /pois/

---

<ul>
  {% for p in site.pois %}
    <li>
      <a href="{{ p.url | relative_url}}">{{ p.title }}</a>
    </li>
  {% endfor %}
</ul>
