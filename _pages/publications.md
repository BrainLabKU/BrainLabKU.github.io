---
title: "Brain Lab - Publications"
layout: gridlay
excerpt: "Brain Lab - Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Highlights

**At the end of this page, you can find the [full list of publications](#full-list-of-publications).**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  {% if publi.news1 %}
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  {% endif %}
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left"/>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br>

## Full List of publications

<hr>

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

<br>

## Patents
<hr>

### Patent granted
{% for publi in site.data.patent %}

  {{ publi.title }} <br />
  <em>{{ publi.number }} </em>

{% endfor %}

### Patent pending
{% for publi in site.data.patent_pending %}

  {{ publi.title }} <br />
  <em>{{ publi.number }}</em>

{% endfor %}