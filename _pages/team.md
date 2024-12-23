---
title: "Greet our team"
layout: archive
permalink: /team/
sidebar:
  nav: "Team"
author_profile: false
---

<!-- ![Group photo](/images/team/Group-photo.webp) -->  
{% assign photo_dims = "1200 * 623" %}
{% assign crop_top = 5 %}
{% assign crop_bottom = 66 %}
<img src="/images/team/Group-photo.webp" alt="Group photo" style="clip-path: rect({{ crop_top }}% auto {{ crop_bottom }}% auto); margin-bottom: calc(-{{ 100 | minus: crop_bottom }}% / {{ photo_dims }}); margin-top: calc(-{{ crop_top }}% / {{ photo_dims }});">
We are beautiful. But not as beautiful as _de novo_ designed proteins 💁🏻‍♀️


Group Leader
------------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} 
  {% if post.tags contains 'PI' %} 
    {% include archive-single-proj.html type="grid" %} 
  {% endif %} 
{% endfor %}
</div>
</div>

<!-- Researchers
-----------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'researcher' %} {% include archive-single-proj.html type="grid" %} {% endif %} {% endfor %}
</div>
</div> -->

Postdocs
-----------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'postdoc' %} {% include archive-single-proj.html type="grid" %} {% endif %} {% endfor %}
</div>
</div>

PhD Students
------------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'phd' %} {% include archive-single-proj.html type="grid" %} {% endif %} {% endfor %}
</div>
</div>

<!-- Staff
-----
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'staff' %} {% include archive-single-proj.html type="grid" %} {% endif %} {% endfor %}
</div>
</div> -->

Students
--------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'student' %} {% include archive-single-proj.html type="grid" %} {% endif %} {% endfor %}
</div>
</div>

Past members since 2022
--------
<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'former' %} {% include archive-single-proj-former.html type="grid" %} {% endif %} {% endfor %}
</div>
</div>