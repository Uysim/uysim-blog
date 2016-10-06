---
layout: page
title: Uysim's Blog
tagline: Rails developer
---
{% include JB/setup %}
{% for post in site.posts %}
  <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
  <p>
    <span class="text-muted">{{ post.date | date_to_string }}&raquo;</span>
  </p>
  <p>{{ post.content | strip_html | truncatewords: 100 }}<a href="{{ BASE_PATH }}{{ post.url }}">Read more</a></p>
  <hr>
{% endfor %}

