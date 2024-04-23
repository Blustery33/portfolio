---
title: Dyma-moutmout
publishDate: 2024-04-23 00:00:00
img: /assets/accueil-dyma.png
img_alt: dyma-moutmout
class: zoomable
description: | 
  Developpement d'une application similaire à twitter pour apprendre Node.js / Express
tags:
  - Node JS
  - Express
  - Socket.io
---

## <a href="https://dyma-moutmout.fr" target="_blank">Dyma-moutmout</a>
&nbsp;

Est une application que j'ai développé en Node.js sous le framework Express.
Elle reprend les grands principes de twitter

[//]: # (Leur donnée utilisateur est remplie en ligne par les conseillers d’admission, qui appellent les prospects afin de clôturer des ventes. )

[//]: # (Il gère aussi le paiement en ligne, la comptabilité et toutes les statistiques de vente  &#40;autofinancement, CPF, rétractation, etc&#41;. )

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/chat-dyma.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Chat (socket.io)</span></div>
</div>

&nbsp;
&nbsp;

### Résumer

L’objectif de ce projet était de me former en Node.js. J'ai donc mis en place beaucoup de fonctionnalités pour apprendre
et m'entraîner avec comme mission faire une application twitter.

<div class="container">
</div>
J'ai pu donc mettre en place, l'authentification avec JWT. Socket.io pour le chat. Nodemailer pour le mot de passe oublié
et l'activation du compte pour avoir le status "vérifié". Multer pour l'upload d'image de profil etc.

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/mdp-dyma.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Réinitialisation de mot de passe avec nodemailer et sweetalert2</span></div>
</div>

&nbsp;
&nbsp;

#### Technologies utilisées

- Html/Css/Pug
- Javascript
- Express
- MongoDb
- Github

#### Packages utilisés
  |  |  |   |
  |----------------|----------------|---|
 - Socket.io &nbsp;&nbsp;/&nbsp;&nbsp; Nodemailer
 - Bcrypt &nbsp;&nbsp;/&nbsp;&nbsp; Jwt
 - Mongoose &nbsp;&nbsp;/&nbsp;&nbsp; Multer
 - uuid &nbsp;&nbsp;/&nbsp;&nbsp; errorhandler
 - moment &nbsp;&nbsp;/&nbsp;&nbsp; sweetalert2 
</br>
</br>

<div class="container">
<img src="/assets/loic-dyma.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Profil d'un autre utilisateur, possibilité de follow/unfollow</span></div>
</div>

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
