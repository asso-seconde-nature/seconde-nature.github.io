---
layout: home
title: News
description: Nouvelles !
---
<section id="news" class="mini-section mt-6 bg-gray-light">
  <div class="container-lg p-responsive">
    <div class="mt-md-12 clearfix gutter-spacious">
      {% for hi in site.data.news %}
      <div class="mb-4 float-left">
        <img class="d-block pr-4 float-left" style="width: 80px;" src="{{ hi.image }}">
        {{ hi.name }}
        <h2 class="alt-h3 mb-2">
          {{ hi.content }}
          <a href="{{ hi.link }}" target="_blank">Plus d'infos</a>
        </h2>
      </div>
      {% endfor %}
    </div>
  </div>
</section>