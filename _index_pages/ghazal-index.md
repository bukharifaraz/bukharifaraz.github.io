---
layout: single
title: "My Ghazal(s)"
---

<ul>
  {% for post in site.posts %}
    {% if post.tags contains "ghazal" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span> - {{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Ghazal Collection</h1>

<ul>
  {% for item in site.ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>







