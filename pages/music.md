---
layout: page-fullwidth
subheadline: "Netlabel & Netaudio Music"
title: "Discover Free Creative Commons Music"
teaser: 'Discover music in four different ways: <a href="http://netlabels.org/electronic-music/">Filter</a> netlabels for your favorite genre, check out <a href="http://netlabels.org/netlabels/">netlabels</a> in our database, have a look at the freshest netlabel <a href="http://netlabels.org/releases/">releases</a> or read some <a href="http://netlabels.org/reviews/">music reviews</a>.'
meta_description: "Discover free creative commons music by filter, by netlabels, by releases or read reviews."
header:
    image_fullwidth: "blog/header-listening-music.jpg"
permalink: "/music/"
show_meta: false
---

<div class="row">

<div class="medium-3 columns">
    <h2 class="b15">Filter</h2>
    <p>What kind of music do you like? Easily filter netlabels by genre.</p>
    <a class="button radius small" href="{{ site.url }}/electronic-music/">Genre Filter ›</a>
</div><!-- /.medium-3.columns -->


<div class="medium-3 columns">
    <h2 class="b15">{% include count-collection-items collection='netlabels' %} Netlabels</h2>
    <p>There are currently {% include count-collection-items collection='netlabels' %} netlabels in our database.</p>
    <a class="button radius small" href="{{ site.url }}/netlabels/">Show netlabels ›</a>
</div><!-- /.medium-3.columns -->


<div class="medium-3 columns">
    <h2 class="b15">{% include count-collection-items collection='releases' %} Releases</h2>
    <p>There are currently {% include count-collection-items collection='releases' %} releases in our database.</p>
    <a class="button radius small" href="{{ site.url }}/releases/">Listen to releases ›</a>
</div><!-- /.medium-3.columns -->



<div class="medium-3 columns">
    <h2 class="b15">{% include count-collection-items collection='reviews' %} Reviews</h2>
    <p>What do the critics say? Read one of our {% include count-collection-items collection='reviews' %} reviews.</p>
    <a class="button radius small" href="{{ site.url }}/reviews/">Read reviews ›</a>
</div><!-- /.medium-3.columns -->


</div><!-- /.row -->
