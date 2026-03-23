---
layout: home
title: Home
---

<style>
  /* Force Dark Theme */
  body { background-color: #0d1117 !important; color: #c9d1d9 !important; font-family: 'Georgia', serif !important; margin: 0; padding: 0; }
  .site-header { background-color: #161b22 !important; border-bottom: 2px solid #c6a052 !important; border-top: 4px solid #c6a052 !important; }
  .site-title, .site-nav { color: #c6a052 !important; text-transform: uppercase !important; letter-spacing: 2px !important; }
  
  /* Logo & Header Alignment */
  .brand-header { 
    display: flex; 
    justify-content: space-between; 
    align-items: center; 
    padding: 20px 0;
    margin-bottom: 30px;
    border-bottom: 1px solid #30363d;
  }
  
  /* THE FIX: Controlled Logo Size */
  .site-logo { 
    height: 60px; /* Reduced size for better proportion */
    width: auto; 
    filter: drop-shadow(0px 0px 5px rgba(198, 160, 82, 0.3)); 
  }

  .status-intel { text-align: right; color: #c6a052; font-family: monospace; font-size: 0.7rem; line-height: 1.2; }

  /* Insights List */
  .insight-card { margin-bottom: 20px; border-left: 4px solid #c6a052; padding: 15px 20px; background: #161b22; transition: 0.3s; }
  .badge { font-size: 0.7rem; color: #c6a052; font-family: monospace; border: 1px solid #c6a052; padding: 2px 6px; text-transform: uppercase; border-radius: 2px; display: inline-block; margin-bottom: 8px; }
  
  /* Footer Specializations */
  .spec-footer { margin-top: 60px; padding: 30px 0; border-top: 1px solid #30363d; background: #0d1117; }
  .spec-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 20px; margin-top: 20px; }
  .spec-box { font-size: 0.8rem; color: #8b949e; }
  .spec-box strong { color: #c6a052; display: block; margin-bottom: 5px; text-transform: uppercase; }
</style>

<div class="brand-header">
  <img src="/assets/images/logo.png" alt="Kadiaman Logo" class="site-logo">
  
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
    <a href="{{ post.url | relative_url }}" style="font-weight: bold; font-size: 1.2rem; text-decoration: none; display: block; margin-top: 5px;">{{ post.title }}</a>
  </div>
{% endfor %}

<div style="text-align: center; margin-top: 20px;">
  [**Access Full Intelligence Archive →**]({{ '/archive/' | relative_url }})
</div>

<div class="spec-footer">
  <div class="spec-grid">
    <div class="spec-box"><strong>Geopolitical Risk</strong>Mapping global power shifts and regional stability.</div>
    <div class="spec-box"><strong>Military Law (LOAC)</strong>Expertise in International Humanitarian Law.</div>
    <div class="spec-box"><strong>Rule of Law</strong>Navigating Indonesia’s modern legal reform.</div>
  </div>
</div>
