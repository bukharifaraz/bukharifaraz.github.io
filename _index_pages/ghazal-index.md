---
layout: single
title: Ghazal Collection
---
<div style='text-align:center'>
<p>
اک شاعر ہے اچھا بخاری فراز<br>
  ہے خیال آپکا ہَم نہیں مانتے<br>
</p>




<p>
As a poet "Bukhari Faraz" is remarkable ! <br>
It's (merely) your opinion, I don't agree !<br>
</p>
<p stlye='font:20px'>
Read full <a href='https://bukharifaraz.github.io/ghazal/dekha-suna-ham-nahin-maante/'>here</a>..
</p>

  </div>
  
<ol>
  {% for item in site.ghazal %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      <span style='color:gray'> - {{ item.date | date: "%B %d, %Y" }}</span>
    </li>
  <hr>
  {% endfor %}
</ol>







