---
title: Bogy CRM ( Gestion utilisateur )
publishDate: 2024-02-15 00:00:00
img: /assets/crm-gestion-utilisateur.png
img_alt: une gestion utilisateur dans un crm
class: zoomable
description: | 
  J'ai développé une interface de gestion d'utilisateur complètement dynamique.
tags:
  - Symfony
  - Bundle
  - Live component
---

## Bogy CRM entreprise
&nbsp;

> Bogy

BOGY est une interface de gestion d’élèves qui concerne l’avancement de leur formation sur la plateforme d’apprentissage. Leur donnée utilisateur est remplie en ligne par les conseillers d’admission, qui appellent les prospects afin de clôturer des ventes. Il gère aussi le paiement en ligne, la comptabilité et toutes les statistiques de vente  (autofinancement, CPF, rétractation, etc). 

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/photo-bogy-1.png" id="image" alt="image" class="zoomable">
</div>

&nbsp;
&nbsp;

### Mission

L’objectif de ce projet était de refondre toute l’application interne de l’entreprise en une version 2.0. Pour cela, il était nécessaire d’améliorer toutes les fonctionnalités déjà existantes. L’objectif final était de parfaire l’utilisation de l’application par les collaborateurs.

Afin d’atteindre cette mission, j’étais en charge de la création d’une interface dynamique de gestion des utilisateurs. Le but de cette interface était de rendre possible la modification des informations des utilisateurs, d’activer ou désactiver leur compte et de pouvoir assigner des formations précises à la personne.

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/photo-bogy-2.png" id="image" alt="image" class="zoomable">
</div>

&nbsp;
&nbsp;

#### Technologies utilisées

- Html/Css
- Javascript
- Symfony
- Php
- Bundle Live Component
- Twig
- MySQL
- GitLab

[//]: # (- We noted this)

[//]: # (- And also this other point)
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
