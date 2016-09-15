---
layout: page
title: Machine Learner
slug: home
---

<p class="lede">Notes , Articles and daily complaints of a Chemist turned Machine Learner.</p>

<ul class="list">
  {% for post in site.posts limit:5 %}
  <li>
    <p class="list__date  muted"><date>{{ post.date | date_to_xmlschema }}</date></p>
    <h3 class="list__title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <div class="list__content">{{ post.excerpt }}</div>
  </li>
  {% endfor %}
  {% for post in site.posts limit:5 offset:5 %}
  <li>
    <p class="list__date  muted"><date>{{ post.date | date_to_xmlschema }}</date></p>
    <h3 class="list__title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
  </li>
  {% endfor %}
</ul>
