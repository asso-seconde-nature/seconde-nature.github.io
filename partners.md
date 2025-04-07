---
title: Partenaires
layout: home
description: "Partenaires"
---
<h1 style="text-align: center;">Merci à tous nos partenaires qui soutiennent ce projet</h1>

<div class="row">
  {% for hi in site.data.partners %}
  <div class="col-sm-4">
    <div class="card">
      <img src="{{ hi.image }}" style="width: 10rem;max-height: 180px;width: 100%;object-fit: contain" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">{{ hi.name }}</h5>
        <p class="card-text">{{ hi.description }}</p>
        <a href="{{ hi.link }}" target='_blank' class="btn btn-primary">{{ hi.link_note }}</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>

  <br>
  <div>
        <p class="text-center">
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[PARTENAIRE]" target="_blank" class="btn btn-primary">Devenez partenaire !</a>        
        </p>
  </div>