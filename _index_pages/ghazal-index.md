---
layout: single
title: Ghazal Collection
---

<ol>
  {% for item in site.ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  <hr>
  {% endfor %}
</ol>







