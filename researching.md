---
layout: page
title: "Researching"
---

{% assign posts = site.categories.researching %}
{% if posts and posts.size > 0 %}
{% for post in posts %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
{% endfor %}
{% else %}
<p>No posts yet.</p>
{% endif %}
