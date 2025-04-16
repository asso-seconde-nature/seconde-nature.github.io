---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h2 style="text-align: center;" class="text-danger">Ouverture le Samedi 14/06 à 10H00</h2>
<h2 style="text-align: center;">Horaires hebdomadaires</h2>
<table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th scope="col">Jour</th>
      <th scope="col">Horaires Recyclerie</th>
      <th scope="col">Horaires Réparation</th>
    </tr>
  </thead>
  <tbody>
    {% for hi in site.data.horaires %}
      <tr class="table-{{ hi.status }}">
        <th scope="row">{{ hi.name }}</th>
        <td>{{ hi.horaires }}</td>
        <td>{{ hi.horaires_repair }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

<div class="row">
  <div class="col d-flex justify-content-center">
    <iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=2&ctz=Europe%2FZurich&showDate=0&showPrint=0&showCalendars=0&showTz=0&showTitle=0&src=NDQzMDBmZDg3ODcxMTM0YjM5ZTc5NTNkZDhkMTBjMzEyYmY5NTViNjllYmNkZTg1NGYwOGExYzYxYTJmZjg3YkBncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23A79B8E" style="border-width:0" width="100%" height="600" frameborder="0" scrolling="no"></iframe>
  </div>
</div>

<h2 style="text-align: center;">Le bureau</h2>

<div class="row">
    {% for hi in site.data.infos %}
    <div class="col-sm-2 mb-2 mb-sm-0">
        <div class="card shadow-sm" style="width: 14rem;">
            <img src="{{ hi.image }}" class="card-img-top" alt="">
            <div class="card-body">
                <h5 class="card-title">{{ hi.name }}</h5>
                <p class="card-text">{{ hi.content }}</p>
            </div>
        </div>
    </div>
    {% endfor %}
</div>

<h2 style="text-align: center;">Les documents de l'asso</h2>

  <div class="row">
      <div class="col-sm-2 mb-2 mb-sm-0">
        <p class="text-center">
          <a href="/assets/doc/statuts.pdf" target="_blank" class="btn btn-info">Statuts</a>
        </p>
      </div>
       <div class="col-sm-2 mb-2 mb-sm-0">
        <p class="text-center">
          <a href="/assets/doc/reglement_interieur.pdf" target="_blank" class="btn btn-info">Réglement intérieur</a>
        </p>
      </div>
      <div class="col-sm-2 mb-2 mb-sm-0">
        <p class="text-center">
          <a href="/assets/doc/charte_benevoles.pdf" target="_blank" class="btn btn-info">Charte des bénévoles</a>
        </p>
      </div>
  </div>

<h2 style="text-align: center;">Venir à la recyclerie ( 8 rue du bouil bleu 17250 SAINT-PORCHAIRE )</h2>
<div class="row">
    <div class="col d-flex justify-content-center">
              <iframe class="embed-responsive-item"  width="100%" height="600px" frameborder="0" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/fr/map/seconde-nature_1163837?scaleControl=true&miniMap=true&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#19/45.82805/-0.78452"></iframe>
               </div>
  </div>

<h2 style="text-align: center;">Nous contacter</h2>
  <div>
        <p class="text-center">
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[CONTACT]" target="_blank" class="btn btn-primary">Contact</a>
        </p>
      </div>