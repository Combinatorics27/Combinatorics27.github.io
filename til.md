---
layout: page
title: Today I Learned
permalink: /til/
---

<ul>
{% for post in site.categories.til %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small>— {{ post.date | date: "%d %b %Y" }}</small>
  </li>
{% endfor %}
</ul>
