---
layout: default
title: De Berlin à Dresde et Prague à vélo
description: "Rando vélo express de Berlin à Prague en passant par Dresde. 400 kilomètres en 4 jours, Suisse-saxonne, Suisse-bohémienne, Elbe. Idéal pour un long week-end. Retrouvez le détail des étapes."
category: 'rando-velo'
lang: 'fr'
dep: Berlin
arr: Prague
tags: [ Allemagne, République Tchèque ]
last_modified_at: 28.02.2019
comments: true
img: /Images/berlin-prague.jpg
---

<div class="container blog">
  <div class="row">
    <div class="col-sm-12">
      <h1>Randonnée à vélo de Berlin à Dresde et Prague</h1>
      Mis à jour le {{ page.last_modified_at | date: "%d-%m-%Y" }}<br/>
      <p>Voyage à vélo de <strong>400 kilomètres en 4 jours</strong>. Nous sommes partis <strong>avec une tente</strong>, nous avons passé trois nuits en camping. Le <strong>retour en bus</strong>. Voici ci-dessous le détail de nos 5 étapes : 3 jours complets et deux demie-journées.<br/> En résumé, c'était une super balade : <strong>Suisse saxonne, Suisse bohémienne, Elbe</strong>. De bonnes pistes cyclables coté allemand, un peu moins coté République Tchèque. Idéal pour un long week-end, ou une semaine si vous souhaitez visiter Dresde et Prague.</p>  
    </div>
  </div>
</div>

<div class="container blog">
  {% assign posts=site.posts | where:"lang", page.lang %}
    {% for post in posts %}
      {% if post.trip == 'berlin-prague' %}

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

{% include btn-back-fr.html %}
</div>
