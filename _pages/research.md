---
layout: archive
title: "Research fields"
permalink: /research/
sidebar:
  nav: "Research"

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