---
layout: page-fullwidth
header: no
subheadline: "Catalogue"
title: "Netlabel Releases"
teaser: ""
permalink: "/releases/"
show_meta: false
---
<span class="teaser">There are currently {% include count-collection-items collection='releases' %} releases in our database. This list is sorted by date, where the freshest come first. Happy diggin'!</span>


{% include list-releases collection='releases' showdate='true' sort='release_date' reverse='true' %}
