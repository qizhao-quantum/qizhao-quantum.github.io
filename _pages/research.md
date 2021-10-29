---
title: "InspiringGroup - Publications"
layout: gridlay
excerpt: "InspiringGroup -- Publications."
sitemap: false
permalink: /research/
---

## Publications

### Group highlights

<div class="largefont">
(The following are our research highlights. For a full publication list, please visit [DBLP](https://dblp.org/pid/69/11514.html))
</div>

{% assign number_printed = 0 %}
{% for publi in site.data.projects %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit class="largefont">{{ publi.name }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ publi.image }}" class="img-responsive" width="90%" style="float:right;margin-bottom:18px;" />

  <ul style="overflow: hidden">
	{% if publi.number_desc == 1 %}   
	<li> {{ publi.desc1}} </li> 
	{% endif %}                        

	{% if publi.number_desc == 2 %}   
	<li> {{ publi.desc1}} </li> 
	<li> {{ publi.desc2}} </li> 
	{% endif %}                        

	{% if publi.number_desc == 3 %}   
	<li> {{ publi.desc1}} </li> 
	<li> {{ publi.desc2}} </li> 
	<li> {{ publi.desc3}} </li> 
	{% endif %}                        

	{% if publi.number_desc == 4 %}   
	<li> {{ publi.desc1}} </li> 
	<li> {{ publi.desc2}} </li> 
	<li> {{ publi.desc3}} </li> 
	<li> {{ publi.desc4}} </li> 
	{% endif %}                        

	{% if publi.number_desc == 5 %}   
	<li> {{ publi.desc1}} </li> 
	<li> {{ publi.desc2}} </li> 
	<li> {{ publi.desc3}} </li> 
	<li> {{ publi.desc4}} </li> 
	<li> {{ publi.desc5}} </li> 
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

---

### Selected Publications

{% for publi in site.data.publist %}

  <b>{{ publi.title }}</b><br />
  <em>{{ publi.authors }} </em><br />
  {{publi.conference}}<br />
  {%- if publi.pdf != nil -%}
  <a href="{{ publi.pdf }}">[pdf]</a>
  {% endif %}
  {%- if publi.doi != nil -%}
  <a href="{{ publi.doi }}">[doi]</a>
  {% endif %}
  {%- if publi.slides != nil -%}
  <a href="{{ publi.slides }}">[slides]</a>
  {% endif %}
  {%- if publi.codes != nil -%}
  <a href="{{ publi.codes }}">[codes]</a>
  {% endif %}
  {%- if publi.patent != nil -%}
  <a href="{{ publi.patent }}">[patent]</a>
  {% endif %}

<a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endfor %}
<br />
