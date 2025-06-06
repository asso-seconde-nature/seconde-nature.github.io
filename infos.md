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