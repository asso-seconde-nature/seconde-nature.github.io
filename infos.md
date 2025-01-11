---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h1 style="text-align: center;">Infos pratiques</h1>
<h2 style="text-align: center;" class="text-danger">Ouverture prévue prochainement</h2>
<h2 style="text-align: center;">Horaires hebdomadaires</h2>
<table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th scope="col">Jour</th>
      <th scope="col">Horaires</th>
    </tr>
  </thead>
  <tbody>
    {% for hi in site.data.horaires %}
      <tr class="table-{{ hi.status }}">
        <th scope="row">{{ hi.name }}</th>
        <td>{{ hi.horaires }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

<h2 style="text-align: center;">Nous contacter</h2>

  <div>
        <p class="text-center">
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[BENEVOLAT]" target="_blank" class="btn btn-primary">Je deviens bénévole</a>
          <a href="mailto:asso.seconde.nature@gmail.com?subject=[DONS]" target="_blank" class="btn btn-primary">Je donne des objets</a>
        </p>
      </div>