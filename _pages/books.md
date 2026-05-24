---
layout: default
title: misc
permalink: /misc/
nav: true
nav_order: 5
collection: books
---

## Books that I am reading, have read, or will read

{% assign books = site.books | sort: "year" | reverse %}
{% assign year = nil %}
{% for item in books %}
  {% assign current_year = item.year %}
  {% if current_year != year %}
    {% unless forloop.first %}</div>{% endunless %}
    <h1 id="y{{ current_year }}">{{ current_year }}</h1>
    <div class="year-group">
    {% assign year = current_year %}
  {% endif %}
  <figure class="cover">
    {% if item.cover %}
      <img src="{{ item.cover | relative_url }}" alt="{{ item.title }}" style="height:200px">
    {% endif %}
    {% if item.finished %}
      <figcaption class="finished">FINISHED</figcaption>
    {% else %}
      <figcaption class="unfinished">UNFINISHED</figcaption>
    {% endif %}
  </figure>
{% endfor %}
{% if books.size > 0 %}</div>{% endif %}