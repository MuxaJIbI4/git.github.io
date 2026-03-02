---
layout: default
title: Summer of Code Archives
---

These pages are historical materials for Summer of Code. They are for reference only!

<ul>
{% for node in site.pages reversed %}
  {% if node.navbar == false %}
    {% if node.title contains "SoC" %}
      <li><a href="{{node.url | relative_url }}">{{node.title}}</a>
    {% endif %}
  {% endif %}
{% endfor %}