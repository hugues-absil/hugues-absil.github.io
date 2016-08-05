---
layout: page
title: Cours
permalink: /cours/
---

Voici la liste des cours publiés sur ce site :

## Cours d’[histoire de l'art]({{ site.baseurl }}/cours/histoire-art) ;
{% for item in site.courshistoire %}
  - [{{ item.title }}]({{ item.url }})
{% endfor %}

## Cours sur les [techniques artistiques]({{ site.baseurl }}/cours/techniques-art).
{% for item in site.courstechnique %}
  - [{{ item.title }}]({{ item.url }})
{% endfor %}
