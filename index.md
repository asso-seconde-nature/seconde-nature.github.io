---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h1 style="text-align: center;">Notre Seconde Nature, c'est Réemployer, Réparer et Réutiliser !</h1>
<h2 style="text-align: center;" class="text-danger">!! Ouverture prochainement !!</h2>
<h2 class="text-primary" style="text-align: center;">Nos objectifs</h2>

<h4 style="text-align: center;">* Sensibiliser les citoyen·nes à la réduction des déchets par le réemploi.</h4>
<h4 style="text-align: center;">* Encourager une consommation plus raisonnable afin de préserver l’environnement.</h4>

<h2 class="text-primary" style="text-align: center;">Nos missions</h2>

<div class="row">
  {% for hi in site.data.missions %}
  <div class="col-sm-3">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">{{ hi.name }}</h5>
        <p class="card-text">{{ hi.description }}</p>
      </div>
      <p class="text-center">
          <a href="{{ hi.link }}" target="_blank" class="btn btn-primary">{{ hi.link_note }}</a>
        </p>
    </div>
  </div>
  {% endfor %}
</div>
  