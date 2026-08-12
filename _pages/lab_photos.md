---
layout: page
permalink: /lab-photos/
title: Lab Photos
description: a gallery of past Cheng Lab moments
nav: true
nav_order: 7
---

<style>
  html,
  body {
    font-family: "Open Sans", Arial, sans-serif;
    font-size: 110%;
  }
  #search-toggle .nav-link {
    font-size: 0;
  }
  #search-toggle .nav-link::before {
    content: "Search";
    font-size: 1rem;
    margin-right: 0.4em;
  }
  #search-toggle .nav-link i {
    font-size: 1rem;
  }
  .post-title {
    font-size: 40px; /* keep header text at its original (pre-150%) size */
  }
  .navbar .nav-link {
    font-size: 24px; /* keep navbar menu items at their original (pre-150%) size */
  }

  /* Sub-navigation bar: sticks just below the main navbar so the four
     category links stay reachable while scrolling through the photos. */
  .photo-subnav {
    position: sticky;
    top: 73px;
    z-index: 10;
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    padding: 1rem 0;
    background-color: #ffffff;
    margin-bottom: 0.5rem;
  }
  .photo-subnav a {
    padding: 0.5rem 1.25rem;
    border-radius: 999px;
    background-color: #1565c0;
    color: #ffffff;
    font-weight: 600;
    font-size: 0.95rem;
    text-decoration: none;
  }
  .photo-subnav a:hover {
    opacity: 0.85;
  }

  /* Category section headers: standard text, not the blue banner used elsewhere. */
  .photo-section-header {
    margin: 2.5rem 0 1.5rem 0;
    scroll-margin-top: 90px; /* keeps the heading clear of the sticky bars when jumped to */
  }
  .photo-section-header:first-of-type {
    margin-top: 0.5rem;
  }

  /* Masonry-style gallery: a constant number of columns, but each photo keeps
     its own natural aspect ratio instead of being cropped to a fixed shape. */
  .photo-gallery {
    column-count: 3;
    column-gap: 1rem;
  }
  .photo-gallery figure {
    margin: 0 0 1rem 0;
    break-inside: avoid;
  }
  .photo-gallery img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 0.5rem;
  }
  .photo-gallery figcaption {
    margin-top: 0.35rem;
    font-size: 0.85em;
    font-style: italic;
    opacity: 0.75;
  }
  @media (max-width: 768px) {
    .photo-gallery {
      column-count: 2;
    }
  }
  @media (max-width: 480px) {
    .photo-gallery {
      column-count: 1;
    }
  }
</style>

<nav class="photo-subnav">
  <a href="#lab-outings">Lab Outings</a>
  <a href="#lab">Lab</a>
  <a href="#defense-parties">Defense Parties</a>
  <a href="#conferences-and-retreats">Conferences and Retreats</a>
</nav>

{% assign photo_categories = "Lab Outings|Lab|Defense Parties|Conferences and Retreats" | split: "|" %}
{% for category in photo_categories %}
{% assign anchor = category | slugify %}
{% assign folder_path = "/assets/img/lab_photos/" | append: category | append: "/" %}

  <h2 id="{{ anchor }}" class="photo-section-header">{{ category }}</h2>

  <div class="photo-gallery">
    {% assign category_photos = site.static_files | where_exp: "f", "f.path contains folder_path" %}
    {% for photo in category_photos %}
      {% assign ext = photo.extname | downcase %}
      {% if ext == ".jpg" or ext == ".jpeg" or ext == ".png" or ext == ".gif" %}
        {% assign rel_path = category | append: "/" | append: photo.name %}
        {% assign caption = site.data.lab_photo_captions[rel_path] %}
        <figure>
          <img src="{{ photo.path | relative_url | uri_escape }}" alt="Cheng Lab photo — {{ category }}">
          {% if caption %}
            <figcaption>{{ caption }}</figcaption>
          {% endif %}
        </figure>
      {% endif %}
    {% endfor %}
  </div>
{% endfor %}

<!-- To add more photos: drop image files into the matching assets/img/lab_photos/<Category>/
     subfolder — this page picks them up automatically, no edits needed here.
     To caption a specific photo: add a line to _data/lab_photo_captions.yml (see that
     file for the exact format). -->
