---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---
{% include base_path %}

Full list of publication [can be found here](https://scholar.google.com/citations?user=DaHYEd0AAAAJ&hl=en&oi=ao).

# Featured publications

<p class="legenda" style="font-size: small; color: gray; margin-top: 1.5rem;">* ... shared first author <br>✉ ... shared corresponding/senior author</p>
{% assign featured_publications = site.publications | where: "featured", true | sort: "order" %}
<ul >
{% for post in featured_publications %}

    {% include archive-single-pub.html featured=true %}

{% endfor %}
</ul>

{% assign date = '' %}



# All publications
<ul>
{% for post in site.publications reversed %}
  {% if post.featured == true %} {% continue %} {% endif %}
  {% assign currentdate = post.date | date: "%Y" %}
    {% if currentdate != date %}
       <h2 id="y{{post.date | date: "%Y"}}"><span style="color:gray">{{ currentdate }}</span></h2>      
      {% assign date = currentdate %}
    {% endif %}
    {% include archive-single-pub.html %}
    
{% endfor %}

</ul>
