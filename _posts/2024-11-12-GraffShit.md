---
layout: post
title:  "GraffShit"
date:   2024-11-12 22:51:06 -0800
categories: art graffiti coral
published: true
image: tumblr_9ab057dfcb5ba2d5a76b3b6287774817_4b2ec709_500.webp
---

{% assign posts = site.posts | where_exp: "post", "post.categories contains 'coral'" %}
{% for post in posts %}
  <li>{{ post.title }}</li>
{% endfor %}

[Preserving New York's History of Graffiti Art](https://time.com/4743207/martha-cooper-subway-graffiti/)
{% include graffiti.md %}