---
layout: page-fullwidth
subheadline: "Interview Archive"
title: "Interviews with Netlabels and Netaudio Activists"
teaser: "This is a loose collection of interviews and portraits of netlabels and netaudio artists and activists."
header:
    image_fullwidth: "blog/header_unsplash_8.jpg"
permalink: "/interviews/"
---
{% include alert info='If you want to contribute to our archive, please <a href="http://netlabels.org/contact/">CONTACT US</a>. We are interested in scans, flyers, portraits. In every language.' %}



## DEUTSCH: Interviews und Portraits



<div class="row">
<div class="medium-6 columns" markdown="1">

### Netlabel Interviews

<ul class="side-nav">
  {% for interview in site.interviews %}
    {% unless interview.published == false %}
        {% if interview.language == 'de' %}
        {% if interview.subheadline contains 'Netlabel' %}
            <li><a href="{{ site.url }}{{ interview.url }}">{{ interview.title }}</a></li>
        {% endif %}
        {% endif %}
    {% endunless %}
  {% endfor %}
  <li>&nbsp;</li>
</ul>


</div><!-- /.medium-6.columns -->
<div class="medium-6 columns" markdown="1">


### Netaudio Interviews

<ul class="side-nav">
  {% for interview in site.interviews %}
    {% unless interview.published == false %}
        {% if interview.language == 'de' %}
        {% unless interview.subheadline contains 'Netlabel' %}
            <li><a href="{{ site.url }}{{ interview.url }}"><span class="subheader">{{ interview.subheadline }}</span> »{{ interview.title }}«</a></li>
        {% endunless %}
        {% endif %}
    {% endunless %}
  {% endfor %}
  <li>&nbsp;</li>
</ul>


</div><!-- /.medium-6.columns -->
</div><!-- /.row -->




