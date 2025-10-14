---
title: "Qi Zhao - Publications"
layout: gridlay
excerpt: "Qi Zhao -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

For research highlights organized by topic, please visit our [Research Directions](/research/) page.

For a full list of publications and patents see [below](#full-list-of-publications) or go to [Google Scholar](https://scholar.google.com/citations?user=VVQuTDMAAAAJ&hl=zh-CN&authuser=1).

## Full List of Publications

{% assign ppidx = 0 %}

{% for publi in site.data.publist %}

{% increment ppidx %}. {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
<br/>


## Patents
<em> Xiongfeng Ma and Qi Zhao </em><br />Measurement-device-independent quantum key distribution with biasedbasis choice<br /> Patent number: ZL201621455743.9

<em> Xiongfeng Ma and Qi Zhao </em><br />Quantum key distribution based on two-way classical communication <br /> Patent number: ZL201621440463.0

<em> Xiongfeng Ma and Qi Zhao </em><br />Quantum key distribution data postprocessing for detector efficiencymismatc <br /> Patent number: CN105049200A

