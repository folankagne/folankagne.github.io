---
layout: archive
permalink: /drafts/
title: "Work in Progress - Drafts"
author_profile: true
---

<style>
  p {
    text-align: justify;
    text-justify: inter-word;
  }
</style>

<p>
Ébauches, textes en chantier: 
</p>

{% include base_path %}
{% assign drafts = site.posts | where: "draft", true %}
{% if drafts.size > 0 %}
  {% for post in drafts %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p><em>Aucun brouillon pour l'instant.</em></p>
{% endif %}
