---
layout: default
title: Building Standards
---
<ul>
  {% for standards in site.building_standards %}
    <li>
      <a href="{{ standards.url }}">{{ standards.title }}</a>
    </li>
  {% endfor %}
</ul>