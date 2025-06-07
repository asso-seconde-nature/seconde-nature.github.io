---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h2 style="text-align: center;">Collecte</h2>

La recyclerie procède à des collecte auprès de ses partenaires locaux pour récupérer des objets jetés, inutilisés ou invendus.

<h2 style="text-align: center;">Apport volontaire</h2>

Seul les <span class="badge bg-warning">adhérents</span> peuvent apporter des objets.

La politique de apport et de collecte est <span class="badge bg-warning">décidé par le bureau</span> et peut être revue tous les ans.

Les objets doivent être fonctionnels et en bon état d’utilisation, propres et à l’usure modérée.

Les objets peuvent être <span class="badge bg-success">accepté</span>, <span class="badge bg-warning">accepté avec conditions</span> ou <span class="badge bg-danger">refusé</span>.
Le responsable des apports peut refuser un article selon l'<span class="badge bg-warning">état</span>  (hors d’usage, cassés, sales, usure avancée…) de l'article même si il apparait autorisé dans le tableau ci-dessous.

<table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th scope="col">Rayon</th>
      <th scope="col">Article</th>
      <th scope="col">Commentaire</th>
    </tr>
  </thead>
  <tbody>
    {% for hi in site.data.collected_items %}
      <tr class="table-{{ hi.status }}">
        <th scope="row">{{ hi.category }}</th>
        <td>{{ hi.article }}</td>
        <td>{{ hi.comment }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>