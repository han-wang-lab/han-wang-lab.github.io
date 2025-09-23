---
title: "Han&Wang Lab - Home"
layout: homelay
excerpt: "Han&Wang Lab"
sitemap: false
permalink: /
---

# 认知神经工程与AD精准调控团队

<!-- 统一 16:9 轮播 -->
<style>

/* === 画框：16:9 + 圆角 === */
.carousel-dual{
  position:relative;
  max-width:100%;
  margin:auto;
  overflow:hidden;   /* 必须，让圆角把图片裁掉 */
  aspect-ratio:16 / 9;
  border-radius:12px; /* 圆角大小随意调 */
}
/* IE / 旧浏览器 fallback（如需要） */
@supports not (aspect-ratio:16/9){
  .carousel-dual{height:0; padding-bottom:56.25%;}
}

/* === 图片：铺满 + 居中裁剪 + 无边框 === */
.carousel-dual img{
  position:absolute;
  top:0; left:0;
  width:100%; height:100%;
  object-fit:cover;
  display:none;
  border:none;
  border-radius:12px; /* 与容器保持一致 */
}
.carousel-dual img.active{display:block;}

/* === 按钮 === */
.carousel-dual button{
  position:absolute;
  top:50%; transform:translateY(-50%);
  background:rgba(0,0,0,.4); color:#fff;
  border:none; padding:6px 12px; font-size:20px;
  cursor:pointer; user-select:none;
}
.carousel-dual .prev{left:0;}
.carousel-dual .next{right:0;}
</style>

<!-- === 图片容器 === -->
<div class="carousel-dual">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/team3-1.jpg" class="active" alt="team">
   <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/teamall.jpg" alt="team3">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/team2.jpg" alt="lab">

  <button class="prev" onclick="changeD(-1)">&#10094;</button>
  <button class="next" onclick="changeD(1)">&#10095;</button>
</div>

<!-- === 轮播逻辑 === -->
<script>
(function(){
  const imgs = document.querySelectorAll('.carousel-dual img');
  let idx = 0;

  window.changeD = function(d){
    imgs[idx].classList.remove('active');
    idx = (idx + d + imgs.length) % imgs.length;
    imgs[idx].classList.add('active');
  };

  /* 自动播放 */
  setInterval(function(){ changeD(1); }, 4000);
})();
</script>

<!-- ![]({{ site.url }}{{ site.baseurl }}/images/teamall.jpg){: style="width: 150px; float: left;margin-right: 20px; border: 10px"} -->
<!-- ![]({{ site.url }}{{ site.baseurl }}/images/teampic/teamall.jpg){: style="width: 100%; border: 10px"} -->
<br>

## 团队介绍：

随着全球人口老龄化进程的加剧，以阿尔茨海默病（AD）为代表的神经退行性疾病已成为严峻的社会与健康挑战。这类疾病的病理机制复杂，早期诊断困难，且缺乏有效的干预手段。本团队致力于融合前沿神经影像学、计算科学与神经调控工程，进行认知障碍的“精准诊疗（Theranostics）”。开发并应用多模态磁共振成像技术（sMRI, fMRI, DTI等），结合人工智能与先进的计算模型，挖掘能够在临床症状出现前预警疾病风险的、高维度的生物标记物。同时，我们积极探索以时域干涉（Temporal Interference，TI）为代表的新型无创深部脑刺激技术，旨在通过精确调控病理状态下的深部大脑核团与神经网络，实现对认知功能的修复与重塑。我们的最终目标是建立一个从基础理论（高阶脑网络机制）到关键技术（多模态生物标记物、TI无创神经调控），再到临床应用（AD的早期诊断与干预）的完整研究闭环，为攻克神经退行性疾病提供创新的理论基础和工程解决方案。
<!-- The Ying Han & Hao Wang Lab aims to advance research in **computer vision**, **robotics**, and **medical imaging**. Over the past few years, we have made significant progress in these fields through our cutting-edge research and collaboration with leading experts in the field. Our work has resulted in numerous publications in top-tier conferences and journals, and we continue to push the boundaries of what is possible with our advanced machine learning techniques, particularly in the areas of deep neural networks. We are excited to continue our research and contribute to the field of computer vision, robotics, and medical imaging. -->
<br>

## 研究方向：
- **阿尔茨海默病的多模态磁共振智能诊断与高阶生物标记物挖掘**
- **时域干涉（TI）无创深部神经调控的物理机制与临床转化研究**
- **大脑结构-功能网络的高阶耦合机制及其在认知障碍中的应用**
- **面向精准干预的神经影像-神经调控闭环计算模型构建**

## News

* 2025年9月5日: 举办神经影像与阿尔茨海默病早期诊断闭门研讨会！
* 2025年9月3日: 研究生新生宋旭东、苏铱鸣、阳标、林荣涵、邓新宇加入课题组！
<!-- * Jul 02, 2021: [College of Engineering Offers Applied Machine Learning Intensive for Summer](https://news.uark.edu/articles/57146/college-of-engineering-offers-applied-machine-learning-intensive-for-summer) -->

## Prospective Students

如果您有兴趣加入，请参阅*[Join Us](recruitment)* 页面。

<p style="color:red;">我们从 2025 年夏季开始为博士后提供空缺职位！</p>
