---
title: "Han&Wang Lab - Research"
layout: textlay
excerpt: "Han&Wang Lab -- Research"
sitemap: false
permalink: /research/
---

## 第一部分：基于血浆多维标志物（Aβ/tau/GFAP）构建预测AD神经退行性速率的计算模型研究
{% assign plasma = site.data.research | where_exp: "item", "item.id == 'plasma'" %}
{% for p in plasma %}
  <div class="paper-card">
    <img src="/assets/images/{{ p.image }}" alt="thumbnail" width="150" style="float:left; margin-right:1rem;">
    <h3><a href="{{ p.url }}" target="_blank">{{ p.title }}</a></h3>
    <p><strong>作者：</strong>{{ p.description | split: ',' | first }}</p>
    <p><strong>期刊：</strong>{{ p.description | split: ',' | last }}</p>
    <p>{{ p.abstract | default: "暂无摘要" }}</p>
    <div style="clear:both;"></div>
  </div>
{% endfor %}

## 第二部分：时域干涉（TI）电场聚焦的个体化精准计算与靶点验证
{% assign ti = site.data.research | where_exp: "item", "item.id == 'ti'" %}
{% for t in ti %}
  <div class="paper-card">
    <img src="/assets/images/{{ t.image }}" alt="thumbnail" width="150" style="float:left; margin-right:1rem;">
    <h3><a href="{{ t.url }}" target="_blank">{{ t.title }}</a></h3>
    <p><strong>作者：</strong>{{ t.description | split: ',' | first }}</p>
    <p><strong>期刊：</strong>{{ t.description | split: ',' | last }}</p>
    <p>{{ t.abstract | default: "暂无摘要" }}</p>
    <div style="clear:both;"></div>
  </div>
{% endfor %}
