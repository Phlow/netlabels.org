---
layout: page-fullwidth
subheadline: "Archive"
title: "Netlabel Screenshot Archive"
teaser: "These are ancient screenshots taken between 2002 to 2006. All screenshots where collected by Moritz »mo.« Sauer for his presentations on netlabel culture."
header:
    image_fullwidth: "blog/header_unsplash_8.jpg"
permalink: "/history/netlabel-screenshots/"
show_meta: false
---

<ul class="clearing-thumbs" data-clearing>
{% for screenshot in site.data.netlabel_screenshots %}
  <li><a href="{{ site.url }}/archive/screenshot/{{ screenshot.image }}"><img  data-caption="{{ screenshot.caption }}" class="th" src="{{ site.url }}/archive/screenshot/{{ screenshot.image | replace: '.jpg', '-thumb.jpg' }}"></a></li>
{% endfor %}
</ul>


