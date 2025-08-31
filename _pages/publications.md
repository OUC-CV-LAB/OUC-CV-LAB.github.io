---
title: "计算机视觉前沿交叉实验室 - Publications"
layout: gridlay
excerpt: "计算机视觉前沿交叉实验室 -- Publications."
sitemap: false
permalink: /publications/
---

<!-- 英雄区域 -->
<div class="publications-hero">
  <div class="publications-hero-content">
    <div class="publications-hero-icon">📚</div>
    <h1 class="publications-title">学术论文</h1>
    <p class="publications-subtitle">前沿研究成果，推动学科发展</p>
  </div>
</div>

<!-- 论文列表 -->
<div class="publications-section">
  {% assign number_printed = 0 %}
  {% for publi in site.data.publist %}
  {% assign even_odd = number_printed | modulo: 2 %}
  {% if publi.highlight == 1 %}
  
  {% if even_odd == 0 %}
  <div class="row">
  {% endif %}
  
  <div class="col-sm-12">
    <div class="publication-card">
      <div class="publication-image">
        <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" alt="{{ publi.title }}" />
      </div>
      <div class="publication-content">
        <h3 class="publication-title">
          <a href="{{ publi.link.url }}" target="_blank">{{ publi.title }}</a>
        </h3>
        <p class="publication-venue">{{ publi.link.display }}</p>
        <div class="publication-links">
          {% if publi.pdf %}
          <a href="{{ publi.pdf }}" class="publication-link pdf-link" target="_blank">
            <i class="fas fa-file-pdf"></i> PDF
          </a>
          {% endif %}
          {% if publi.code %}
          <a href="{{ publi.code }}" class="publication-link code-link" target="_blank">
            <i class="fas fa-code"></i> Code
          </a>
          {% endif %}
          {% if publi.cn %}
          <a href="{{ publi.cn }}" class="publication-link cn-link" target="_blank">
            <i class="fas fa-language"></i> 中文解读
          </a>
          {% endif %}
        </div>
      </div>
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
</div>



