---
layout: frontpage
header: no
widget-1:
    title: 'Netlabel History'
    url: '/history/'
    text: 'Dig through our archive full of articles, interviews, screenshots about netlabel and netaudio culture.'
    image: blog/widget-computer.jpg
widget-2:
    title: 'Listen to netlabel...'
    url: /reviews/
    text: "...releases immidiately and find interesting releases through our archived reviews (currently only in German)."
    image: blog/widget-listening-music.jpg
widget-3:
    title: 'Promote your music'
    url: http://www.facebook.com/netlabels
    text: 'You have a netlabel? You want to promote your releases? Than <a href="http://www.facebook.com/netlabels">promote your new releases on our Facebook-Page</a>.'
    image: blog/unsplash_9-302x182.jpg
---
<div class="row t60">
<div class="medium-6 columns" markdown="1">

## Netlabels
{: .b15 }

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
