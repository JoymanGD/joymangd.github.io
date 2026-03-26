---
layout: default
title: "Math"
---

{% assign posts = site.posts | where_exp: "post", "post.categories contains 'math'" %}
{% if posts and posts.size > 0 %}
{% for post in posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% else %}
<p>No posts yet.</p>
{% endif %}
