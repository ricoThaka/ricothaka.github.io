{% for image in site.static_files %}
    {% if image.path contains 'assets/images/worknotes03' %}
        <a href="{{ site.baseurl }}{{ image.path }}" target="_blank">
            <img src="{{ site.baseurl }}{{ image.path }}" alt="" class="img-thumbnail" />
        </a>
    {% endif %}
{% endfor %} 