---
title: "计算机视觉前沿交叉实验室 - Publications"
layout: gridlay
excerpt: "计算机视觉前沿交叉实验室 -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

---

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="row">
 	<img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="300px" style="float: right" />
  <p><a class="pub1" style="font-size: 1em;" href="{{ publi.link.url }}">{{ publi.title }}</a></p>
  <a class="pub2" style="font-size: 0.8em;"> {{ publi.link.display }} </a>
    {% if publi.code %}
      <a class="pub2" href="{{ publi.code }}" style="font-size: 0.8em; margin-left: 10px;">[code]</a>
    {% endif %}
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

<p> &nbsp; </p>



