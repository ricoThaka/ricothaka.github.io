
![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0001.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0002.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0003.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0004.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0005.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0006.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0007.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0008.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0009.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0014.png)

![Advanced Unix Programming](https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/pixelsquare/assets/images/worknotes03/files0015.png)





```
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
```