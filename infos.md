---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h2 style="text-align: center;" class="text-danger">Ouverture prévue prochainement</h2>
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

<h2 style="text-align: center;">Bureau</h2>

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

<h2 style="text-align: center;">Nous contacter</h2>

  <div>
        <p class="text-center">
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[BENEVOLAT]" target="_blank" class="btn btn-primary">Je deviens bénévole</a>
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[DONS]" target="_blank" class="btn btn-primary">Je donne des objets</a>
        </p>
      </div>