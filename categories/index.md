---
layout: page
title: Categories
tags: programming
---

Cat


<h1>{{ page.tag }}</h1>

<ul>
{% for post in site.tags[page.tag] %}
  <li>
    {{ post.date | date: "%B %d, %Y" }}: <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>