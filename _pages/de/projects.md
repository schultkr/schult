---
layout: archive
title: "Projekte"
permalink: /de/projects/
author_profile: true
---

{% include base_path %}

{% comment %} 
  Hier filtern wir die Kurse, damit nur die mit 'lang: de' angezeigt werden 
{% endcomment %}

{% assign german_projects = site.portfolio |where: "lang", "de" %}

{% for post in german_projects reversed %}
  {% include archive-single.html %}
{% endfor %}
