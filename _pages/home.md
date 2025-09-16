---
title: "Han&Wang Lab - Home"
layout: homelay
excerpt: "Han&Wang Lab"
sitemap: false
permalink: /
---

# Welcome to Ying Han & Hao Wang Lab

<!-- 双图轮播，适配原主题 -->
<style>
.carousel-dual{position:relative;max-width:100%;margin:auto;overflow:hidden}
.carousel-dual img{width:100%;display:none;border:10px solid #fff}
.carousel-dual img.active{display:block}
.carousel-dual button{position:absolute;top:50%;transform:translateY(-50%);background:rgba(0,0,0,.4);color:#fff;border:none;padding:4px 8px;font-size:18px;cursor:pointer}
.carousel-dual .prev{left:0}
.carousel-dual .next{right:0}
</style>

<div class="carousel-dual">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/teamall.jpg" class="active" alt="team">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/lab1.jpg" alt="lab">

  <button class="prev" onclick="changeD(-1)">&#10094;</button>
  <button class="next" onclick="changeD(1)">&#10095;</button>
</div>

<script>
(function(){
  let idx=0, imgs=document.querySelectorAll('.carousel-dual img');
  window.changeD=function(d){
    imgs[idx].classList.remove('active');
    idx=(idx+d+imgs.length)%imgs.length;
    imgs[idx].classList.add('active');
  };
  setInterval(function(){changeD(1)},4000);
})();
</script>

<!-- ![]({{ site.url }}{{ site.baseurl }}/images/teamall.jpg){: style="width: 150px; float: left;margin-right: 20px; border: 10px"} -->
<!-- ![]({{ site.url }}{{ site.baseurl }}/images/teampic/teamall.jpg){: style="width: 100%; border: 10px"} -->
The AICV Lab aims to advance research in **computer vision**, **robotics**, and **medical imaging**. Over the past few years, we have made significant progress in these fields through our cutting-edge research and collaboration with leading experts in the field. Our work has resulted in numerous publications in top-tier conferences and journals, and we continue to push the boundaries of what is possible with our advanced machine learning techniques, particularly in the areas of deep neural networks. We are excited to continue our research and contribute to the field of computer vision, robotics, and medical imaging.
<br>

## News

* 2025年9月5日: 举办神经影像与阿尔茨海默病早期诊断闭门研讨会！
* 2025年9月3日: 研究生新生宋旭东、苏铱鸣、阳标、林荣涵、邓新宇加入课题组！
<!-- * Jul 02, 2021: [College of Engineering Offers Applied Machine Learning Intensive for Summer](https://news.uark.edu/articles/57146/college-of-engineering-offers-applied-machine-learning-intensive-for-summer) -->

## Prospective Students

如果您有兴趣加入，请参阅*[Join Us](recruitment)* 页面。

<p style="color:red;">我们从 2025 年夏季开始为博士生（研究助理）提供空缺职位！</p>
