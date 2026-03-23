---
layout: page
title: Strategic Intelligence Archive
permalink: /archive/
---

# Archive of Strategic Insights

Below is a curated list of analyses regarding Geopolitical Risk, Military Law, and Institutional Power.

<ul>
  {% for post in site.posts %}
    <li>
      <span style="font-family: monospace; color: #8b949e;">{{ post.date | date: "%Y-%m-%d" }}</span> &raquo; 
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

---
*For restricted briefings, please contact coordination.*
