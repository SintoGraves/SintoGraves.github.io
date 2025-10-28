---
layout: page
title: All Posts
permalink: /posts/
---

{% assign all_posts = site.posts | sort: "date" | reverse %}
{% for post in all_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%B %-d, %Y" }}
{% endfor %}
