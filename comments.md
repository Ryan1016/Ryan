﻿---
layout: page
title: 留言
---
交换友链可以在评论区留言~

{% for friend in site.friends %}
<div class="card">
    <div class="card-portrait">
        <a href="{{ friend.src }}"><img src="{{ friend.portrait }}"></a>
    </div>
    <div class="card-information">
        <p style="text-align:center; font-size:30px">{{ friend.name }}</p>
        <p style="text-align:center; font-size:20px">{{ friend.description }}</p>
    </div>
</div>
{% endfor %}

{% include valine.html %}
