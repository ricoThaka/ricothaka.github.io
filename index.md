<div class="swatch">
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div>
  </div>
</div>

{% highlight ruby %}
puts 'Hello, World!'
puts 'HelloWorld'
{% endhighlight %}


<hr />
{% if paginator.total_pages > 1 %}
<div class="pagination">
  {% if paginator.previous_page == 1 %}
  <a href="{{ '/' | prepend: site.baseurl | replace: '//', '/' }}" class="page-item">&laquo;</a>
  {% elsif paginator.previous_page%}
  <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}" class="page-item">&laquo;</a>
  {% else %}
  <span class="page-item">&laquo;</span>
  {% endif %} {% for page in (1..paginator.total_pages) %} {% if page == paginator.page %}
  <span class="page-item">{{ page }}</span>
  {% elsif page == 1 %}
  <a href="{{ '/' | prepend: site.baseurl | replace: '//', '/' }}" class="page-item">{{ page }}</a>
  {% else %}
  <a href="{{ site.paginate_path | prepend: site.baseurl | replace: '//', '/' | replace: ':num', page }}" class="page-item">{{ page }}</a>
  {% endif %} {% endfor %} {% if paginator.next_page %}
  <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}" class="page-item">&raquo;</a>
  {% else %}
  <span class="page-item">&raquo;</span>
  {% endif %}
</div>
{% endif %} {% include footer.html %}

{% if site.google_analytics %}
  {% include analytics.html %}
{% endif %}
---
layout: default
---

<ul>
    {% for post in paginator.posts %}
      <li>
          <h2><a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">{{ post.title }}</a></h2>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
          <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
    {% endfor %}
</ul>
<hr />

<div class="twoPanelSpread" >
    <div class="row">
      <div class="panelColumn">
        <div class="leftColumn">

  <!-- lightbox container hidden with CSS -->
  <a href="#img1">
          <img src="https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/master/assets/images/5247_1_Bright_Gully_Deposits_on_Mars-full2.jpg">
  </a>

  <!-- lightbox container hidden with CSS -->
  <a href="#" class="lightbox" id="img1">
    <span style="background-image: url('https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/master/assets/images/5247_1_Bright_Gully_Deposits_on_Mars-full2.jpg')"></span>
  </a>
          </div>
      </div>
      <div class="panelColumn">
        <div class="rightColumn">
  <a href="#img2">
    <img src="https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/master/assets/images/adobeColor.jpg" alt="Bright Gully Deposits on Mars">
  </a>

  <!-- lightbox container hidden with CSS -->
  <a href="#" class="lightbox" id="img2">
    <span style="background-image: url('https://raw.githubusercontent.com/ricoThaka/ricothaka.github.io/master/assets/images/adobeColor.jpg')"></span>
  </a>
           </div>
      </div>
    </div>
  </div>
{% highlight python %}
  print("# HOLE_TO_ANOTHER_UNiVERSE###Alicia?####Normani?##")
{% endhighlight %}
  <object data="https://murray-lab.caltech.edu/CTX/V01/SceneView/MurrayLabCTXmosaic.html" width="100%" height="400" >
</object>
   <img src="https://apod.nasa.gov/apod/image/2403/PIA19048europa.jpg" alt="Galileo's Europa">
   <p> 

# Explanation:  
<hr />
{% highlight bash %}
#!/bin/bash
#set -x
make_swatches() {
    counter=1
    swatches=''
    input_file=$1
    limit=$2
    template=".swatch div:nth-child(%d){ background: %s; }"
    while read swatch; do
        swatches+="$(printf "$template\n" "$counter" "$swatch")"$'\n'
        ((counter++))
        [[ "$counter" -gt "$limit" ]] && break
    done < "$input_file"
    echo "$swatches"
}

make_swatches colorvalues.csv 8
{% endhighlight %}

Looping through the Jovian system in the late 1990s, the
<a href="https://solarsystem.nasa.gov/galileo/">Galileo spacecraft</a>
recorded stunning views of Europa and uncovered
evidence that the moon's icy surface likely hides
a deep, global ocean.

Galileo's Europa image data has been
<a href="https://photojournal.jpl.nasa.gov/catalog/?IDNumber=PIA19048">
remastered here</a>, with improved calibrations to produce a
color image approximating what the human eye might see.

