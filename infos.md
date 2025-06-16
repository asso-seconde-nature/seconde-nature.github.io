---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h2 style="text-align: center;">Horaires d'ouvertures (mis à jour régulièrement)</h2>
<div class="row">
  <div class="col d-flex justify-content-center">
    <iframe src="https://calendar.google.com/calendar/embed?height=800&wkst=2&ctz=Europe%2FZurich&showPrint=0&mode=WEEK&src=NDQzMDBmZDg3ODcxMTM0YjM5ZTc5NTNkZDhkMTBjMzEyYmY5NTViNjllYmNkZTg1NGYwOGExYzYxYTJmZjg3YkBncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%230b8043" style="border-width:0" width="100%" height="800" frameborder="0" scrolling="no"></iframe>
  </div>
</div>

<h2 style="text-align: center;">Horaires hebdomadaires théoriques (selon la disponibilité des bénévoles)</h2>
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