---
layout: default
title: misc
permalink: /misc/
nav: true
nav_order: 5
collection: media
---

{% assign media = site.data.media %}

<style>
.media-container {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

figure.cover {
  position: relative;
  margin: 0;
  display: inline-block;
}

figure.cover img {
  display: block;
}

figcaption {
  position: absolute;
  bottom: 12px;
  left: -4px;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.05em;
  padding: 3px 8px 3px 6px;
  clip-path: polygon(0 0, 100% 0, 93% 50%, 100% 100%, 0 100%);
}

.status-completed  { background: #1D9E75; color: #E1F5EE; }
.status-reading    { background: #378ADD; color: #E6F1FB; }
.status-watching   { background: #378ADD; color: #E6F1FB; }
.status-paused     { background: #BA7517; color: #FAEEDA; }
.status-dropped    { background: #A32D2D; color: #FCEBEB; }
.status-plan       { background: #888780; color: #F1EFE8; }
</style>

## Books

{% assign books = media | where: "type", "book" %}

<div class="media-container">
{% for item in books %}
  <figure class="cover">
    {% if item.cover %}
      <img src="{{ item.cover | relative_url }}" alt="{{ item.title }}" style="height:200px">
    {% endif %}
    {% if item.status == "completed" %}
      <figcaption class="status-completed">COMPLETED</figcaption>
    {% elsif item.status == "reading" %}
      <figcaption class="status-reading">READING</figcaption>
    {% elsif item.status == "paused" %}
      <figcaption class="status-paused">PAUSED</figcaption>
    {% elsif item.status == "dropped" %}
      <figcaption class="status-dropped">DROPPED</figcaption>
    {% else %}
      <figcaption class="status-plan">PLAN TO READ</figcaption>
    {% endif %}
  </figure>
{% endfor %}
</div>

## Shows / Movies

{% assign shows = media | where: "type", "show" %}

<div class="media-container">
{% for item in shows %}
  <figure class="cover">
    {% if item.cover %}
      <img src="{{ item.cover | relative_url }}" alt="{{ item.title }}" style="height:200px">
    {% endif %}
    {% if item.status == "completed" %}
      <figcaption class="status-completed">COMPLETED</figcaption>
    {% elsif item.status == "watching" %}
      <figcaption class="status-watching">WATCHING</figcaption>
    {% elsif item.status == "paused" %}
      <figcaption class="status-paused">PAUSED</figcaption>
    {% elsif item.status == "dropped" %}
      <figcaption class="status-dropped">DROPPED</figcaption>
    {% else %}
      <figcaption class="status-plan">PLAN TO WATCH</figcaption>
    {% endif %}
  </figure>
{% endfor %}
</div>

<!-- ## Movies
{% assign movies = media | where: "type", "movie" %}
<div class="media-container">
{% for item in movies %}
  <figure class="cover">
    {% if item.cover %}
      <img src="{{ item.cover | relative_url }}" alt="{{ item.title }}" style="height:200px">
    {% endif %}
    {% if item.status == "completed" %}
      <figcaption class="status-completed">COMPLETED</figcaption>
    {% elsif item.status == "watching" %}
      <figcaption class="status-watching">WATCHING</figcaption>
    {% elsif item.status == "paused" %}
      <figcaption class="status-paused">PAUSED</figcaption>
    {% elsif item.status == "dropped" %}
      <figcaption class="status-dropped">DROPPED</figcaption>
    {% else %}
      <figcaption class="status-plan">PLAN TO WATCH</figcaption>
    {% endif %}
  </figure>
{% endfor %}
</div>
 -->

## Spotify Playlists

<ul class="playlist-list">
  <li>
    <a href="https://open.spotify.com/playlist/7dPw5BM1sWJ69LI0gAyFGZ?si=12ae74a03c994e73" target="_blank">
      Spring 2026, Chem 322
    </a>
  </li>

  <li>
    <a href="https://open.spotify.com/" target="_blank">
      Fall 2026, Chem 120
    </a>
  </li>
</ul>
