---
title: Equipe
layout: home
description: "L'équipe"
---
<h1 style="text-align: center;">Nouveau bureau, Nouveaux projets</h1>

<div class="container">
L'association vient d'être créer pour developper l'économie sociale et solidaire au sein du site de La Vauzelle.
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