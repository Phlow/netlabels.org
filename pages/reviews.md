---
layout: page
subheadline: "Reviews"
title: "A Collection of Netlabel Reviews"
teaser: "These reviews were written by several Netaudio lovers over the years. Most of the reviews cover the early era of netlabel culture. These reviews are just a tiny glimpse at the flood of available creative commons music releases. They reflect mostly the taste of the reviewer."
permalink: "/reviews/"
show_meta: false
header:
    image_fullwidth: "blog/header_unsplash_8.jpg"
---

## German Reviews

These {% assign counter = 1 %}{% for item in site.reviews %}{% if item.language == 'de' %}{% assign counter=counter | plus:1 %}{% endif %}{% endfor %}{{ counter }} German netlabel music reviews were mostly written for the German Phlow Magazin Blog.

{% include list-reviews language='de' prefix_text='<span class="subheader">Musikkritik </span>' %}


