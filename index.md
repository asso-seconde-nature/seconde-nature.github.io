---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h1 style="text-align: center;">Notre Seconde Nature, c'est Réemployer, Réparer et Réutiliser !</h1>
<h2 style="text-align: center;" class="text-danger">!! Ouverture le Samedi 14/06 à 10H00 !!</h2>


<div class="row">
    <div class="col d-flex justify-content-center">
            <div class="embed-responsive embed-responsive-16by9">
              <iframe class="embed-responsive-item" width="800" height="450" src="/assets/img/france3.mp4" frameborder="0" allowfullscreen=""></iframe>
            </div>
    </div>
</div>

<h2 class="text-primary" style="text-align: center;">Nos objectifs</h2>

<h3 style="text-align: center;"><span class="badge bg-success">Sensibiliser</span>les citoyen·nes à la réduction des déchets par le réemploi.</h3>
<h3 style="text-align: center;"><span class="badge bg-success">Encourager</span>une consommation plus raisonnable afin de préserver l’environnement.</h3>
<h3 style="text-align: center;"><span class="badge bg-success">Innover</span>dans le ré-emploi avec des technologies ouvertes et durables.</h3>

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
  