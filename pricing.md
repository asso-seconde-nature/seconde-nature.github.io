---
layout: home
title: Seconde Nature
description: Economie sociale et solidaire, Insertion, seconde main.
---
<h2 style="text-align: center;" class="text-danger">CONDITIONS GENERALES DE VENTE</h2>

Ces conditions s’appliquent dans leur intégralité pour toute personne effectuant
un achat au sein de la recyclerie Seconde Nature. Merci d’en prendre connaissance.
La vente des objets a pour objectif d'offrir une deuxième vie aux objets.
Nous avons à cœur de vous présenter un espace de vente agréable et organisé en rayons.
Nos approvisionnements dépendent des collectes et des apports et par conséquent l’offre de produits change toutes les semaines.

<h2 style="text-align: center;">Prix</h2>

La politique de prix est décidé par le bureau et peut être revue tous les ans.

<table class="table table-striped table-bordered">
  <thead>
    <tr>
      <th scope="col">Rayon</th>
      <th scope="col">Article</th>
      <th scope="col">Unité de vente</th>
      <th scope="col">Prix</th>
    </tr>
  </thead>
  <tbody>
    {% for hi in site.data.pricing %}
      <tr class="table-{{ hi.status }}">
        <th scope="row">{{ hi.category }}</th>
        <td>{{ hi.article }}</td>
        <td>{{ hi.unity }}</td>
        <td>{{ hi.value }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

Les prix affichés sont <span class="badge bg-warning">non négociable</span>

<h2 style="text-align: center;">Garantie</h2>

Les produits sont vendus en l’état <span class="badge bg-warning">sans garantie commerciale</span>. Les retours sont acceptés
uniquement pour les équipements électriques et électroniques en cas de panne matérielle, dans un délai de 1 semaine sur présentation du ticket de caisse. Un avoir, valable 3 mois est remis au client.

<h2 style="text-align: center;">Paiement</h2>

Le paiement se fait en <span class="badge bg-success">espèces</span>, par <span class="badge bg-success">virement instantanné</span> ou par <span class="badge bg-success">carte bancaire</span>.
Nous n'acceptons pas les paiements par <span class="badge bg-danger">chéque</span>

En cas d’achat à retrait différé, le paiement se fait à la caisse du magasin et le retrait sur
le quai de déchargement après avoir justifié du paiement. Les achats en attente d’être
retirés seront remis en vente sans aucun remboursement dans un délai d’une semaine.

<h2 style="text-align: center;">Livraison</h2>

La livraison est <span class="badge bg-warning">payante</span> et comprend le kilométrage et le temps de travail. Elle inclue le
chargement, le trajet puis le déchargement à domicile.
Le responsable de la livraison <span class="badge bg-warning">pourra refuser</span> toute livraison s’il estime que les conditions de
<span class="badge bg-warning">sécurité</span> ne sont pas satisfaisantes comme par exemple de trop lourdes charges à livrer
dans un lieu sans ascenseur ou bien un accès véhicule limité qui nécessite trop de
portage.