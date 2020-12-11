---
layout: post
title: "Température en météo"
# date:   2020-11-16 16:08:00 +0200
categories: Sciences
tags:
    - Météorologie
excerpt: \"Température ressentie 0°C\". Mais qu'est-ce vraiment le degré Celsius ? Comment mesure-t-on la température ? Et qu'est-ce que la température ressentie ?
image:
  path: /images/post-images/2020-12-10-temperature-meteo/main.jpg
  thumbnail: /images/post-images/2020-12-10-temperature-meteo/main-thumb-flat.jpg
  caption: "Photo par [Matthew Henry](https://unsplash.com/@matthewhenry)"
---

## Introduction

Il existe plusieurs échelles de température : degré Celsius, degré Fahrenheit, kelvin, etc. Mais d'où viennent-elles et quelles sont leurs différences ? D'ailleurs saviez-vous que l'eau ne bout pas à 100°C (à pression standard) ?

Savez-vous comment les services météo mesurent la température ?

Vous avez sans-doute déjà entendu parler la *température ressentie*, que ce soit dans les bulletins météos ou dans votre application sur smartphone. Mais que représente-t-elle ?

<!--
TODO :

* Attention, multiplication a du sens qu'en kelvin (vérifier)
* comment on mesure la température
* effet du vent, transpiration, etc. sur les flux thermiques
* Temp ressentie que pour la peau exposée ? (donc sans vêtements ?)
* ...
-->

## Qu'est-ce que la température ?

Le température est la mesure de l'*énergie thermique*, qui est l'énergie cinétique (l'énergie de mouvement) des molécules et des atomes de la matière.

Par exemple l'image ci-dessous est une modélisation de l'agitation d'une protéine :

![Agitation d'une protéine]({{ site.baseurl }}/images/post-images/2020-12-10-temperature-meteo/agitation.gif)

Plus les particules s'agitent, plus la température est élevée.

## Les échelles de température

Il existe plusieurs échelles de température utilisées aujourd'hui :

* Le kelvin
* Le degré Celsius
* Le degré Fahrenheit

D'autres échelles ont existent, plus utlisées aujourd'hui, comme :

* Le degré centigrade (l'ancêtre du degré Celsius)
* Le Rankine
* Le degré Delisle
* Le degré Newton
* Le degré Réaumur
* Le degré Rømer

Note : dans les pays anglophones, notamment au Royaume-Uni, il arrive que les gens parlent de degré *centigrade* pour désigner en fait un degré *celsius*.

### Le kelvin

Le kelvin (K) est l'unité de mesure de la température du système international d'unités. C'est l'échelle de température la plus récente.

Elle est nommée d'après William Thomson, Baron Kelvin, physicien britannique du 19è siècle, qui exposa dans son article de 1848 *On an Absolute Thermometric Scale*[^kelvin_scale] la nécessité d'avoir une échelle absolue de mesure de la température.

![Lord Kelvin]({{ site.baseurl }}/images/post-images/2020-12-10-temperature-meteo/lord-kelvin.jpg){: .medium-height}

Une échelle absolue est *un système de mesure d'une grandeur débutant à 0 et progressant dans un sens unique*. Par exemple l'échelle métrique est une échelle de mesure absolue de longueur, puisqu'il n'y a aucune longueur qui puisse être négative.

Ainsi, puisque la grandeur physique représentée par le température est l'énergie thermique (et donc l'agitation des particules), le 0 de l'échelle kelvin correspond à une énergie thermique nulle, c'est-à-dire l'absence de toute agitation des particules. On l'appelle le *zéro absolu*.

Pour faciliter la conversion avec l'échelle Celsius largement utilisée, on a décidé que les graduations seraient les mêmes pour le kelvin, c'est-à-dire qu'une augmentation de 1K équivaut à une augmentation de 1°C. On a donc l'équivalence suivante : 0K = −273,15°C.

#### Pourquoi une échelle absolue ?

Mais pourquoi s'embêter à créer une échelle absolue si on avait déjà l'échelle Celsius à l'époque ?

Dans son article[^kelvin_scale], Lord Kelvin expose plusieurs raisons, notamment la précision des mesures et la correspondance plus exacte avec la grandeur physique mesurée.

Mais la raison la plus visible pour les non-experts est sans doute la possibilité de comparer les températures.

Imaginez que la météo annonce un jour une température de 10°C et le lendemain 20°C. Vous vous dites : "incroyable, la température a double en 24 heures !". Mais en fait, pas du tout.

En effet, comparer des température en Celsius (ou tout échelle non absolue) c'est aussi vide de sens que de comparer deux longueurs dans une unité, dison le *toto*, où on fixerait le 0 à 1,50m. Dirait-on qu'une personne mesurant 20 totos (1,70m) est deux fois plus grande qu'une personne mesurant 10 totos (1,60m) ? Bien sûr que non.

C'est la même chose avec les Celsius. En réalité une température de 20°C (293,15K) est 3,5% plus grande qu'une de 10°C (283,15K).

![Comparaison °C]({{ site.baseurl }}/images/post-images/2020-12-10-temperature-meteo/compare-c.svg){: .medium-height .inline}
![Comparaison K]({{ site.baseurl }}/images/post-images/2020-12-10-temperature-meteo/compare-k.svg){: .medium-height .inline}

### Le degré centigrade

...

### Le degré Celsius

...

### Le degré Fahrenheit

...

## La mesure de la température

## La température ressentie

![Application météo]({{ site.baseurl }}/images/post-images/2020-12-10-temperature-meteo/meteo-small.png)

### Le froid ressenti

### La chaleur ressentie

### D'autres mesures

### Manque de sens

<!--
  https://fr.wikipedia.org/wiki/Temp%C3%A9rature_ressentie
  https://en.wikipedia.org/wiki/Apparent_temperature
  https://fr.wikipedia.org/wiki/Indice_universel_du_climat_thermique
  https://www.lemonde.fr/les-decodeurs/article/2019/06/24/canicule-qu-est-ce-que-la-temperature-ressentie_5480770_4355770.html
  https://www.youtube.com/watch?v=GN7wROt_W6k
  https://www.youtube.com/watch?v=8bUNGLlp048
-->

<!-- Références -->

[^kelvin_scale]: Thomson, W. (1882). *On an Absolute Thermometric Scale founded on Carnot's Theory of the Motive Power of Heat, and calculated from Regnault's Observations*. Mathematical and Physical Papers, 1, 100‑106. <https://web.archive.org/web/20080201095927/http://zapatopi.net/kelvin/papers/on_an_absolute_thermometric_scale.html>
