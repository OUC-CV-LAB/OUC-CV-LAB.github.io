---
title: "计算机视觉前沿交叉实验室 - Team"
layout: gridlay
excerpt: "计算机视觉前沿交叉实验室: Team members"
sitemap: false
permalink: /team/
---

<div class="team-hero">
  <div class="team-hero-content">
    <h1 class="team-title">🌟 团队成员</h1>
    <p class="team-subtitle">汇聚国内外顶尖人才，打造一流研究团队</p>
  </div>
</div>



---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">👨‍🏫</div>
    <h2 class="section-title">导师团队</h2>
    <p class="section-description">引领学术前沿，培养创新人才</p>
  </div>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
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

---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🤝</div>
    <h2 class="section-title">合作学者</h2>
    <p class="section-description">携手共创，推动学术发展</p>
  </div>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
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

---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🎓</div>
    <h2 class="section-title">博士研究生</h2>
    <p class="section-description">深入探索，追求卓越</p>
  </div>

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      {% if member.url %}
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
      {% else %}
      <h4 class="member-name"><a class="off">{{ member.name }}</a></h4>
      {% endif %}
      <p class="member-title">{{ member.info }}</p>
      <p class="member-research">{{ member.info2 }}</p>
      {% if member.pub %}
      <p class="member-publication">{{ member.pub }}</p>
      {% endif %}
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

---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🔬</div>
    <h2 class="section-title">25级研究生</h2>
    <p class="section-description">锐意进取，勇于创新</p>
  </div>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 5 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      {% if member.url %}
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
      {% else %}
      <h4 class="member-name"><a class="off">{{ member.name }}</a></h4>
      {% endif %}
      <p class="member-title">{{ member.info }}</p>
      <p class="member-research">{{ member.info2 }}</p>
      {% if member.pub %}
      <p class="member-publication">{{ member.pub }}</p>
      {% endif %}
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

---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">💡</div>
    <h2 class="section-title">24级研究生</h2>
    <p class="section-description">思维活跃，潜力无限</p>
  </div>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      {% if member.url %}
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
      {% else %}
      <h4 class="member-name"><a class="off">{{ member.name }}</a></h4>
      {% endif %}
      <p class="member-title">{{ member.info }}</p>
      <p class="member-research">{{ member.info2 }}</p>
      {% if member.pub %}
      <p class="member-publication">{{ member.pub }}</p>
      {% endif %}
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

---

<div class="team-section">
  <div class="section-header">
    <div class="section-icon">🚀</div>
    <h2 class="section-title">23级研究生</h2>
    <p class="section-description">经验丰富，成果丰硕</p>
  </div>
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="member-card">
    <div class="member-photo">
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" alt="{{ member.name }}" />
    </div>
    <div class="member-info">
      {% if member.url %}
      <h4 class="member-name"><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
      {% else %}
      <h4 class="member-name"><a class="off">{{ member.name }}</a></h4>
      {% endif %}
      <p class="member-title">{{ member.info }}</p>
      <p class="member-research">{{ member.info2 }}</p>
      {% if member.pub %}
      <p class="member-publication">{{ member.pub }}</p>
      {% endif %}
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






