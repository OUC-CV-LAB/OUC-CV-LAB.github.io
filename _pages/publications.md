---
title: "计算机视觉前沿交叉实验室 - Publications"
layout: gridlay
excerpt: "计算机视觉前沿交叉实验室: Publications"
sitemap: false
permalink: /publications/
---

<!-- 英雄区域 -->
<div class="publications-hero">
  <div class="publications-hero-content">
    <div class="publications-hero-icon">📚</div>
    <h1 class="publications-title">发表文章</h1>
    <p class="publications-subtitle">高质量学术成果，推动学科发展</p>
  </div>
</div>

<!-- 发表文章列表 -->
<div class="publications-section">
  <div class="section-header">
    <div class="section-icon">📖</div>
    <div>
      <h2 class="section-title">最新发表</h2>
      <p class="section-description">实验室成员在顶级期刊和会议上的重要成果</p>
    </div>
  </div>
  
  <div class="publications-grid">
    {% for pub in site.data.publist %}
    {% if pub.highlight == 1 %}
    <div class="publication-card">
      <div class="publication-image">
        <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ pub.image }}" alt="{{ pub.title }}" />
      </div>
      <div class="publication-content">
        <h3 class="publication-title">
          {% if pub.link.url %}
          <a href="{{ pub.link.url }}" target="_blank">{{ pub.title }}</a>
          {% else %}
          {{ pub.title }}
          {% endif %}
        </h3>
        <p class="publication-authors">{{ pub.link.display }}</p>
        {% if pub.pdf %}
        <a href="{{ pub.pdf }}" class="publication-link" target="_blank">PDF</a>
        {% endif %}
        {% if pub.code %}
        <a href="{{ pub.code }}" class="publication-link" target="_blank">Code</a>
        {% endif %}
      </div>
    </div>
    {% endif %}
    {% endfor %}
  </div>
</div>



