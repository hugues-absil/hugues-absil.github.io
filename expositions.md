---
layout: page
title: Expositions
permalink: /expositions/
---

<!-- Timeline
================================================== -->
<ul class="timeline">
{% assign i = 1 %}
{% for post in site.posts %}
{% if post.categorie == "exposition" %}
    <li {% if post.categorie != "exposition" %}class="timeline-inverted"{% endif %}>
      <div class="timeline-badge {% if post.categorie == "exposition" %}danger{% endif %}"><i class="glyphicon {% if post.categorie == "exposition" %}glyphicon-calendar{% else %}glyphicon-hand-right{% endif %}"></i></div>
      <div class="timeline-panel">
        <div class="timeline-heading">
          <h4 class="timeline-title"><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h4>
          {% if post.categorie != "exposition" %}<p><small class="text-muted"><i class="glyphicon glyphicon-time"></i>{% include date.html date=post.date %}</small></p>{% endif %}
        </div>
        <div class="timeline-body">
          {% if post.categorie == "exposition" %}
          <p>
          <i class="fa fa-calendar"></i>&nbsp; {{ post.date_expo }}<br />
          <a href="http://www.openstreetmap.org/search?query={{post.lieu_expo}}"><i class="fa fa-map"></i>&nbsp; {{ post.lieu_expo }}</a><br />
          {% if post.brochure_expo %}<a href="{{ site.baseurl}}/files/expositions/{{ post.brochure_expo }}"><i class="fa fa-file-o"></i>&nbsp; Voir la brochure de l'exposition</a><br />{% endif %}
          {% if post.brochure_expo %}<i class="fa fa-comment"></i>&nbsp; {{ post.comment_expo }}<br />{% endif %}
          </p>
          {% else %}<p>{{ post.content }}</p>{% endif %}
        </div>
      </div>
    </li>
{% endif %}
{% assign i = i+1 %}
{% endfor %}
