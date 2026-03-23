---
layout: home
title: Home
---

<style>
  body { background-color: #0d1117 !important; color: #c9d1d9 !important; font-family: 'Georgia', serif !important; }
  .site-header { background-color: #161b22 !important; border-bottom: 2px solid #c6a052 !important; border-top: 4px solid #c6a052 !important; }
  .site-title, .site-nav { color: #c6a052 !important; text-transform: uppercase !important; letter-spacing: 2px !important; }
  .wrapper { max-width: 800px !important; }
  a { color: #c6a052 !important; text-decoration: underline !important; }
  .contact-box { border: 1px solid #30363d; padding: 20px; background: #161b22; margin-top: 40px; border-left: 4px solid #c6a052; }
</style>

<div style="text-align: right; color: #c6a052; font-family: monospace; font-size: 0.8rem;">
  CLASSIFICATION: STRATEGIC INTEL // UNRESTRICTED ACCESS
</div>

# Law as a Strategic Asset

In a fragmented global landscape, law is not a mere administrative procedure; it is an instrument of sovereignty and an extension of strategic power. 

**Kadiaman Strategic Advisor** provides deep-dive analysis at the intersection of Military Law (LOAC/IHL), Geopolitical Risk, and Institutional Resilience.

### Core Strategic Pillars

* **Sovereignty & Defense:** Navigating the Law of Armed Conflict (LOAC).
* **Institutional Power Dynamics:** Structural forces and legal frameworks.
* **Strategic Governance:** Systems designed to withstand geopolitical volatility.

---

### Latest Strategic Insights

{% for post in site.posts limit:3 %}
  <div style="margin-bottom: 20px; border-left: 4px solid #c6a052; padding: 10px 20px; background: #161b22;">
    <span style="font-size: 0.8rem; color: #8b949e; font-family: monospace;">PUBLISHED: {{ post.date | date: "%Y-%m-%d" }}</span><br>
    <a href="{{ post.url }}" style="font-weight: bold; font-size: 1.2rem; text-decoration: none;">{{ post.title }}</a>
    <p style="font-size: 0.9rem; margin-top: 5px; color: #c9d1d9;">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
  </div>
{% endfor %}

<br>
[**Access Full Intelligence Archive →**](/archive/)

---

<div class="contact-box">
  <h4 style="color: #c6a052; margin-top: 0;">STRATEGIC COMMUNICATION</h4>
  <p style="margin-bottom: 5px;">Direct Line: <strong><a href="tel:+6287875618777" style="color: #fff !important;">+62 878 7561 8777</a></strong></p>
  <p style="font-size: 0.85rem; color: #8b949e;"><em>Available for tactical briefing and legal-strategic consultation.</em></p>
</div>
