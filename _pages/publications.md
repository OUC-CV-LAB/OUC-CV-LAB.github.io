---
title: "计算机视觉前沿交叉实验室 - Publications"
layout: gridlay
excerpt: "计算机视觉前沿交叉实验室 -- Publications."
sitemap: false
permalink: /publications/
---


<div class="publications-hero">
  <div class="publications-hero-content">
    <h1 class="publications-title">📚 学术论文</h1>
    <p class="publications-subtitle">发表在国际顶级会议和期刊的研究成果</p>
  </div>
</div>

---

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if publi.code %}
{% if publi.cn %}
<div class="col-sm-12 clearfix">
 <div class="publication-card">
  <div class="publication-image">
    <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" alt="论文配图" />
  </div>
  <div class="publication-content">
    <h3 class="publication-title"><a href="{{ publi.link.url }}">{{ publi.title }}</a></h3>
    <p class="publication-venue">{{ publi.link.display }}</p>
    <div class="publication-links">
      <a href="{{ publi.pdf }}" class="publication-link pdf-link">📄 PDF</a>
      <a href="{{ publi.code }}" class="publication-link code-link">💻 Code</a>
      <a href="{{ publi.cn }}" class="publication-link cn-link">🇨🇳 中文解读</a>
    </div>
  </div>
 </div>
</div>
{% else %}
<div class="col-sm-12 clearfix">
 <div class="publication-card">
  <div class="publication-image">
    <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" alt="论文配图" />
  </div>
  <div class="publication-content">
    <h3 class="publication-title"><a href="{{ publi.link.url }}">{{ publi.title }}</a></h3>
    <p class="publication-venue">{{ publi.link.display }}</p>
    <div class="publication-links">
      <a href="{{ publi.pdf }}" class="publication-link pdf-link">📄 PDF</a>
      <a href="{{ publi.code }}" class="publication-link code-link">💻 Code</a>
    </div>
  </div>
 </div>
</div>
{% endif %}
{% else %}
{% if publi.cn %}
<div class="col-sm-12 clearfix">
 <div class="publication-card">
  <div class="publication-image">
    <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" alt="论文配图" />
  </div>
  <div class="publication-content">
    <h3 class="publication-title"><a href="{{ publi.link.url }}">{{ publi.title }}</a></h3>
    <p class="publication-venue">{{ publi.link.display }}</p>
    <div class="publication-links">
      <a href="{{ publi.pdf }}" class="publication-link pdf-link">📄 PDF</a>
      <a href="{{ publi.cn }}" class="publication-link cn-link">🇨🇳 中文解读</a>
    </div>
  </div>
 </div>
</div>
{% else %}
<div class="col-sm-12 clearfix">
 <div class="publication-card">
  <div class="publication-image">
    <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" alt="论文配图" />
  </div>
  <div class="publication-content">
    <h3 class="publication-title"><a href="{{ publi.link.url }}">{{ publi.title }}</a></h3>
    <p class="publication-venue">{{ publi.link.display }}</p>
    <div class="publication-links">
      <a href="{{ publi.pdf }}" class="publication-link pdf-link">📄 PDF</a>
    </div>
  </div>
 </div>
</div>
{% endif %}
{% endif %}
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



