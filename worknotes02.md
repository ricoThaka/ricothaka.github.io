

{% for i in (1..18) %}
<img src="assets/images/worknotes03/{{ i }}.png"><br>
{% endfor %}

{% for image in site.static_files %}
    {% if image.path contains 'assets/images/worknotes03' %}
        <a href="{{ site.baseurl }}{{ image.path }}" target="_blank">
            <img src="{{ site.baseurl }}{{ image.path }}" alt="" class="img-thumbnail" />
        </a>
    {% endif %}
{% endfor %} 