---
layout: default
title: Home
---

# Welcome to Investing ideas

{% assign categories = site.categories | sort %}
{% for category in categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% assign posts = category[1] | sort_natural: "title" %}
    {% for post in posts %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
