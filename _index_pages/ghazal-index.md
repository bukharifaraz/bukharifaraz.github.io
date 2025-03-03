---
layout: single
author_profile: true
title: Ghazal Collection
---
<hr>
<div style='text-align:center'>
<p style="
  font-family: 'Amiri', 'Lateef', 'Scheherazade', serif; /* Arabic calligraphy-friendly fonts */
  font-size: 1rem; /* Adjust size as needed */
  color: #D4AF37; /* Golden color */
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Adds depth to the text */
  background: linear-gradient(to right, #D4AF37, #FFD700); /* Gradient for a golden effect */
  -webkit-background-clip: text; /* Clips the background to the text */
  -webkit-text-fill-color: transparent; /* Makes the text transparent to show the gradient */
  text-align: center; /* Centers the text */
  line-height: 1.6; /* Improves readability */
">

ایک شاعر ہے اچھا بخاری فراز<br>
  ہے خیال آپکا ہَم نہیں مانتے<br>
</p>




<p style="color:gray">
  <i>
    As a poet "Bukhari Faraz" is remarkable ! <br>
It's your opinion, (which) I don't agree (with) !<br>
  </i>

</p>
<p stlye='font:20px'>
Read full <a href='https://bukharifaraz.github.io/ghazal/dekha-suna-ham-nahin-maante/'>here</a>..
</p>
  </div>
  <hr>
  
<ul>
{% assign sorted_ghazal = site.ghazal | sort: 'date' | reverse %}
{% for item in sorted_ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span style='color:gray'> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  <hr>
  {% endfor %}
</ul>







