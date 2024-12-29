---
title: LeBonZaap
publishDate: 2024-12-29 00:00:00
img: /assets/Main-page-offer.png
img_alt: Page d'accueil des offres
class: zoomable
description: |
  Développement d'une plateforme d'échange de service pour jeux vidéos.
tags:
  - Java / Spring Boot
  - React
  - Docker
  - PostgreSQL
  - Liquibase
---

# <a href="https://github.com/Blustery33/LeBonZaapDemo" target="_blank">LeBonZaap</a>

LeBonZaap est une plateforme d’échange de services dédiée aux joueurs d’un même jeu vidéo.</br></br>
L’application permet aux utilisateurs de publier des offres et de proposer des services qu’ils souhaitent vendre, 
en lien avec leur jeu préféré. Que ce soit pour des échanges d’objets virtuels, de l’entraide en jeu, ou des prestations personnalisées, LeBonZaap facilite la mise en relation entre joueurs passionnés.

&nbsp;

### Un projet en Pair programming

<p style="font-size: 22px;"><strong>Travailler en duo sur ce projet m’a permis de :</strong></p>

- **Améliorer mes compétences techniques** en collaborant sur GitHub pour la gestion du code et des versions.  
  <br>
- **Développer une meilleure organisation** en suivant l’avancement des tâches via Trello et en adoptant une approche agile.  
  <br>
- **Renforcer ma capacité à communiquer et résoudre des problèmes**, en partageant des idées et en codant à deux en temps réel.
  <br>
  <br>
<p>Les images ci-dessous montrent notre processus : dépôt GitHub collaboratif, tableau Trello et aperçus de l’application en développement.
  <br>
Ce projet reflète non seulement mes compétences techniques, mais aussi ma capacité à travailler efficacement 
en équipe et à apprendre en continu dans un environnement collaboratif.</p>

&nbsp;
&nbsp;

<div class="container">
<div>
<img src="/assets/trello-lebonzaap.png" id="image" alt="trello" class="zoomable">
<div style="text-align: center"><span><strong>Trello</strong></span></div>
</div>
</div>

&nbsp;
&nbsp;

<div class="container">
<div>
<img src="/assets/github-lebonzaap.png" id="image" alt="github" class="zoomable">
<p style="text-align: center"><a href="https://github.com/Blustery33/LeBonZaapDemo" target="_blank"><span><strong>Github</strong></span></a></p>
</div>
</div>

&nbsp;
&nbsp;

<div class="container">
<div>
<img src="/assets/offer-service.png" id="image" alt="service offre" class="zoomable">
<div style="text-align: center"><span><strong>Morceau de code du service implémentation des offres</strong></span></div>
</div>
</div>

&nbsp;

### Maquette de l'application
Pour concevoir l’interface de l’application **LeBonZaap**, nous avons utilisé **Figma**. 
Cet outil de design collaboratif nous a permis de créer des maquettes interactives et de visualiser chaque écran avant de passer au développement.
<br>
<br>
L’image ci-dessous présente un aperçu de la maquette réalisée.

&nbsp;
&nbsp;

<div class="container">
<div>
<img src="/assets/figma-lebonzaap.png" id="image" alt="figma lebonzaap" class="zoomable">
<div style="text-align: center"><span><strong>Figma</strong></span></div>
</div>
</div>

&nbsp;

### Test d'intégration
Pour garantir la **stabilité et le bon fonctionnement** de l’application **LeBonZaap**, j'ai réalisé des **tests d’intégration**. Ces tests m'ont permis de vérifier que les différentes fonctionnalités s’assemblent correctement et communiquent sans erreur.
<br>
<br>
L’image ci-dessous illustre une phase de **test** effectuée durant le développement.

&nbsp;
&nbsp;

<div class="container">
<div>
<img src="/assets/test-lebonzaap.png" id="image" alt="test d'intégration création d'une offre" class="zoomable">
<div style="text-align: center"><span><strong>Test d'intégration pour la création d'une offre</strong></span></div>
</div>
</div>

&nbsp;

#### Technologies utilisées

- Java
- Spring Boot
- Docker
- PostgreSQL
- Liquibase
- GitHub
- Figma

<style>
.container {
  position: relative;
}

.zoomable {
  width: 100%;
  height: auto;
  cursor: pointer;
}

.zoomable:hover {
  transform: scale(1.1); /* Changer le facteur d'agrandissement */
}

.zoomable.zoomed {
  transform: scale(1.7); /* Changer le facteur d'agrandissement */
  z-index: 9999;
}

</style>
<script>
document.addEventListener('DOMContentLoaded', function () {
  const zoomableImages = document.querySelectorAll('.zoomable');

  zoomableImages.forEach(image => {
    image.addEventListener('click', function () {
      if (!this.classList.contains('zoomed')) {
        this.classList.add('zoomed');
      } else {
        this.classList.remove('zoomed');
      }
    });
  });

  
  document.addEventListener('click', function (event) {
    
    if (!event.target.closest('.zoomed')) {
      zoomableImages.forEach(image => {
        image.classList.remove('zoomed');
      });
    }
  });
});

</script>
