---
layout: homepage
permalink: /
title: Articles
date: 2014-06-02T12:26:34-04:00
modified: 2016-02-26T10:36:43-05:00
excerpt: "A collection of things I've written."
subtitle: "A collection of things I've written."
feature:
  visible: true
  headline: "Featured Articles"
  category: articles
notitle: true
---

{% for post in site.categories.articles %}
  {% if post.featured != true %}
  {% include homepage__item.html %}
  {% endif %}
{% endfor %}
