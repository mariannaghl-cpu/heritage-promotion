---
layout: default
title: Αναρριχητικά Πεδία (Λίστα)
---

# 🧗‍♂️ Αναρριχητικά Πεδία

{% assign items = site.pois | sort: 'title' %}
<ul>
{% for poi in items %}
  <li><a href="{{ poi.url | relative_url }}">{{ poi.title }}</a></li>
{% endfor %}
</ul>
