---
title: "CV前沿交叉组 - Home"
layout: homelay
excerpt: "计算机视觉前沿交叉实验室 at OUC."
sitemap: false
permalink: /
---

## 欢迎来到中国海大计算机视觉前沿交叉实验室


![]({{ site.url }}{{ site.baseurl }}/images/lab_logo.jpg){: style="width: 230px; float: left;margin-right: 20px; border: 10px"}


介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍介绍


我们的主要研究方向是:

1. **A**: AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
2. **B**: BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBB
BBBBBBBBBBBBBBBBBBBBBBBB
3. **C**: CCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCC
4. **D**: DDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD
DDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD
DDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD


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

<!-- 
### 合作
We work with closely with numerous collaborators, including the [State Lab](https://www.mstatelab.com/) and [Bender Lab](https://benderlab.ucsf.edu/lab-members) at UCSF, the [Devlin Lab](https://www.psychiatry.pitt.edu/about-us/our-people/faculty/bernie-j-devlin-phd) at UPMC, the [Roeder Lab](http://www.stat.cmu.edu/~roeder/) at Carnegie Mellon, the [Sestan Lab](http://medicine.yale.edu/lab/sestan/index.aspx), and the [Talkowski lab](http://talkowski.mgh.harvard.edu/) at Harvard.

### 加入我们
If you are interested in joining please go to the [recruitment](recruitment) page. -->

### 联系我们
联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们联系我们


<figure class="third">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/xiaohui.png" style="width: 200px">	

<!-- <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_SFARI.png" style="width: 200px">

<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_ASF.jpeg" style="width: 200px"> <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_BBRF.png" style="width: 200px">
</figure> -->






