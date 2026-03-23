---
layout: home
title: Home
---

<style>
  body { background-color: #0d1117 !important; color: #c9d1d9 !important; font-family: 'Georgia', serif !important; }
  
  /* Branding Header Styling */
  .brand-header { 
    display: flex; 
    justify-content: space-between; 
    align-items: center; 
    margin-bottom: 30px; 
    padding: 20px 0;
    border-bottom: 1px solid #30363d;
  }
  .site-logo { 
    height: 80px; 
    width: auto; 
    /* This ensures visibility and a professional "glow" */
    filter: drop-shadow(0px 0px 8px rgba(198, 160, 82, 0.4)); 
  }
  .status-intel { text-align: right; color: #c6a052; font-family: monospace; font-size: 0.75rem; line-height: 1.4; }

  /* Insights & Footer Styles */
  .insight-card { margin-bottom: 20px; border-left: 4px solid #c6a052; padding: 15px 20px; background: #161b22; transition: 0.3s; }
  .insight-card:hover { border-left: 4px solid #fff; background: #1c2128; }
  .badge { font-size: 0.7rem; color: #c6a052; font-family: monospace; border: 1px solid #c6a052; padding: 2px 6px; text-transform: uppercase; border-radius: 2px; display: inline-block; margin-bottom: 8px; }
  .spec-footer { margin-top: 60px; padding: 30px 0; border-top: 1px solid #30363d; background: #0d1117; }
  .spec-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 20px; margin-top: 20px; }
  .spec-box { font-size: 0.85rem; color: #8b949e; line-height: 1.5; }
  .spec-box strong { color: #c6a052; display: block; margin-bottom: 8px; text-transform: uppercase; letter-spacing: 1px; }
</style>

<div class="brand-header">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Kadiaman Strategic Logo" class="site-logo">
  
  <div class="status-intel">
    LOCATION: JAKARTA // 106.8456° E<br>
    STATUS: OPERATIONAL<br>
    INTEL: UNRESTRICTED ACCESS
  </div>
</div>

# Law as a Strategic Asset

In a fragmented global landscape, law is not a mere administrative procedure; it is an instrument of sovereignty and an extension of strategic power. 

---

### Latest Strategic & Academic Insights

{% for post in site.posts limit:5 %}
  <div class="insight-card">
    <div class="badge">
      {% if post.categories contains 'Academic-Journal' %}PEER-REVIEWED{% else %}STRATEGIC BRIEF{% endif %}
    </div>
    <span style="font-size: 0.8rem; color: #8b949e; font-family: monospace; margin-left: 10px;">{{ post.date | date: "%Y-%m-%d" }}</span><br>
    <a href="{{ post.url | relative_url }}" style="font-weight: bold; font-size: 1.25rem; text-decoration: none; display: block; margin-top: 5px;">{{ post.title }}</a>
    <p style="font-size: 0.9rem; margin-top: 5px; color: #c9d1d9;">{{ post.excerpt | strip_html | truncatewords: 22 }}</p>
  </div>
{% endfor %}

<div style="text-align: center; margin-top: 20px;">
  [**Access Full Intelligence Archive →**]({{ '/archive/' | relative_url }})
</div>

---

<div class="spec-footer">
  <h5 style="color: #fff; text-align: center; margin-bottom: 25px;">CORE STRATEGIC SPECIALIZATIONS</h5>
  <div class="spec-grid">
    <div class="spec-box">
      <strong>Geopolitical Risk</strong>
      Mapping global power shifts and their impact on regional stability and trade routes.
    </div>
    <div class="spec-box">
      <strong>Military Law (LOAC)</strong>
      Expertise in the Law of Armed Conflict and International Humanitarian Law (IHL).
    </div>
    <div class="spec-box">
      <strong>Rule of Law</strong>
      Navigating Indonesia’s modern legal reform and institutional resilience frameworks.
    </div>
  </div>
</div>
