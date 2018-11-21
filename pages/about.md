---
layout: page
title: About
description: 任天宇的博客
keywords: Cyrusr Ren,Ren TianYu, 任天宇
comments: true
menu: 关于
permalink: /about/
---

我是任天宇，目前就读于武汉理工大学。

我喜欢编程，也会继续学习！

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
