---
layout: archive
title: "Research fields"
permalink: /research/
sidebar:
  nav: "Research"
author_profile: false

---
{% include base_path %}

## Molecular machines
some text and a photo here

## Design of Binders
Also has some text and an image.

Running projects :running:
------------
<hr>
<div class="grid">
<div class="wrapper">
  {% for post in site.research %}
    {% include archive-single-proj.html type="grid" %}
  {% endfor %}
</div>
</div>