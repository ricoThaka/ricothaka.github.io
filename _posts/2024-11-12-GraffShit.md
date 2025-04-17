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


{% include graffiti.md %}

# Black On Both Sides
by Mos Def
<iframe src="https://archive.org/embed/mos-def-black-on-both-sides" width="500" height="60" frameborder="0" webkitallowfullscreen="true" mozallowfullscreen="true" allowfullscreen></iframe>