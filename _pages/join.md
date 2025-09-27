---
title: "计算机视觉前沿交叉实验室 - Data"
layout: activity0_lay
excerpt: "计算机视觉前沿交叉实验室 -- Data."
sitemap: false
permalink: /join.html
---

# <span style="color:red">参与学术活动</span>

---

<html lang="zh">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>学术活动介绍</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
    }
    .activity-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 30px;
    }
    .activity-title {
      font-size: 1.5em;
      font-weight: bold;
      color: #007bff;
      margin-bottom: 10px;
    }
    .activity-photo {
      max-width: 1000px; /* 增加最大宽度 */
      height: auto;
      margin-bottom: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
      transition: transform 0.3s ease;
    }
    .activity-photo:hover {
      transform: scale(1.02);
    }
    .activity-description {
      font-size: 1em;
      text-align: center;
      width: 80%;
      max-width: 800px;
      margin-bottom: 20px;
    }
    .activity-details {
      font-size: 0.9em;
      color: #555;
      text-align: center;
    }
  </style>
</head>
<body>

<!-- 轮播图样式 -->
<style>
    .carousel-container {
        position: relative;
        text-align: center;
        margin: 25px auto;
        max-width: 1200px; /* 增加最大宽度 */
        border-radius: 15px;
        overflow: hidden;
        box-shadow: 0 6px 20px rgba(0,0,0,0.15);
    }

    .carousel-container img {
        width: 100%;
        height: auto; /* 改为auto，让图片完整显示 */
        max-height: 600px; /* 设置最大高度 */
        object-fit: contain; /* 改为contain，完整显示图片 */
        border-radius: 15px;
        box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }

    .carousel-btn {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background-color: rgba(0, 0, 0, 0.6);
        color: white;
        border: none;
        padding: 15px 20px;
        cursor: pointer;
        font-size: 28px;
        border-radius: 50%;
        width: 50px;
        height: 50px;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: all 0.3s ease;
    }

    .carousel-btn.left {
        left: 20px;
    }

    .carousel-btn.right {
        right: 20px;
    }

    .carousel-btn:hover {
        background-color: rgba(0, 0, 0, 0.8);
        transform: translateY(-50%) scale(1.1);
    }
    
    /* 手机端自适应优化 */
    @media (max-width: 768px) {
        body {
            margin: 10px;
        }
        .activity-container {
            margin-bottom: 30px;
            padding: 15px;
        }
        .activity-title {
            font-size: 1.4em;
            margin-bottom: 12px;
        }
        .activity-photo {
            max-width: 100%;
            border-radius: 8px;
        }
        .activity-description {
            font-size: 1em;
            line-height: 1.6;
        }
        .activity-details {
            font-size: 0.9em;
            padding: 12px;
        }
        .carousel-container {
            margin: 20px auto;
            max-width: 100%;
        }
        .carousel-container img {
            max-height: 400px;
        }
        .carousel-btn {
            width: 40px;
            height: 40px;
            font-size: 20px;
            padding: 10px;
        }
        .carousel-btn.left {
            left: 10px;
        }
        .carousel-btn.right {
            right: 10px;
        }
    }
    
    @media (max-width: 480px) {
        .activity-container {
            padding: 10px;
            margin-bottom: 25px;
        }
        .activity-title {
            font-size: 1.2em;
        }
        .activity-photo {
            border-radius: 6px;
        }
        .carousel-container img {
            max-height: 300px;
        }
        .carousel-btn {
            width: 35px;
            height: 35px;
            font-size: 16px;
            padding: 8px;
        }
        .carousel-btn.left {
            left: 5px;
        }
        .carousel-btn.right {
            right: 5px;
        }
    }
</style>

