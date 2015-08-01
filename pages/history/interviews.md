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

## Interviews and Portraits in German

<ul class="side-nav">
  {% for interview in site.interviews %}
    {% unless interview.published == false %}
        {% if interview.language == 'de' %}
            <li><a href="{{ site.url }}{{ interview.url }}"><span class="subheader">{{ interview.subheadline }}</span> »{{ interview.title }}«</a></li>
        {% endif %}
    {% endunless %}
  {% endfor %}
  <li>&nbsp;</li>
</ul>