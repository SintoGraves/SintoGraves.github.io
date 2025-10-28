---
layout: page
title: Reason Over Rhetoric
---

Welcome to **Reason Over Rhetoric** — weekly op-eds by Sinto Gra'Ves.

---

### Author’s Statement

*Reason Over Rhetoric* is a forum for disciplined thinking in a noisy democracy.  Each op-ed challenges readers, and those in power,
to weigh words against duty, and ambition against the oath they swore.  Rather than echo partisan talking points, these essays trace the 
Constitution’s intent and the responsibilities it places on those who serve under it.

This project exists to rekindle civic reasoning: to remind citizens that loyalty to the Republic begins with loyalty to truth.  Whether addressing Congress’s inertia, executive overreach, or the erosion of public trust, every piece follows a single rule — **think first, speak second.**    By reviving reflection, *Reason Over Rhetoric* seeks to make debate once again a public service, not a performance.
   
---

### Latest Series
{%- assign overviews = site.posts | where: "series_overview", true | sort: "date" | reverse -%}
{%- if overviews.size > 0 -%}
{%- for post in overviews limit:10 -%}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%B %-d, %Y" }}
  {%- if post.description %}<br>{{ post.description }}{%- endif %}
{%- endfor -%}
{%- else -%}
_No series overview posts yet._
{%- endif -%}



