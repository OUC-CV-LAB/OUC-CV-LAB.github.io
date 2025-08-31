---
title: "计算机视觉前沿交叉实验室 - Team"
layout: modern
excerpt: "计算机视觉前沿交叉实验室: Team members"
sitemap: false
permalink: /team/
---

<!-- 英雄区域 -->
<div class="team-hero">
  <div class="team-hero-content">
    <div class="team-hero-icon">👥</div>
    <h1 class="team-title">优秀团队</h1>
    <p class="team-subtitle">汇聚国内外顶尖人才，打造一流研究团队</p>
  </div>
</div>

<!-- 导师团队 -->
<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🎓</div>
    <div>
      <h2 class="section-title">导师团队</h2>
      <p class="section-description">引领研究方向，培养优秀人才</p>
    </div>
  </div>
  
  <div class="team-grid">
    {% assign number_printed = 0 %}
    {% for member in site.data.team_members %}
    {% assign even_odd = number_printed | modulo: 2 %}
    {% if member.group == 0 %}
    
    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}
    
    <div class="col-sm-6">
      <div class="member-card">
        <div class="member-photo">
          <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" alt="{{ member.name }}" />
        </div>
        <div class="member-info">
          <h4 class="member-name">
            {% if member.url %}
            <a href="{{ member.url }}" target="_blank">{{ member.name }}</a>
            {% else %}
            {{ member.name }}
            {% endif %}
          </h4>
          <p class="member-title">{{ member.info }}</p>
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
</div>

<!-- 合作学者 -->
<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🤝</div>
    <div>
      <h2 class="section-title">合作学者</h2>
      <p class="section-description">国际知名学者，共同推进科研发展</p>
    </div>
  </div>
  
  <div class="team-grid">
    {% assign number_printed = 0 %}
    {% for member in site.data.team_members %}
    {% assign even_odd = number_printed | modulo: 2 %}
    {% if member.group == 4 %}
    
    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}
    
    <div class="col-sm-6">
      <div class="member-card">
        <div class="member-photo">
          <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" alt="{{ member.name }}" />
        </div>
        <div class="member-info">
          <h4 class="member-name">
            {% if member.url %}
            <a href="{{ member.url }}" target="_blank">{{ member.name }}</a>
            {% else %}
            {{ member.name }}
            {% endif %}
          </h4>
          <p class="member-title">{{ member.info }}</p>
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
</div>

<!-- 博士研究生 -->
<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🎯</div>
    <div>
      <h2 class="section-title">博士研究生</h2>
      <p class="section-description">潜心研究，追求学术卓越</p>
    </div>
  </div>
  
  <div class="team-grid">
    {% assign number_printed = 0 %}
    {% for member in site.data.team_members %}
    {% assign even_odd = number_printed | modulo: 2 %}
    {% if member.group == 3 %}
    
    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}
    
    <div class="col-sm-6">
      <div class="member-card">
        <div class="member-photo">
          <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" alt="{{ member.name }}" />
        </div>
        <div class="member-info">
          <h4 class="member-name">
            {% if member.url %}
            <a href="{{ member.url }}" target="_blank">{{ member.name }}</a>
            {% else %}
            {{ member.name }}
            {% endif %}
          </h4>
          <p class="member-title">{{ member.info }}</p>
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
</div>

<!-- 硕士研究生 -->
<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🌟</div>
    <div>
      <h2 class="section-title">硕士研究生</h2>
      <p class="section-description">年轻有为，充满创新活力</p>
    </div>
  </div>
  
  <div class="team-grid">
    {% assign number_printed = 0 %}
    {% for member in site.data.team_members %}
    {% assign even_odd = number_printed | modulo: 2 %}
    {% if member.group == 1 or member.group == 2 or member.group == 5 %}
    
    {% if even_odd == 0 %}
    <div class="row">
    {% endif %}
    
    <div class="col-sm-6">
      <div class="member-card">
        <div class="member-photo">
          <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" alt="{{ member.name }}" />
        </div>
        <div class="member-info">
          <h4 class="member-name">
            {% if member.url %}
            <a href="{{ member.url }}" target="_blank">{{ member.name }}</a>
            {% else %}
            {{ member.name }}
            {% endif %}
          </h4>
          <p class="member-title">{{ member.info }}</p>
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
</div>










