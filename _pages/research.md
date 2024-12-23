---
layout: archive
title: "Research fields"
permalink: /research/
sidebar:
  nav: "Research"
author_profile: false

---
{% include base_path %}

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