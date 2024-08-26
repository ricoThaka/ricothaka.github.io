

{% for i in (1..18) %}
 {% if image.path contains 'assets/images/worknotes03' %}
<img src="{{ site.baseurl }}{{ image.path }}"><br>
{% endif %}
{% endfor %}

{% for image in site.static_files %}
    {% if image.path contains 'assets/images/worknotes03' %}
        <a href="{{ site.baseurl }}{{ image.path }}" target="_blank">
            <img src="{{ site.baseurl }}{{ image.path }}" alt="" class="img-thumbnail" />
        </a>
    {% endif %}
{% endfor %} 