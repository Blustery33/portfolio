---
title: Tennis rankings API
publishDate: 2024-10-16 00:00:00
img: /assets/api-accueil-java.png
img_alt: api-java-tennis
class: zoomable
description: | 
  Développement d'une Api de classement de joueur de tennis
tags:
  - Java
  - Spring Boot
  - Api
---

## Tennis rankings API
&nbsp;

Tennis Rankings API est une application que j'ai développée en <strong>Java</strong> avec le framework <strong>Spring Boot</strong>. 
Elle permet de gérer et de consulter le classement des joueurs de tennis, en respectant les principes des <strong>API REST</strong>.

[//]: # (Leur donnée utilisateur est remplie en ligne par les conseillers d’admission, qui appellent les prospects afin de clôturer des ventes. )

[//]: # (Il gère aussi le paiement en ligne, la comptabilité et toutes les statistiques de vente  &#40;autofinancement, CPF, rétractation, etc&#41;. )

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/tennis-players.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Liste des joueurs</span></div>
</div>

&nbsp;
&nbsp;

### Résumé

L'application Tennis Rankings API permet de gérer et de consulter le classement des joueurs de tennis via une <strong>API REST</strong>.
Elle offre des fonctionnalités comme l'<strong>ajout</strong>, la <strong>mise à jour</strong> et la <strong>suppression</strong> de joueurs, ainsi que la gestion de leurs scores et un reclassement automatique.  
Le backend est développé en Java avec Spring Boot, offrant ainsi une architecture robuste et extensible, tout en respectant les bonnes pratiques REST pour des interactions efficaces avec les clients.

<div class="container">
</div>

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/tennis-find-player.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Chercher un joueur par son nom de famille</span></div>
</div>

&nbsp;
&nbsp;

#### Technologies utilisées

- Java
- Spring Boot
- Spring sécurity
- PostgreSQL
- Github

</br>

<div class="container">
<img src="/assets/tennis-connexion.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Url de connexion utilisateur</span></div>
</div>

[//]: # (- We noted this)

[//]: # (- And also this other point)
<style>
.margin-ul ul{
  width: 110%;
}
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
