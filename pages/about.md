---

layout: page
title: About
description: 
keywords: 
comments: true
menu: 关于
permalink: /about/
---

慕斯分享一些无聊的碎碎念的地方

## 联系

<ul>

{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mousse-cake.github.io' %}
<li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
