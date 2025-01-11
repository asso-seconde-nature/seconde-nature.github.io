---
title: Equipe
layout: home
description: "L'équipe"
---
<h1 style="text-align: center;">Nouveau bureau, Nouveaux projets</h1>

<div class="container">
L'association fête ses 10 ans et voit arriver de nouveaux membres du bureau pour donner une nouvelle jeunesse à ce beau projet.
Une assemblée générale a eu lieu le 09/12/2024 et a élu une nouvelle équipe porteur de projets pour péréniser et developper les activités de l'association.
</div>
<br>
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