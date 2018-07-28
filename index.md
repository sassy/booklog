---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

# 投稿一覧

<ul>
{% for post in site.posts %}
    <li>{{post.date | date_to_long_string}} <br><a href="{{post.url | | absolute_url}}">{{ post.title }}</a></li>
{% endfor %}
</ul>

