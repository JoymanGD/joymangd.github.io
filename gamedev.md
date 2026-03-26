---
layout: default
title: "GameDev"
---

{% assign posts = site.posts | where_exp: "post", "post.categories contains 'gamedev'" %}
{% if posts and posts.size > 0 %}
{% for post in posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% else %}
<p>No posts yet.</p>
{% endif %}
