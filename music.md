---
layout: page
title: "Music"
---

{% assign posts = site.categories.music %}
{% if posts and posts.size > 0 %}
{% for post in posts %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
{% endfor %}
{% else %}
<p>No posts yet.</p>
{% endif %}
