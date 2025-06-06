---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseZero" aria-expanded="false" aria-controls="collapseZero">
        Qui participe à cette association ?
      </button>
    </h2>
    <div id="collapseZero" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="row">
        {% for hi in site.data.infos %}
          <div class="col-sm-2 mb-2 mb-sm-0">
              <div class="card shadow-sm" style="width: 14rem;">
                  <img src="{{ hi.image }}" class="card-img-top" alt="">
                  <div class="card-body">
                      <h5 class="card-title">{{ hi.name }}</h5>
                      <p class="card-text">{{ hi.content }}</p>
                      {% for keyword in hi.keywords %}
                        <span class="badge bg-secondary">{{ keyword }}</span>
                      {% endfor %}
                      {% for domain in hi.domains %}
                        <span class="badge bg-info">{{ domain }}</span>
                      {% endfor %}
                  </div>
              </div>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
        Peux t on consulter les documents de l'association ?
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <p class="text-center">
          <a href="/assets/doc/charte_benevoles.pdf" target="_blank" class="btn btn-info">Charte des bénévoles</a>
        </p>
        <p class="text-center">
          <a href="/assets/doc/reglement_interieur.pdf" target="_blank" class="btn btn-info">Réglement intérieur</a>
        </p>
        <p class="text-center">
          <a href="/assets/doc/statuts.pdf" target="_blank" class="btn btn-info">Statuts</a>
        </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        Comment venir ?
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        La recyclerie est situé au 8 rue du bouil bleu 17250 SAINT-PORCHAIRE.
        <div class="col d-flex justify-content-center">
              <iframe class="embed-responsive-item"  width="100%" height="600px" frameborder="0" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/fr/map/seconde-nature_1163837?scaleControl=true&miniMap=true&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#19/45.82805/-0.78452"></iframe>
        </div>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Comment nous contacter ?
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        Envoyez nous un email
        <p class="text-center">
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[CONTACT]" target="_blank" class="btn btn-primary">Contact</a>
        </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
        Quelles sont les horaires d'ouvertures ?
      </button>
    </h2>
    <div id="collapseFour" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        La recyclerie est ouverte selon la disponibilité des bénévoles, les horaires sont ci-dessous
        <p class="text-center">
          <a href="{{ "/infos" | relative_url}}" class="btn btn-primary">Horaires</a>
        </p>
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFive" aria-expanded="false" aria-controls="collapseFive">
        Peux t on apporter des objets ?
      </button>
    </h2>
    <div id="collapseFive" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <span class="badge bg-success">Oui</span>, pour apporter des objets, il faut être <a href="{{ "/adherents" | relative_url}}">adhérent</a>, vérifier que vos objets correspondent à la <a href="{{ "/collected_items" | relative_url}}">liste des objets autorisés</a> puis prendre rendez vous en nous envoyant un email (asso.seconde.nature@gmail.com).
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSix" aria-expanded="false" aria-controls="collapseSix">
        Faites vous des vide-maisons ? Venez vous à domicile pour collecter des objets ?
      </button>
    </h2>
    <div id="collapseSix" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <span class="badge bg-danger">Non</span>, nous ne faisons pas de vide-maison pour le moment.
      </div>
    </div>
  </div>
</div>