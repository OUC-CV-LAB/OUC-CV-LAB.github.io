---
title: "计算机视觉前沿交叉实验室 - Activity"
layout: default
excerpt: "计算机视觉前沿交叉实验室: Activity"
sitemap: false
permalink: /activity/
---

<div class="col-sm-12">
  <!-- 英雄区域 -->
  <div class="activity-hero">
    <div class="activity-hero-content">
      <div class="activity-hero-icon">🌍</div>
      <h1 class="activity-title">学术活动</h1>
      <p class="activity-subtitle">国际交流合作，拓展学术视野</p>
    </div>
  </div>

  <!-- 学术活动列表 -->
  <div class="activity-section">
    <div class="section-header">
      <div class="section-icon">🎪</div>
      <div>
        <h2 class="section-title">最新活动</h2>
        <p class="section-description">实验室参与的学术会议、研讨会和合作项目</p>
      </div>
    </div>
    
    <div class="activity-container">
      {% for activity in site.data.news %}
      <div class="activity-item">
        <div class="activity-date">
          <span class="date-day">{{ activity.date | date: "%d" }}</span>
          <span class="date-month">{{ activity.date | date: "%b" }}</span>
        </div>
        <div class="activity-content">
          <h3 class="activity-title">{{ activity.headline }}</h3>
          {% if activity.link %}
          <a href="{{ activity.link }}" class="activity-link" target="_blank">了解更多</a>
          {% endif %}
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</div>



  



  
