---
layout: default
title:  "Cartagena, Spain"
image-folder: "cartagena"
camera: "Fujifilm X100T"
film-simulation: "Classic Chrome"
date:   2017-01-15 13:07:25 +0000
---

<div class="container">
  <div class="details">
      <div class="details__item">
        <span class="label">Location: </span>{{ page.title }}
      </div>
      <div class="details__item">
        <span class="label">Camera: </span>{{ page.camera }}
      </div>
      <div class="details__item">
        <span class="label">Film Simluation: </span>{{ page.film-simulation }}
      </div>
  </div>
  <div class="photos">
    {% for image in site.static_files %}
      {% if image.path contains '/assets/images' %}
        <img src="{{ image.path }}" alt="">
      {% endif %}
    {% endfor %}
  </div>
</div>
