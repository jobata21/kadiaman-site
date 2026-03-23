---
layout: page
title: Strategic Intelligence Archive
permalink: /archive/
---

# Publication History
*Complete list of journals, articles, and strategic assessments.*

---

{% for post in site.posts %}
  <div style="border-bottom: 1px solid #30363d; padding: 20px 0;">
    <span style="color: #c6a052; font-family: monospace;">[{{ post.date | date: "%Y-%m-%d" }}]</span>
    <a href="{{ post.url }}" style="font-size: 1.4rem; font-weight: bold; display: block; margin-top: 5px;">{{ post.title }}</a>
  </div>
{% endfor %}

---
[Return to Home (Command Center)](/)
