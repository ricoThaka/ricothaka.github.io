<MAIN>



<SECTION>

<div class="tupperware">
{% for post in site.posts %}
    
<ARTICLE itemprop="blogPosts" itemscope itemtype="https://schema.org/BlogPosting" >
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2 itemprop="headline"><span>{{ post.title }}</span></h2>
    </div>
  </a>
</ARTICLE>

{% endfor %}
</div>



</SECTiON>
</MAIN>