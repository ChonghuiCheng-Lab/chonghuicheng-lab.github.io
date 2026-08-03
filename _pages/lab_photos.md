---
layout: page
permalink: /lab-photos/
title: lab photos
description: a gallery of past Cheng Lab moments
nav: true
nav_order: 6
---

<style>
  :root {
    --global-bg-color: #e0e2dc;
    --global-card-bg-color: #e0e2dc;
  }
  html,
  body {
    font-family: "Open Sans", Arial, sans-serif;
  }
  .photo-gallery {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 1rem;
    margin-top: 1.5rem;
  }
  .photo-gallery img {
    width: 100%;
    height: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 0.5rem;
    display: block;
  }
</style>

<div class="photo-gallery">
  {% assign lab_photos = site.static_files | where_exp: "f", "f.path contains '/assets/img/lab_photos/'" %}
  {% for photo in lab_photos %}
    {% assign ext = photo.extname | downcase %}
    {% if ext == ".jpg" or ext == ".jpeg" or ext == ".png" or ext == ".gif" %}
      <img src="{{ photo.path | relative_url }}" alt="Cheng Lab photo">
    {% endif %}
  {% endfor %}
</div>

<!-- To add more photos, just drop image files into assets/img/lab_photos/ — this page picks them up automatically, no other edits needed. -->
