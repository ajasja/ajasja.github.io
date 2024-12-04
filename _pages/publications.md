---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign date = '' %} 
<ul style="padding-left: 1.5ch;">
{% for post in site.publications reversed %}

  {% assign currentdate = post.date | date: "%Y" %}
    {% if currentdate != date %}
      <h2 id="y{{post.date | date: "%Y"}}"><span style="color:gray">{{ currentdate }}</span></h2>
      {% assign date = currentdate %}
    {% endif %}
  
  <ul style="padding-left: 1.5ch;">
    {% include archive-single-pub.html %}
  </ul>
  
{% endfor %}
</ul>

<p class="legenda" style="font-size: small; color: gray; margin-top: 1.5rem;">* ... special author <br># ... special author</p>