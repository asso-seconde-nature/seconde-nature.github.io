---
title: Services
layout: home
description: "Services"
---
<h1 style="text-align: center;">Nous proposons également des services avec l'aide de nos bénévoles</h1>

<div class="row">
  {% for hi in site.data.services %}
  <div class="col-sm-4">
    <div class="card">
      <img src="{{ hi.image }}" style="width: 10rem;" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">{{ hi.name }}</h5>
        <p class="card-text">{{ hi.description }}</p>
        <a href="{{ hi.link }}" class="btn btn-primary">{{ hi.link_note }}</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>