---
title: "OUC计算机视觉前沿交叉实验室 - Home"
layout: homelay
excerpt: "计算机视觉前沿交叉实验室 at OUC."
sitemap: false
permalink: /
---

### 欢迎来到中国海大计算机视觉前沿交叉实验室


![]({{ site.url }}{{ site.baseurl }}/images/lab_logo.jpg){: style="width: 230px; float: left;margin-right: 20px; border: 10px"}


计算机视觉前沿交叉实验室隶属于<a href="https://www.ai-ouc.cn/" class="off" target="_blank">中国海洋大学人工智能研究院</a>，指导老师为<a href="https://tocaiqing.github.io" class="off" target="_blank">蔡青</a>副教授。我们的主要研究方法包括医学图像处理、疾病辅助诊断、水下视觉、水下图像增强、三维重建等。近年来
团队的研究成果发表于AAAI、IJCAI、MM、TIP等国际顶级学术会议和期刊。实验室先后主持和参与国家自然科学基金、山东省自然科学基金等项目。

欢迎对我们研究方向感兴趣的同学加入实验室，我们实验室学术氛围浓厚、成员融洽、不强制打卡，欢迎各位优秀的同学咨询！同时欢迎学有余力的本科生进入实验室！联系方式：cq@ouc.edu.cn 

<div style="text-align:center;">
  <img id="imageDisplay" src="{{ site.url }}{{ site.baseurl }}/images/homepageimg/1.jpg" alt="Image" style="width: 500px; height: auto;">
  <br>
  <button onclick="changeImage()">切换图片</button>
</div>

<script>
  let currentImage = 1;

  function changeImage() {
    currentImage++;
    if (currentImage > 2) currentImage = 1; // 假设有三张图片
    document.getElementById('imageDisplay').src = `https://example.com/image${currentImage}.jpg`;
  }
</script>

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






