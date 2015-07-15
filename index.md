---
layout: frontpage
widget-1:
    title: 'Promote your music'
    url: http://www.facebook.com/netlabels
    text: 'You have a netlabel? You want to promote your releases? Than <a href="http://www.facebook.com/netlabels">promote your new releases on our Facebook-Page</a>.'
    image: unsplash_9-302x182.jpg
widget-2:
    title: 'Netlabel History'
    url: '/history/'
    text: 'Dig through our archive full of articles, interviews, screenshots about netlabel and netaudio culture.'
    image: widget-computer.jpg
widget-3:
    title: 'Please be patient!'
    url: /news/start/
    text: "We're finally starting over... But you have to be patient. We feed our little project in our rare spare time."
    image: widget-listening-music.jpg
---
<div class="row t60">
<div class="medium-6 columns" markdown="1">

## Netlabels
{: .b15 }

{% include list-netlabels %}

<a class="button radius small" href="{{ site.url }}/netlabels/">Show all netlabels ›</a>


</div><!-- /.medium-6.columns -->
<div class="medium-6 columns" markdown="1">

## Releases
{: .b15 }

<ul class="side-nav">
  {% for release in site.releases limit:7 %}
    {% unless release.published == false %}
    <li><a href="{{ site.url }}{{ release.url }}"><span class="subheader">{{ release.netlabel_name | upcase }}</span> › {{ release.release_artist }} – »{{ release.release_title }}«</a></li>
    {% endunless %}
  {% endfor %}
  <li>&nbsp;</li>
</ul>

<a class="button radius small" href="{{ site.url }}/releases/">Show all releases ›</a>

</div><!-- /.medium-6.columns -->
</div><!-- /.row -->
