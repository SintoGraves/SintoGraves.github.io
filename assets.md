---
layout: page
title: Media Library
permalink: /media/
---

# Media Library

Welcome to the visual reference section of *Reason Over Rhetoric*.  
Below are the images, tables, and charts used throughout current and upcoming op-eds.

---

## Protest Reference Table (Featured)

<figure class="table-figure">
  <img src="{{ '/assets/images/Protests.png' | relative_url }}"
       alt="Protests and Congressional Response Table"
       style="max-width:100%;height:auto;">
  <figcaption>
  Featured reference table for the two-part series:
  <a href="{{ '/when-congress-forgets-who-it-serves/' | relative_url }}">Part 1</a> ·
  <a href="{{ '/when-the-people-vote-congress-gets-the-message/' | relative_url }}">Part 2</a> ·
  <a href="{{ '/assets/images/Protests.png' | relative_url }}"
   download="Protests.png"
   target="_blank"
   rel="noopener noreferrer">Download PNG</a>

</figcaption>
</figure>

---

## Image Archive

<div style="display:flex;flex-wrap:wrap;gap:1rem;">
  {% assign imgs = site.static_files | where_exp: "file", "file.path contains '/assets/images/'" %}
  {% for img in imgs %}
    <div style="flex:1 0 240px;text-align:center;">
      <a href="{{ img.path | relative_url }}" target="_blank" rel="noopener">
        <img src="{{ img.path | relative_url }}" alt="{{ img.name }}"
             style="max-width:100%;height:auto;border:1px solid #ccc;padding:4px;border-radius:8px;">
      </a>
      <div style="font-size:0.9rem;color:#666;margin-top:0.25rem;">{{ img.name }}</div>
    </div>
  {% endfor %}
</div>
