---
title: "Brain Lab - Members"
layout: gridlay
excerpt: "Brain Lab: Team members"
sitemap: false
permalink: /members/
---

# Lab Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

## Research Professor
{% assign number_printed = 0 %}
{% for member in site.data.research_professor %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <div markdown="0" style="padding-top:16px">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}

    </ul>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>


## Ph.D. Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 2 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    {% endif %}
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}
    </ul>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>


## Master Students

{% assign number_printed = 0 %}
{% for member in site.data.master_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 2 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    {% endif %}
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}
    </ul>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>

## Undergraduate Students

{% assign number_printed = 0 %}
{% for member in site.data.undergraduate %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 2 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    {% endif %}
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}
    </ul>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>

## Alumni (Ph.D.)

{% assign number_printed = 0 %}
{% for member in site.data.alumni_phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 2 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    {% endif %}
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}
    </ul>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>

## Alumni (M.Eng.)

{% assign number_printed = 0 %}
{% for member in site.data.alumni_meng %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Email</b>: {{ member.email }}<br></span>
    <span style="padding:0"><b>Research Interest</b></span>
    <ul style="overflow: hidden">
    {% if member.number_educ == 2 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    {% endif %}
    {% if member.number_educ == 3 %}
    <li> {{ member.education1 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education3 }} </li>
    {% endif %}
    </ul>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<br/>

## Administrative Staff

{% assign number_printed = 0 %}
{% for member in site.data.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  
  <div markdown="0" style="padding-top:16px; justify-content:center; align-items:center">
    <span style="font-style:italic; font-size:14px"><b>{{ member.info }}</b><br></span>
    <span><b>Call</b>: 02-3290-3847<br></span>
    <span><b>Office</b>: Science Library 619<br></span>
  </div> 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}