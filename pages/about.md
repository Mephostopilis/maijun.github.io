---
layout: page
title: About
description: 打码改变世界
keywords: Mr. Hu
comments: true
menu: 关于
permalink: /about/
---

我是机器人少儿教育胡老师，传播stem教育

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
