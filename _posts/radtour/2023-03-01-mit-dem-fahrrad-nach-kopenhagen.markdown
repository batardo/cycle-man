---
redirect_from: 
- "blog/mit-dem-fahrrad-nach-kopenhagen.html"
layout: default
title: Mit dem Fahrrad von Berlin nach Kopenhagen - Die 4 Etappen
description: Von Berlin nach Kopenhagen mit dem Rad, eine tolle Radtour über die Mecklenburgische Seen Route, perfekt für lange Wochenende.
category: [radtour]
placement: [home]
lang: de
dep: Berlin
arr: Kopenhagen
last_modified_at: 19.03.2023
img: /img/berlin-copenhague/step4_b.png
footer: top2
---

<div class="container blog">
<div id="spacer"></div>
Artikel zuletzt am {{ page.last_modified_at | date: "%d-%m-%Y" }} aktualisiert<br/>
<div class="col-sm-12">
<div class="row">
      <h1>Mit dem Rad von Berlin nach Kopenhagen in 4 Tagen</h1>
      <a href="https://www.komoot.com/tour/62695337/zoom" target="_blank">
<img src="/img/berlin-copenhague/route-berlin-rostock-copenhague.jpg" width="80%" class="center"></a>
</div>
</div>
<div class="col-sm-12">
<div class="row">
<p>Ein paar Daten über meine Fahrradroute:</p>
<ul>
      <li id="plan">Distanz: 465 km</li>
      <li id="plan">Dauer: 4 Tage, 3 Nächte</li>
      <li id="plan">Strassenzustand: Sehr gut</li>
      <li id="plan">Route für Rennräder geeignet: Ja</li>
      <li id="plan">Aufstieg: ca. 1600 m</li>
      <li id="plan">Abstieg: ca. 1600 m</li>
      <li id="plan">Unterkunft: 3 Nächte (Camping, Privat, Hotel) = Budget ca. 100€ </li>
      <li id="plan">Fahrkarten: Fähre rostock-Gedser + Nachtbus Kopenhagen-Berlin = Budget ca. 150€</li>
      <li id="plan">Budget insgesamt ca. 250€ ohne Verpflegung</li>
</ul>
      <p>Im Durchschnitt bin ich um die 100 Kilometer pro Tag gefahren. Wer mehr Zeit hat, kann auch über die
<a href="https://de.eurovelo.com/ev7/germany"> EuroVelo 7 Fahrradstraße </a> fahren. Etwa 200 Kilometer länger, dafür 
wahrscheinlich noch schöner und vor allem besser für Fahrräder geeignet. Ansonsten hier sind meine<a href="#etapes"> 
4 Etappen von Berlin nach Kopenhagen</a>.</p></div>
  </div>    
  </div>

<div class="container blog">
  <h2 id="etapes">EuroVelo 7 von Berlin nach Kopenhagen : meine 4 Etappen</h2>
  {% assign posts=site.posts | where:"lang", page.lang %}
    {% for post in posts %}
      {% if post.trip == 'berlin-copenhague' %}

<div class="row vcenter">

<div class="col-sm-5">
  <a href="{{ post.map_url }}"><img src="{{ post.img }}" alt="{{ post.img_name }}" class="img responsive img-rounded"></a>
  
  </div>

<div class="col-sm-7">
    <p id="post_title">Von {{post.from}} nach {{post.to}}</p>
      {{ post.description }}<br/>
      {% include share-bar-de.html %} <br/>
      Distanz : {{ post.distance }} km<br/>
      Schwierigkeit : {{ post.rating_difficulty }}/5<br/>
      Aufstieg : {{ post.up }} m<br/>
      Abstieg : {{ post.down }} m<br/>
      {% if post.accomodation_url  %}
      Unterkunft : <a href="{{ post.accomodation_url }}" target="_blank">{{ post.accomodation_name }}</a>
      {% else %}
      Unterkunft : {{ post.accomodation_name }}
      {% endif %}
</div>
</div>

<div id="spacer"></div>

  {% endif %}
  {% endfor %}

{% include btn-back-de.html %}
</div>

