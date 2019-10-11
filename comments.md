---
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
        <font size="6px">{{ friend.name }}</font><br>
        <font size="4.5px">{{ friend.description }}</font>
    </div>
</div>
{% endfor %}

{% include valine.html %}
