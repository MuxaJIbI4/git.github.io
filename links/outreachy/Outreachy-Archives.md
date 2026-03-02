---
layout: default
title: Outreachy Archives
---

These pages are historical materials for Outreachy. They are for reference only!

<ul>
{% for node in site.pages reversed %}
  {% if node.navbar == false %}
    {% if node.title contains "Outreachy" %}
      <li><a href="{{node.url | relative_url }}">{{node.title}}</a>
    {% endif %}
  {% endif %}
{% endfor %}