<script>
    const imagesAI = [
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27.jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27(2).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27(3).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27(4).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27(5).jpg"
    ];
    
    const imagesCSIG = [
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-12-13.jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-12-13(2).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-12-13(3).jpg"
    ];

    let currentIndexCSIG = 0; // 当前图片索引
    let currentIndexAI = 0; // 当前图片索引

    function changeImageCSIG(direction) {
        currentIndexCSIG += direction;

        // 处理边界情况（循环切换）
        if (currentIndexCSIG < 0) {
            currentIndexCSIG = imagesCSIG.length - 1;
        } else if (currentIndexCSIG >= imagesCSIG.length) {
            currentIndexCSIG = 0;
        }

        // 更新图片
        document.getElementById("imageDisplayCSIG").src = imagesCSIG[currentIndexCSIG];
    }

    function changeImageAI(direction) {
        currentIndexAI += direction;
        
        // 处理边界情况（循环切换）
        if (currentIndexAI < 0) {
            currentIndexAI = imagesAI.length - 1;
        } else if (currentIndexAI >= imagesAI.length) {
            currentIndexAI = 0;
        }

        // 更新图片
        document.getElementById("imageDisplayAI").src = imagesAI[currentIndexAI];
    }
</script>


















<div class="activity-container">
    <div class="activity-title">中国多媒体大会(ChinaMM )2024 </div>
    <div class="activity-details">
      <strong>时间：</strong>2024年07月24日<br>
      <strong>地点：</strong>宁夏回族自治区银川市<br>
      <strong>主办方：</strong>中国图象图形学学会（CSIG）、中国计算机学会（CCF）
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-7-24(2).jpg" alt="活动合影">
    <div class="activity-description">
        本次会议邀请了本领域国内外学术界和企业界的顶尖专家与学者做主题报告，分享最新的前沿技术与产业热点。会议期间，还将组织学术高峰论坛、前沿技术专题论坛、顶会顶刊论文分享论坛、多媒体智能计算讲习班、企业论坛等多角度、多层次的丰富活动，为参会者提供丰富技术盛宴，全方位地扩大交流范畴，创新交流形式，增强交流实效。
        中国海洋大学蔡青教授已成功通过2024年CCF多媒体执行委员会申请。
    </div>
    
  </div>




<div class="activity-container">
    <div class="activity-title">第七届中国模式识别与计算机视觉大会（PRCV2024）</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年10月18日<br>
      <strong>地点：</strong>新疆乌鲁木齐<br>
      <strong>主办方：</strong>中国自动化学会（CAA）、中国图象图形学学会（CSIG）、中国人工智能学会（CAAI）和中国计算机学会（CCF）联合主办
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-10-18.jpg" alt="活动合影">
    <div class="activity-description">
        本次大会聚焦于模式识别与计算机视觉领域所面临的新挑战、新问题和新发展方向，旨在展示我国在该领域的最新研究进展。大会为科研院所和科技企业的研究、开发及应用相关人员搭建了一个重要的交流平台。
        中国海洋大学蔡青教授参与2024年PRCV并入选CCF-CV专委会。
    </div>

  </div>
<div class="activity-container">
    <div class="activity-title">人工智能前沿论坛・第二期</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年09月27日<br>
      <strong>地点：</strong>中国科学技术大学高新校区<br>
      <strong>主办方：</strong>脑启发智能感知与认知教育部重点实验室
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-9-27.jpg" alt="活动合影">
    <div class="activity-description">
        本次论坛邀请了中国科学院信息工程研究所李凤华研究员、华南理工大学金连文教授、国防科技大学徐昕教授、西安交通大学陈霸东教授、北京理工大学邬霞教授、南京大学智能科学与技术学院党委书记兼执行院长高阳教授、电子科技大学李宏亮教授、山西大学大数据科学与产业研究院院长钱宇华教授、天津大学郝建业副教授、华南理工大学计算机学院院长陈俊龙教授，一共10位人工智能领域专家。中国科学技术大学党委常委、副校长吴枫教授，脑启发智能感知与认知教育部重点实验室副主任王杰教授，中国科学技术大学大数据学院副院长何向南教授，中国科学技术大学谢洪涛教授、张天柱教授等出席会议，此外现场来宾还有来自中国科学技术大学、南京大学、合肥工业大学、安徽大学等高校师生及科研院所学者专家，参会人次共计300余人。
    </div>
    
  </div>
