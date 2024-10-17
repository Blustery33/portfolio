---
title: Docker-project
publishDate: 2024-04-23 00:00:00
img: /assets/docker-compose-dev.png
img_alt: docker-project
class: zoomable
description: | 
  Mise en place complète d'un environnement Docker
tags:
  - Docker
  - React
  - Nginx
  - MongoDb
---
Lien vers le repo Github :
## <a href="https://github.com/Blustery33/docker-production" target="_blank">Docker-project</a>
&nbsp;

Docker-project est une base complète pour une nouvelle application dans un environnement <strong>Docker</strong>.

[//]: # (Leur donnée utilisateur est remplie en ligne par les conseillers d’admission, qui appellent les prospects afin de clôturer des ventes. )

[//]: # (Il gère aussi le paiement en ligne, la comptabilité et toutes les statistiques de vente  &#40;autofinancement, CPF, rétractation, etc&#41;. )

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/docker-compose-dev.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>docker-compose.dev.yml</span></div>
</div>

&nbsp;
&nbsp;

### Résumé

L’objectif de ce mini-projet était de me former à <strong>Docker</strong>. J’ai donc mis en place un environnement complet qui peut servir de base à une application <strong>React</strong>.



<br>
<br>


Ci-dessous, l'architecture de l'application est séparée en quatre dossiers distincts, chaque dossier correspondant à un conteneur <strong>Docker</strong>.
<div class="container">
</div>
<div class="margin-ul">

- <strong>Api</strong> : container Nodejs qui gère la connexion à la base de donnée et toutes les url /api
- <strong>Client</strong> : container React qui gère tout le front de l'application
- <strong>Db</strong> : container qui gère les variables d'environnement liés à la base de donnée
- <strong>Reverse-proxy</strong> : container qui va se charger uniquement de répartir les requêtes entrantes entre les différents services

</div>

&nbsp;
&nbsp;
<div class="container">
<img src="/assets/architecture-docker.png" id="image" alt="image" class="zoomable">
<div style="text-align: center"><span>Architecture complète du mini-projet</span></div>
</div>

&nbsp;
&nbsp;

#### Technologies utilisées

- Docker
- Nodejs
- React
- Nginx
- Github


<br>
<br>

[//]: # (<div class="container">)

[//]: # (<img src="/assets/loic-dyma.png" id="image" alt="image" class="zoomable">)

[//]: # (<div style="text-align: center"><span>Profil d'un autre utilisateur, possibilité de follow/unfollow</span></div>)

[//]: # (</div>)

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