Europa's long curving fractures
<a href="https://www.nasa.gov/feature/goddard/2019/nasa-scientists-confirm-water-vapor-on-europa">hint at the subsurface liquid water</a>.  

The tidal flexing the large moon experiences
in its elliptical orbit
around Jupiter supplies the energy to keep the ocean liquid.

But more
<a href="ap140919.html">tantalizing</a> is the possibility
that even in the
absence of sunlight that process could also supply the energy to
support life,
<a href="ap160401.html">making Europa</a>
one of the best places to look for life
beyond Earth.

The Juno spacecraft currently in Jovian orbit
has also made repeated flybys of the water world,
returning images along with data exploring
<a href="https://www.nasa.gov/missions/juno/nasas-juno-mission-measures-oxygen-production-at-europa/">Europa's habitability</a>.

This October will see the launch of the NASA's
<a href="https://europa.nasa.gov/">Europa Clipper</a>
on a voyage of
<a href="https://www.youtube.com/watch?v=EgWbeDNPD6o">exploration</a>.

The spacecraft will make nearly 50 flybys,
approaching to within 25 kilometers of Europa's icy surface.

</p>
<img src="https://murray-lab.caltech.edu/Mars2020/img/Jezero-perspective.jpg">
<img src="https://mars.nasa.gov/mars2020-raw-images/pub/ods/surface/sol/00001/ids/edr/browse/edl/EBF_0001_0667022756_679ECV_N0010052EDLC00001_0010LUJ01_1200.jpg" alt="Bright Gully Deposits on Mars">





<img src="https://photojournal.jpl.nasa.gov/jpeg/PIA26202.jpg"  />
<img src="https://photojournal.jpl.nasa.gov/jpeg/PIA26207.jpg" />
<div class="expandingGallery"><img src="https://raw.githubusercontent.com/ricoThaka/saa2/master/assets/images/sartu_rik_equal_ek.png" />
<img src="https://i1.sndcdn.com/artworks-D91rb2LE45DCZq47-cKlxJg-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-yp5s7R5Iq55q-0-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-P2PTj5dAzg6o2EFl-FUqxIw-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-XuEIzk2XtG1w-0-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-3pLwykq3ZwnP-0-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-QwpUDhaNaX8l-0-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-000327590304-xr9ecf-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-c8b32a26-992b-4caf-b624-a35574dee181-0-t500x500.jpg" />
<img src="https://i1.sndcdn.com/artworks-pTTYEez5J7KK-0-t500x500.jpg" />
<img src=" https://i1.sndcdn.com/artworks-000652828381-8tet2w-t500x500.jpg" >
<img src=" https://i1.sndcdn.com/artworks-L3b6Dwse4RJe-0-t500x500.jpg" >
<img src=" https://i1.sndcdn.com/artworks-ikxDwx60XoJJ-0-t500x500.jpg" >
<img src="https://i1.sndcdn.com/artworks-Tz3UrUOI1wzpn6Qm-jwEiJQ-t500x500.jpg" />
</div>






* * *
{% highlight python %}
1 # HOLE_TO_ANOTHER_UNiVERSE##############################
2 # TO####################################################
3 # ANOTHER###############################################
4 # UNiVERSE########################################Megan?
{% endhighlight %}

<div class="swatch">
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>
<div></div>

</div>
<!-- the div section demonstrates that inline stylng from html to color objects nthChildSelectorsWorkBetter here for historical purposes
<div class="swatch">
  <div style="background -color: #8C2034;"></div>
    <div style="background -color: #D9486E;"></div>
    <div style="background -color: #261018;"></div>
    <div style="background -color: #BF7892;"></div>
    <div style="background -color: #D98FB1;">
      </div>
</div>

[SWATCHPANTONE](https://codepen.io/ricoThaka/pen/ZEZrLaX?editors=1100)

{% highlight python %}
1 # HOLE_TO_ANOTHER_UNiVERSE##############################
2 # TO####################################################
3 # ANOTHER###############################################
4 # UNiVERSE########################################Megan?
{% endhighlight %}

---
layout: default
---

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

Text can be **bold**, _italic_, ~~strikethrough~~ or `keyword`.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.


This is a normal paragraph. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.


> This is a blockquote.
>
> When something is important enough, you do it even if the odds are not in your favor.



```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```


| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```


