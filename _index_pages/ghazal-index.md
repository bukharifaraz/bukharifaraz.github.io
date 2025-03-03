---
layout: single
author_profile: true
title: Ghazal Collection
---
<hr>
<div style='text-align:center'>
<p style=" font-family: 'Traditional Arabic', 'Diwan Thuluth', serif; font-size: 28px; color: gold; text-align: center; direction: rtl; text-shadow: 1px 1px 0 #b8860b, /* Dark gold shadow */ -1px -1px 0 #b8860b, 2px 2px 4px #ffd700; /* Outer glow effect */ -webkit-text-stroke: 1px #b8860b; /* Gold border */ ">
اک شاعر ہے اچھا بخاری فراز<br>
  ہے خیال آپکا ہَم نہیں مانتے<br>
</p>




<p>
As a poet "Bukhari Faraz" is remarkable ! <br>
It's your opinion, (which) I don't agree (with) !<br>
</p>
<p stlye='font:20px'>
Read full <a href='https://bukharifaraz.github.io/ghazal/dekha-suna-ham-nahin-maante/'>here</a>..
</p>
  </div>
  <hr>
  
<ol>
{% assign sorted_ghazal = site.ghazal | sort: 'date' | reverse %}
{% for item in sorted_ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span style='color:gray'> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  <hr>
  {% endfor %}
</ol>







