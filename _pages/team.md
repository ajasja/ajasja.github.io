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


<div style="width: 100%; max-height: 400px; overflow: hidden; margin-bottom: 2rem;">
  <img src="/images/team/Group-photo.webp"
       alt="Group photo"
       style="width: 100%; height: auto; object-fit: cover; object-position: center top;">
</div>




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
--------

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
-----------------------

<div class="grid">
<div class="wrapper">
{% for post in site.team %} {% if post.tags contains 'former' %} {% include archive-single-proj-former.html type="grid" %} {% endif %} {% endfor %}
</div>
</div>
