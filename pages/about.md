---
layout: page
title: About
description: 这个世界的真相是哈七
keywords: daqi, BigQ
comments: true
menu: 关于
permalink: /about/
---

人需要做正确的事情，哪怕是慢点。

代码需要策略和刻意练习。

不走弯路，就是捷径。

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
