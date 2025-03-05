---
title: "OUC计算机视觉前沿交叉实验室 - Home"
layout: homelay
excerpt: "计算机视觉前沿交叉实验室 at OUC."
sitemap: false
permalink: /
---



---
<div class="row" style="max-width: 800px; margin: auto;">
### 学术论文
*通讯作者 #共同一作


{% assign count = 0 %}
{% for publi in site.data.publist %}


{% if publi.highlight == 1 %}
{% assign count = count | plus: 1 %}
    {% if count <= 3 %}

<div class="row" style="max-width: 800px; margin: auto;">
<div class="col-sm-12 clearfix">
 <div class="row">
  <p><a class="pub1" style="font-size: 14px; text-decoration: none;">&#8226;{{ publi.brief }}</a></p>
  
 </div>
</div>



</div>

{% endif %}
{% endif %}
{% endfor %}
<a href="{{ site.url }}{{ site.baseurl }}/publications" style="text-decoration: none; color: #007bff; font-weight: bold;">...更多</a>
</div>
---

<!-- 
### 成员
---

#### 导师
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="https://tocaiqing.github.io" class="off" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>
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

---

#### 24级研究生
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
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


#### 23级研究生
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>
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
-->
<!-- 
### 合作
We work with closely with numerous collaborators, including the [State Lab](https://www.mstatelab.com/) and [Bender Lab](https://benderlab.ucsf.edu/lab-members) at UCSF, the [Devlin Lab](https://www.psychiatry.pitt.edu/about-us/our-people/faculty/bernie-j-devlin-phd) at UPMC, the [Roeder Lab](http://www.stat.cmu.edu/~roeder/) at Carnegie Mellon, the [Sestan Lab](http://medicine.yale.edu/lab/sestan/index.aspx), and the [Talkowski lab](http://talkowski.mgh.harvard.edu/) at Harvard.

### 加入我们
If you are interested in joining please go to the [recruitment](recruitment) page. -->
<div class="row" style="max-width: 800px; margin: auto;">
### 联系我们

蔡青副教授

电子邮箱： cq@ouc.edu.cn

办公地址： 中国海洋大学西海岸校区 信息楼南楼A506


<figure class="third">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/xiaohui.png" style="width: 200px">	








