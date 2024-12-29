---
title: Application web de voyage
publishDate: 2024-02-15 00:00:00
img: /assets/authentictrip.png
img_alt: Gestionnaire de voyage
class: zoomable
description: |
  Projet d'école. Nous avons développé un assistant d'aide à la conception de séjours entièrement personnalisés.
tags:
  - Symfony
  - Voyage
  - Assistant
---

# <a class="h1-title" href="https://authentic-trip.fr/" target="_blank">Authentic Trip</a>

Authentic Trip est une marketplace agrégée d'un assistant d'aide à la conception de séjours entièrement personnalisés et authentiques. 
Destinés aux passionnés du terroir français souhaitant découvrir nos régions autrement. 
Nous regroupons à travers notre service, toute la qualité du savoir-faire en France, ainsi que tous ses trésors culturels et naturels.

&nbsp;

### Un assistant personnalisé

À travers un questionnaire, nous pouvons déterminer les envies de l'utilisateur afin de lui proposer l'expérience la plus adaptée.
3 points principaux sont traités :
- Le profil de l'utilisateur
- Ses habitudes de voyage
- Ce qu'il recherche en termes d'activités

Après avoir validé tous les points, l'assistant génère un carnet de séjours en fonction des choix.

&nbsp;

#### Technologies utilisées

- Html/Css
- Javascript
- Symfony
- Php
- Twig
- MySQL
- GitHub

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
@media (max-width: 320px) {
  .h1-title{
    font-size: 50px;
  }
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
