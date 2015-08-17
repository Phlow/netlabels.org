---
layout: page-fullwidth
header: no
subheadline: "Netlabel & Netaudio Music"
title: "Discover Free Music"
teaser: 'This is the best place to start to discover and download free netlabel music. Find new <a href="http://netlabels.org/netlabels/">netlabels</a>, discover <a href="http://netlabels.org/releases/">netlabel releases</a> or check out our archive of <a href="http://netlabels.org/reviews/">music reviews</a>.'
permalink: "/music/"
show_meta: false
---
<div class="row t60">
<div class="medium-6 columns" markdown="1">

## Netlabels
{: .b15 }

<span class="teaser">There are currently {% include count-collection-items collection='netlabels' %} netlabels in our database.</span>

<ul class="side-nav">
    {% assign sorted = (site.netlabels  %}
    {% for netlabel in sorted limit:7 %}
    {% unless netlabel.published == false %}
    <li><a href="{{ site.url }}{{ netlabel.url }}">{{ netlabel.netlabel_name }} – <span class="subheader">{{ netlabel.tags | join: ' , ' | upcase }}</span></a></li>
    {% endunless %}
    {% endfor %}
    <li>&nbsp;</li>
</ul>

<a class="button radius small" href="{{ site.url }}/netlabels/">Show all netlabels ›</a>


</div><!-- /.medium-6.columns -->
<div class="medium-6 columns" markdown="1">

## Releases
{: .b15 }

<span class="teaser">There are currently {% include count-collection-items collection='releases' %} releases in our database.</span>

<ul class="side-nav">
    {% assign sorted = (site.releases | sort: 'release_date') | reverse %}
    {% for release in sorted limit:7 %}
    {% unless release.published == false %}
    <li><a href="{{ site.url }}{{ release.url }}"><span class="subheader">{{ release.netlabel_name | upcase }}</span> › {{ release.release_artist }} – »{{ release.release_title }}«</a></li>
    {% endunless %}
    {% endfor %}
    <li>&nbsp;</li>
</ul>

<a class="button radius small" href="{{ site.url }}/releases/">Show all releases ›</a>


</div><!-- /.medium-6.columns -->
</div><!-- /.row -->





<div class="row">
<div class="medium-6 columns" markdown="1">

## Music Reviews
{: .b15 }

<span class="teaser">There are currently {% include count-collection-items collection='reviews' %} releases in our database.</span>

<ul class="side-nav">
    {% assign sorted = (site.reviews | sort: 'release_date') | reverse %}
    {% for review in sorted limit:7 %}
    {% unless review.published == false %}
    <li><a href="{{ site.url }}{{ review.url }}"><span class="subheader">{{ review.subheadline | upcase }}</span> › {{ review.title }}</a></li>
    {% endunless %}
    {% endfor %}
    <li>&nbsp;</li>
</ul>

<a class="button radius small" href="{{ site.url }}/reviews/">Show all reviews ›</a>



</div><!-- /.medium-6.columns -->
<div class="medium-6 columns" markdown="1">



</div><!-- /.medium-6.columns -->
</div><!-- /.row -->
