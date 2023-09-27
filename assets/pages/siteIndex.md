--- 
layout: page
title: Index
---
<!-- use site.collections to try to separate pages by subfolder -->
<ul>
  {% for item in site.pages %}
    <li {% if page.url contains item.path %}class="active"{% endif %}><a href="https://didsr.github.io/HTT.home{{ item.url }}">{{ item.title }}</a></li>
  {% endfor %}
</ul>

<!-- https://carpentries-incubator.github.io/jekyll-pages-novice/arrays/index.html -->