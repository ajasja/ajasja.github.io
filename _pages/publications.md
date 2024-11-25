---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign date = '' %} 
<ul>
{% for post in site.publications reversed %}

  {% assign currentdate = post.date | date: "%Y" %}
    {% if currentdate != date %}
      <h2 id="y{{post.date | date: "%Y"}}"><span style="color:gray">{{ currentdate }}</span></h2>
      {% assign date = currentdate %}
    {% endif %}
  
  <ul>
    {% include archive-single-pub.html %}
  </ul>
  
{% endfor %}
</ul>
