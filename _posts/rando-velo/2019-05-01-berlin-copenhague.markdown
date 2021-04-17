---
layout: default
title: En vélo de Berlin à Copenhague en 4 jours
description: "Un bout d'EuroVélo 7 de Berlin à Cophenhague, la randonnée vélo des lacs du Mecklembourg et de la mer baltique. Idéal pour un long week-end prolongé de 4 jours. Compte-rendu."
category: 'rando-velo'
lang: 'fr'
dep: Berlin
arr: Copenhague
tags: [ Allemagne, Danemark ]
last_modified_at: 01.05.2019
comments: true
img: /Images/berlin-copenhague/step4_b.png
---

<div class="container blog">
  <div class="row">
      <h1>Quel voyage à vélo faire en 4 jours au départ de Berlin ?</h1>
      Mis à jour le {{ page.last_modified_at | date: "%d-%m-%Y" }}<br/>
      <p>Ils avaient prévu du beau temps pour ce long week-end d'avril, parfait pour une rando à vélo. L’an dernier j’avais fait la partie sud de <a href="/rando-velo/berlin-prague.html">l’EuroVélo 7 de Berlin à Prague</a>, du coup cette année je me suis lancé vers le nord sur un Berlin-Copenhague. Un itinéraire que je recommande.</p>
      <h2>L’itinéraire vélo de Berlin à Copenhague</h2>
        <div class="col-sm-6">
      <p>Et voilà mon itinéraire. On est en moyenne sur du 100 kilomètres par jour. À noter que si vous avez plus de 4 jours, vous pouvez suivre l'itinéraire officiel de <a href="http://www.eurovelo.com/fr/eurovelos/eurovelo-7/pays/allemagne-1/berlin/veloroute-berlin-copenhague"> l'eurovélo 7</a>. Plus long d'à peu près 200 kilomètres mais certainement plus adapté pour du cyclotourisme. Sinon il y a mon itinéraire dont voici le détail des <a href="#etapes">4 étapes</a>.</p></div>
      <div class="col-sm-6">
      <iframe src="https://www.komoot.com/tour/62695337/embed?profile=1" width="100%" height="400" frameborder="0" scrolling="no"></iframe>
    </div>
      
  </div>
</div>

<div class="container blog">
  <h2 id="etapes">Eurovélo 7 de Berlin à Copenhague : mes 4 étapes</h2>
  {% assign posts=site.posts | where:"lang", page.lang %}
    {% for post in posts %}
      {% if post.trip == 'berlin-copenhague' %}

<div class="row vcenter">

<div class="col-sm-5">
  <a href="{{ post.map_url }}"><img src="{{ post.img }}" alt="{{ post.img_name }}" class="img responsive img-rounded"></a>
  
  </div>

<div class="col-sm-7">
    <p id="post_title">De {{post.from}} à {{post.to}}</p>
      {{ post.description }}<br/>
      {% include share-bar-fr.html %} <br/>
      Distance : {{ post.distance }} km<br/>
      Difficulté : {{ post.rating_difficulty }}/5<br/>
      Dénivelé positif : {{ post.up }} m<br/>
      Dénivelé négatif : {{ post.down }} m<br/>
      {% if post.accomodation_url  %}
      Hébergement : <a href="{{ post.accomodation_url }}" target="_blank">{{ post.accomodation_name }}</a>
      {% else %}
      Hébergement : {{ post.accomodation_name }}
      {% endif %}
</div>
</div>

<div id="spacer">
</div>

  {% endif %}
  {% endfor %}

<h3>La navigation komoot, une première</h3>
<p>Habitué aux bips et douces sonorités du Garmin Touring Plus, je me suis fait guidé pour cette randonnée par la voie métallique de l’application Komoot, une première. Sur cette application, j’avais tracé mon itinéraire et téléchargé la carte offline avant mon départ de manière à  ne pas utiliser de données. Il faut payer pour cela une fois 29€ permettant d’accéder à toutes les cartes. Et franchement le résultat est bon. Les indications sont claires et précises, évidemment il y toujours quelques incompréhensions homme/GPS, qu’il y a d’ailleurs aussi avec le Garmin, mais elles sont rares. J’ai donc pu me concentrer sur la route, sans presque jamais m’arrêter pour regarder la carte. Du grand confort.</p>

{% include btn-back-fr.html %}
</div>
