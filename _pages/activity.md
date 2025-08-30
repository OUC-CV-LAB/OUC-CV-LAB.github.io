---
title: "计算机视觉前沿交叉实验室 - Data"
layout: activity_all
excerpt: "计算机视觉前沿交叉实验室 -- Data."
sitemap: false
permalink: /activity/
---

<div class="activity-hero">
  <div class="activity-hero-content">
    <h1 class="activity-hero-title">🎯 举办/参与学术活动</h1>
    <p class="activity-hero-subtitle">积极参与国内外学术交流，推动学科发展</p>
  </div>
</div>

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
      max-width: 800px;
      height: auto;
      margin-bottom: 15px;
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
    .activity-photo,
    .carousel-container img {
        width: 100%;
        height: 400px;
        object-fit: cover;
        border-radius: 8px;
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

    .carousel-container {
        position: relative;
        text-align: center;
        margin: 20px auto;
        max-width: 600px;
    }

    .carousel-btn {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background-color: rgba(0, 0, 0, 0.5);
        color: white;
        border: none;
        padding: 10px 15px;
        cursor: pointer;
        font-size: 24px;
    }

    .carousel-btn.left {
        left: 0;
    }

    .carousel-btn.right {
        right: 0;
    }

    .carousel-btn:hover {
        background-color: rgba(0, 0, 0, 0.7);
    }
</style>

<script>
    const imagesMeta = [
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-12-15.jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-12-15_2.jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-12-15_3.jpg"
    ];

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
    const images = [
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-11-26.jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-11-26(2).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-11-26(3).jpg",
        "{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-11-26(4).jpg"
    ];
    let currentIndexCSIG = 0; // 当前图片索引
    let currentIndexAI = 0; // 当前图片索引
    let currentIndexMeta = 0; // 当前图片索引
    let currentIndex = 0; // 当前图片索引
    function changeImageCSIG(direction) {
    currentIndexCSIG += direction;

    if (currentIndexCSIG < 0) {
        currentIndexCSIG = imagesCSIG.length - 1;
    } else if (currentIndexCSIG >= imagesCSIG.length) {
        currentIndexCSIG = 0;
    }

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

    function changeImageMeta(direction) {
        currentIndexMeta += direction;
        
        // 处理边界情况（循环切换）
        if (currentIndexMeta < 0) {
            currentIndexMeta = imagesMeta.length - 1;
        } else if (currentIndexMeta >= imagesMeta.length) {
            currentIndexMeta = 0;
        }

        // 更新图片
        document.getElementById("imageDisplayMeta").src = imagesMeta[currentIndexMeta];
    }
    function changeImage(direction) {
        currentIndex += direction;
        
        // 处理边界情况（循环切换）
        if (currentIndex < 0) {
            currentIndex = images.length - 1;
        } else if (currentIndex >= images.length) {
            currentIndex = 0;
        }

        // 更新图片
        document.getElementById("imageDisplay").src = images[currentIndex];
    }

</script>


<div class="activity-container">
    <div class="activity-title">人工智能前沿论坛・第四期</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年12月26日<br>
      <strong>地点：</strong>中国科学技术大学高新校区<br>
      <strong>主办方：</strong>脑启发智能感知与认知教育部重点实验室
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-12-26.jpg" alt="活动合影">
    <div class="activity-description">
        团队负责人蔡青参加由中国科学技术大学脑启发智能感知与认知教育部重点实验室主办的第四期人工智能前沿论坛。
    </div>
    
  </div>


<div class="activity-container">
    <div class="activity-title">CSIG青年科学家会议</div>
    <div class="activity-details">
        <strong>时间：</strong>2024年12月13日<br>
        <strong>地点：</strong>杭州<br>
        <strong>主办方：</strong>中国图象图形学学会
    </div>

    <!-- 轮播图容器 -->
    <div class="carousel-container">
        <button class="carousel-btn left" onclick="changeImageCSIG(-1)">&#10094;</button>
        <img id="imageDisplayCSIG" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-12-13.jpg" alt="活动合影">
        <button class="carousel-btn right" onclick="changeImageCSIG(1)">&#10095;</button>
    </div>

    <div class="activity-description">
        团队负责人蔡青参加第二十届CSIG青年科学家会议，成功申请到第二十一届CSIG青年科学家会议举办权，并顺利入选青工委。
    </div>
</div>


<div class="activity-container">
    <div class="activity-title">人工智能前沿论坛・第三期</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年11月21日<br>
      <strong>地点：</strong>中国科学技术大学高新校区<br>
      <strong>主办方：</strong>脑启发智能感知与认知教育部重点实验室
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-11-21.png" alt="活动合影">
    <div class="activity-description">
      团队负责人蔡青参加由中国科学技术大学脑启发智能感知与认知教育部重点实验室主办的第二期人工智能前沿论坛本次论坛，于会嘉宾有广州大学张文生教授，复旦大学杨珉教授，北京化工大学朱群雄教授，北京大学查红彬教授，大连理工大学卢湖川教授，清华大学鲁继文教授，同济大学赵生捷教授，中科院自动化所刘成林研究员，上海交通大学王新兵教授，中国科学院大学叶齐祥教授，浙江工业大学梁荣华教授，西安交通大学苏洲教授，天津大学郝建业副教授，厦门大学纪荣嵘教授等专家。
    </div>
  </div>


<div class="activity-container">
    <div class="activity-title">大模型混战时代：智能安防的演进路径和机遇挑战”技术论坛</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年11月9日<br>
      <strong>地点：</strong>山东科技大学计算机科学与工程学院<br>
      <strong>主办方：</strong>中国计算机学会
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-11-09.png" alt="活动合影">
    <div class="activity-description">
      团队负责人蔡青参加由中国科学技术大学脑启发智能感知与认知教育部重点实验室主办的第二期人工智能前沿论坛本次论坛，于会嘉宾有同济大学苗夺谦教授、北京交通大学人工智能研究院院长于剑教授、浙江大学计算机学院副院长杨易教授、南京航天航空大学人工智能学院院长张道强教授、东南大学研究生院常务副院长耿新教授、武汉大学计算机学院院长杜博教授等专家。
    </div>
    
  </div>


<div class="activity-container">
    <div class="activity-title">VALSE Webinar 十周年特别活动</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年10月26日<br>
      <strong>地点：</strong>中国海洋大学西海岸校区<br>
      <strong>主办方：</strong>VALSE
    </div>
  
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-10-26.jpg" alt="活动合影">
    <div class="activity-description">
      团队负责人蔡青成功在中国海洋大学西海岸校区举办VALSE Webinar十周年特别活动。VALSE Webinar已成功举办365期。
    </div>
  
  </div>


<div class="activity-container">
    <div class="activity-title">第七届中国模式识别与计算机视觉大会（PRCV2024）</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年10月18日<br>
      <strong>地点：</strong>新疆乌鲁木齐<br>
      <strong>主办方：</strong>中国自动化学会（CAA）、中国图象图形学学会（CSIG）、中国人工智能学会（CAAI）和中国计算机学会（CCF）联合主办
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-10-18.jpg" alt="活动合影">
    <div class="activity-description">
        团队负责人蔡青参加第七届中国模式识别与计算机视觉大会，并顺利当选CCF-CV专委会委员。
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
       团队负责人蔡青参加由中国科学技术大学脑启发智能感知与认知教育部重点实验室主办的第二期人工智能前沿论坛本次论坛，于会嘉宾有同济大学苗夺谦教授、北京交通大学人工智能研究院院长于剑教授、浙江大学计算机学院副院长杨易教授、南京航天航空大学人工智能学院院长张道强教授、东南大学研究生院常务副院长耿新教授、武汉大学计算机学院院长杜博教授等专家。
    </div>
    
  </div>

<div class="activity-container">
    <div class="activity-title">“海洋大模型落地的核心挑战与演进路径”深度技术论坛</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年09月21日<br>
      <strong>地点：</strong>中国海洋大学西海岸校区<br>
      <strong>主办方：</strong>中国计算机学会（CCF）
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-9-21.png" alt="活动合影">
    <div class="activity-description">
        本次论坛由CCF主办，由青岛AC委员中国海洋大学仲国强和CCF YOCSEF青岛委员中国海洋大学蔡青共同担任执行主席，于会嘉宾有南京信息工程大学海洋科学学院院长董昌明教授（中国海洋学会人工智能海洋学专委会主任）、中国海洋大学信息科学与工程学部部长董军宇教授（国家高层次人才计划专家）、国防科技大学汪祥副研究员（湖南省科技创新“湖湘青年英才”、羲和大模型论文一作）等专家。
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
      团队负责人蔡青参加由中国科学技术大学脑启发智能感知与认知教育部重点实验室主办的第一期人工智能前沿论坛本次论坛，于会嘉宾有同济大学苗夺谦教授、北京交通大学人工智能研究院院长于剑教授、浙江大学计算机学院副院长杨易教授、南京航天航空大学人工智能学院院长张道强教授、东南大学研究生院常务副院长耿新教授、武汉大学计算机学院院长杜博教授等专家。
    </div>
    
  </div>

<div class="activity-container">
    <div class="activity-title">举办中国图象图形学学会第二十五期珠峰论坛—视觉前沿技术及创新应用专题研讨会</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年08月21日<br>
      <strong>地点：</strong>中国海洋大学西海岸校区<br>
      <strong>主办方：</strong>中国图象图形学学会
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-8-21.jpg" alt="活动合影">
    <div class="activity-description">
        团队负责人蔡青在青岛成功举办2024中国图象图形学学会第二十五期珠峰论坛—视觉前沿技术及创新应用专题研讨会。于会嘉宾有中国海洋大学电子工程学院郑海永教授、山东大学控制科学与工程学院元辉教授、中国科学院计算技术研究所郭宗辉助理研究员担任执行主席，邀请了南京航空航天大学人工智能学院张道强教授、湖南大学电气与信息工程学院刘敏教授、北京大学计算机学院马思伟教授、浙江大学计算机科学与技术学院李玺教授、北京邮电大学智能工程与自动化学院许长桥教授等专家。
    
  </div>

<div class="activity-container">
    <div class="activity-title">京东副总裁郑宇教授莅临指导工作</div>
    <div class="activity-details">
      <strong>时间：</strong>2024年08月07日<br>
      <strong>地点：</strong>中国海洋大学西海岸校区<br>
      <strong>主办方：</strong>中国海洋大学
    </div>
    <img class="activity-photo" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2024-8-7.jpg" alt="活动合影">
    <div class="activity-description">
        郑宇教授进行 “ 城市计算：释放城市数据要素价值 ” 学术汇报。
    </div>
    
  </div>

<!-- <div class="activity-container">
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
    
  </div> -->

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
        深圳市模式分析与感知计算重点实验室和香港中文大学（深圳）数据科学学院围绕“AI+Science”主题，于1月27日在港中大（深圳）校园举办“模式分析与感知计算”院士高峰论坛，汇聚全球顶尖学者，共同探讨领域的前沿问题与应用，为港中大（深圳）数据科学学院献礼校庆10周年系列活动拉开序幕。
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


<div class="activity-container">
    <div class="activity-title">中国海洋大学"基金申请与论文写作"经验分享会</div>
    <div class="activity-details">
        <strong>时间：</strong>2023年11月26日<br>
        <strong>地点：</strong>中国海洋大学西海岸校区<br>
        <strong>主办方：</strong>中国海洋大学
    </div>

    <!-- 轮播图容器 -->
    <div class="carousel-container">
        <button class="carousel-btn left" onclick="changeImage(-1)">&#10094;</button>
        <img id="imageDisplay" src="{{ site.url }}{{ site.baseurl }}/images/xueshupic/2023-11-26.jpg" alt="活动合影">
        <button class="carousel-btn right" onclick="changeImage(1)">&#10095;</button>
    </div>

    <div class="activity-description">
        中国海洋大学蔡青教授特意举行”基金申请与论文写作”经验分享会，为参与人员提供一个与领域内专家进行深度交流的机会。
    </div>
</div>



  



  
