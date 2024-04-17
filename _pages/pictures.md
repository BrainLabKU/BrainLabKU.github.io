---
title: "Brain Lab - gallery"
layout: piclay
excerpt: "Brain Lab -- gallery"
permalink: /gallery/
---

# Gallery

<hr>
(Right-click *'Open Image in a New Tab'* to see a larger image.)

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="https://storage.googleapis.com/homepage_static_files/gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left; height: 150px;" />
<div style="text-align:center">
<p>{{pic.title}}</p>
</div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>