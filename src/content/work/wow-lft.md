---
title: Wow Lft
publishDate: 2024-02-15 00:00:00
img: /assets/wowlft.png
img_alt: Gestionnaire de recrutement avec l'api world of warcraft.
class: zoomable
description: |
  Projet personnel Backend
tags:
  - Express JS
  - API
  - OAuth
---

> Wow Lft

Wow Lft est un mini projet personnel pour jouer avec l'api de world of warcraft. J'ai fait le choix d'utiliser
Express JS pour découvrir et apprendre ce framework back.

&nbsp;

Pour ce projet j'ai dû travailler avec l'authentification Oauth pour pouvoir donner à l'utilisateur la possibilité
de se connecter avec son compte World of warcraft

&nbsp;

<div class="container">
<img src="/assets/connexionOauth.png" id="image" alt="image" class="zoomable">
</div>

&nbsp;
&nbsp;

Une fois la connexion établie, j'avais accès à son profil en faisant appel à la première
url API pour récupérer toutes les autres url des personnages du compte. J'ai donc bouclé sur toutes les url dont j'avais besoin
pour récupérer certaines informations de chaque personnage et les enregistrer dans la base de données

&nbsp;
&nbsp;

<div class="container">
<img src="/assets/wow-url.png" id="image" alt="image" class="zoomable">
</div>

&nbsp;
&nbsp;

<strong>Pourquoi enregistrer les données en base de données ?</strong>
&nbsp;

Tout simplement pour éviter à chaque fois que l'utilisateur veut voir ses personnages de faire un appel API,
ce qui garantit grandement la vitesse de chargement. Car comme on le sait un appel API peut prendre plusieurs secondes avant de s'exécuter

&nbsp;
&nbsp;

<div class="container">
<img src="/assets/bdd-personnage.png" id="image" alt="image" class="zoomable">
</div>

#### Technologies utilisées

- Node JS
- Express JS
- Oauth
- MongoDB
- Api World of warcraft



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
