---
title: "Qi Zhao - Research."
layout: gridlay
excerpt: "Qi Zhao - Research."
sitemap: false
permalink: /research/
---

## Research directions

{%### Group highlights}

<div class="largefont">
(The following are our research directions.)
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


<br />
