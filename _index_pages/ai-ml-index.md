---
layout: single
author_profile: true
title: AI/ML
---
<hr>



  <hr>
  
<ul>
{% assign sorted_ghazal = site.ai | sort: 'date' | reverse %}
{% for item in sorted_ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span style='color:gray'> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  <hr>
  {% endfor %}
</ul>


<hr>
<a href="https://bukharifaraz.github.io/rl-index/">RL Course Notes</a>
