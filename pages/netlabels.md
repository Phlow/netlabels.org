---
layout: page
title: "Netlabels"
subheadline: ""
teaser: "This is our ever-growing list of netlabels."
permalink: "/netlabels/"
show_meta: false
---
<ul class="side-nav">
  {% for netlabel in site.netlabel %}
    {% unless netlabel.published == false %}
    <li><a href="{{ site.url }}{{ netlabel.url }}">{{ netlabel.netlabel_name }} – <span class="subheader">{{ netlabel.tags | join: ' , ' | upcase }}</span></a></li>
    {% endunless %}
  {% endfor %}
  <li>&nbsp;</li>
</ul>