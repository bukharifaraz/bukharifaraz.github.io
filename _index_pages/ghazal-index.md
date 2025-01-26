---
layout: single
title: "My Ghazal(s)"
---
<h1>Posts Tagged with "Ghazal"</h1>

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