<div class="activity-container">
    <div class="activity-title">人工智能前沿论坛・第一期</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年08月30日<br>
      <strong>地点：</strong>合肥<br>
      <strong>主办方：</strong>脑启发智能感知与认知教育部重点实验室
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-8-30.png" alt="活动合影">
    <div class="activity-description">
        本次论坛邀请了同济大学苗夺谦教授、北京交通大学人工智能研究院院长于剑教授、浙江大学计算机学院副院长杨易教授、南京航天航空大学人工智能学院院长张道强教授、东南大学研究生院常务副院长耿新教授、武汉大学计算机学院院长杜博教授在内的六位人工智能领域专家，中国科学技术大学党委常委、副校长吴枫教授，脑启发智能感知与认知教育部重点实验室副主任王杰教授，中国科学技术大学大数据学院副院长何向南教授出席会议，此外现场来宾还有来自中国科学技术大学、合肥工业大学、安徽大学等高校师生及科研院所专家学者，参会人员共计200余人。
    </div>
    
  </div>
<div class="activity-container">
    <div class="activity-title">献礼校庆十周年——AI+Science智启未来院士高峰论坛</div>
    <div class="activity-details">
        <strong>时间：</strong>2024年01月27日<br>
        <strong>地点：</strong>香港中文大学（深圳）<br>
        <strong>主办方：</strong>香港中文大学（深圳）
    </div>

    <!-- 轮播图容器 -->
    <div class="carousel-container">
        <button class="carousel-btn left" onclick="changeImageAI(-1)">&#10094;</button>
        <img id="imageDisplayAI" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-1-27.jpg" alt="活动合影">
        <button class="carousel-btn right" onclick="changeImageAI(1)">&#10095;</button>
    </div>

    <div class="activity-description">
        深圳市模式分析与感知计算重点实验室和香港中文大学（深圳）数据科学学院围绕“AI+Science”主题，于1月27日在港中大（深圳）校园举办“模式分析与感知计算”院士高峰论坛，汇聚全球顶尖学者，共同探讨领域的前沿问题与应用，为港中大（深圳）数据科学学院献礼校庆10周年系列活动拉开序幕。模式分析与感知计算作为人工智能领域的重要分支，在图像处理、自然语言理解、生物特征识别以及信号分析等方面发挥了巨大作用，极大地促进了人工智能技术的发展与创新。本次院士论坛将聚焦新一代人工智能技术，探讨模式分析与感知计算新方法，发掘AI+Science新应用，促进人工智能技术的深入研究和落地，推动未来的科学发展与社会进步。
    </div>
</div>


<div class="activity-container">
    <div class="activity-title">第四届泰山智能产业创新发展大会———元宇宙与创新成果论坛</div>
    <div class="activity-details">
        <strong>时间：</strong>2023年12月15日<br>
        <strong>地点：</strong>山东省潍坊市富华大酒店<br>
        <strong>主办方：</strong>山东省人工智能学会、山东省电力行业协会、潍坊市科学技术协会共同主办
    </div>

    <!-- 轮播图容器 -->
    <div class="carousel-container">
        <button class="carousel-btn left" onclick="changeImageMeta(-1)">&#10094;</button>
        <img id="imageDisplayMeta" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-12-15.jpg" alt="活动合影">
        <button class="carousel-btn right" onclick="changeImageMeta(1)">&#10095;</button>
    </div>

    <div class="activity-description">
        中国海洋大学蔡青教授参与TAIIC2023并获得了2023年山东省人工智能优秀青年奖。
    </div>
</div>


</body>
</html>
