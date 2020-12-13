---
layout: post
title: "La température en météo"
date:   2020-12-13 09:00:00 +0200
categories: Sciences
tags:
    - Météorologie
excerpt: \"Température ressentie 0 °C\". Mais qu'est-ce vraiment le degré Celsius ? Comment mesure-t-on la température ? Et qu'est-ce que la température ressentie ?
image:
  path: /images/post-images/2020-12-13-temperature-meteo/main.jpg
  thumbnail: /images/post-images/2020-12-13-temperature-meteo/main-thumb-flat.jpg
  caption: "Image de [Matthew Henry](https://unsplash.com/@matthewhenry)"
---

{% include toc %}

## Introduction

"Température ressentie 0 °C".

Mais qu'est-ce vraiment le degré Celsius ? Comment mesure-t-on la température ? Et qu'est-ce que la température ressentie ?

## Qu'est-ce que la température ?

La température est la mesure de l'*énergie thermique*, qui est l'énergie cinétique (l'énergie de mouvement) des molécules et des atomes de la matière.

Par exemple l'image ci-dessous est une modélisation de l'agitation d'une protéine :

![Agitation d'une protéine]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/agitation.gif)

Plus les particules s'agitent, plus la température est élevée.

## Les échelles de température

Il existe plusieurs échelles de température utilisées aujourd'hui :

* Le kelvin
* Le degré Celsius
* Le degré Fahrenheit

D'autres échelles existent, plus utilisées aujourd'hui, comme :

* Le degré centigrade (l'ancêtre du degré Celsius)
* Le Rankine
* Le degré Delisle
* Le degré Newton
* Le degré Réaumur
* Le degré Rømer

Note : dans les pays anglophones, notamment au Royaume-Uni, il arrive que les gens parlent de degré *centigrade* pour désigner en fait un degré *Celsius*.

### Le kelvin

Le kelvin (K) est l'unité de mesure de la température du système international d'unités, celle utilisée dans les sciences. C'est l'échelle de température la plus récente.

Elle est nommée d'après William Thomson, Baron Kelvin, physicien britannique du 19e siècle, qui exposa dans son article de 1848 *On an Absolute Thermometric Scale*[^kelvin_scale] la nécessité d'avoir une échelle absolue de mesure de la température.

![Lord Kelvin]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/lord-kelvin.jpg){: .medium-height}

Une échelle absolue est *un système de mesure d'une grandeur débutant à 0 et progressant dans un sens unique*. Par exemple l'échelle métrique est une échelle de mesure absolue de longueur, puisqu'il n'y a aucune longueur qui puisse être négative.

Ainsi, puisque la grandeur physique représentée par la température est l'énergie thermique (et donc l'agitation des particules), le 0 de l'échelle kelvin correspond à une énergie thermique nulle, c'est-à-dire l'absence de toute agitation des particules. On l'appelle le *zéro absolu*.

Pour faciliter la conversion avec l'échelle Celsius largement utilisée, on a décidé que les graduations seraient les mêmes pour le kelvin, c'est-à-dire qu'une augmentation de 1 K équivaut à une augmentation de 1 °C. On a donc l'équivalence suivante : 0K = −273,15 °C.

#### Pourquoi une échelle absolue ?

Mais pourquoi créer une échelle absolue si on avait déjà l'échelle Celsius ?

Dans son article[^kelvin_scale], Lord Kelvin expose plusieurs raisons, notamment la précision des mesures et la correspondance plus exacte avec la grandeur physique mesurée.

Mais la raison la plus visible pour les non-experts est sans doute la possibilité de comparer les températures.

Imaginez que la météo annonce un jour une température de 10 °C et le lendemain 20 °C. Vous vous dites : "incroyable, la température a doublé en 24 heures !". Mais en fait, pas du tout.

En effet, comparer des températures en Celsius (ou toute échelle non absolue) c'est aussi vide de sens que de comparer deux longueurs dans une unité, disons le *toto*, où on fixerait le 0 à 1,50 m. Dirait-on qu'une personne mesurant 20 totos (1,70 m) est deux fois plus grande qu'une personne mesurant 10 totos (1,60 m) ? Bien sûr que non.

C'est la même chose avec les Celsius. En réalité une température de 20 °C (293,15 K) est 3,5 % plus grande qu'une de 10 °C (283,15 K).

![Comparaison °C]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/compare-c.svg){: .small-medium-height .inline}
![Comparaison K]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/compare-k.svg){: .small-medium-height .inline}
{: .image-row}

### Le degré centigrade

L'échelle de température centigrade est une échelle de température relative, inventée en 1742 par l'astronome et physicien suédois Anders Celsius.

Elle a deux points de référence :

* La température de fusion de l'eau, correspondant à 0° centigrade
* La température d'évaporation de l'eau à la pression standard (1013,25 hPa), correspondant à 100° centigrade

![Centigrade]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/centigrade.svg){: .medium-height}

L'idée était d'avoir une échelle qui facilitait la création de thermomètres à mercure : on le place dans l'eau glacée pour marquer le 0, puis dans l'eau bouillante pour marquer le 100.

À l'origine les deux points de référence étaient inversés, le 0 correspondait à la température d'ébullition et la valeur augmentait avec le froid, pour éviter d'avoir des températures négatives dans les situations de la vie courante. L'année suivante, en 1743, le physicien français Jean-Pierre Christin inverse l'échelle pour que la valeur augmente avec la température.

L'échelle centigrade a été remplacée par l'échelle Celsius en 1948.

### Le degré Celsius

Le degré Celsius (°C), nommé en l'honneur d'Anders Celsius, a été introduit en 1948 par le *Bureau International des Poids et Mesures*. Il est défini pour être similaire au degré centigrade, mais en se basant sur le kelvin et le zéro absolu, décalé de 273,15K[^bipm].

La définition du Celsius est donc :

* 0 °C = -273,15 K
* Une augmentation de 1 °C = une augmentation de 1 K

Le degré Celsius et donc légèrement différent de son ancêtre le degré centigrade.

Si dans la vie courante on continue à dire que l'eau fond à 0 °C et bout à 100 °C, comme pour l'échelle centigrade, en réalité elle fond à environ 0,000 1 °C et bout à environ 99,983 9 °C.

### Le degré Fahrenheit

Le degré Fahrenheit (°F) a été inventé par le physicien allemand Daniel Gabriel Fahrenheit en 1724. C'est la plus ancienne unité de mesure de la température qui est encore utilisée aujourd'hui.

Elle a à l'origine deux points de référence :

* La température de fusion d'un mélange d'eau et de chlorure d'ammonium, correspondant à 0 °F
* La température moyenne sous l'aisselle d'un homme adulte en bonne santé, correspondant à 96 °F

![Fahrenheit]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/fahrenheit.svg){: .medium-height}

Suite à la création du degré centigrade par Anders Celsius, l'échelle Fahrenheit a été légèrement décalée pour aussi prendre comme points de références la fusion et l'évaporation de l'eau, respectivement à 32 °F et 212 °F.

Lorsque le degré Celsius a remplacé le degré centigrade en étant défini par rapport au kelvin, le Fahrenheit a subi le même changement[^bipm].

La définition du Fahrenheit est donc maintenant :

* 0 °F = -459,67 K
* Une augmentation de 1 °F = une augmentation de 5/9 K

Aujourd'hui le degré Fahrenheit est utilisé comme unité officielle de mesure de la température aux États-Unis, aux Iles Caïman et au Liberia. Il est utilisé en complément du Celsius au Royaume-Uni, au Canada et dans quelques anciennes colonies britanniques dans le pacifique.

### Comparaison

#### Unités en usage aujourd'hui

|                       | Kelvin   | Degré Celsius | Degré Fahrenheit |
|-----------------------|----------|---------------|------------------|
| Zéro absolu           | 0        | -273,15       | −459,67          |
| Zéro Celsius          | 273,15   | 0             | 32               |
| Fusion de l'eau       | 273,1501 | 0,0001        | 32,0002          |
| Point triple de l'eau | 273,16   | 0,01          | 32,018           |
| Vaporisation de l'eau | 373,1339 | 99,9839       | 211,971          |

#### Unités historiques

|                       | Degré centigrade | Degré Fahrenheit historique |
|-----------------------|------------------|-----------------------------|
| Zéro absolu           | −273,197         |                             |
| Fusion de l'eau       | 0                | 32                          |
| Vaporisation de l'eau | 100              | 212                         |

## La mesure de la température

### L'OMM

Partout dans le monde, les organismes météorologiques (en France, Météo-France) suivent les normes et directives internationales définies par l'Organisation Météorologique Mondiale (OMM), une institution de l'ONU.

![OMM]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/omm.png){: .small-medium-height}

Cet organisme a plusieurs activités, notamment de rassembler les données météo planétaires afin de créer des modèles prédictifs, de prévenir les catastrophes climatiques ou, ce qui nous intéresse ici, définir des normes standardisées pour les mesures météorologiques.

Avoir des normes communes est indispensable pour pouvoir comparer les données de différents endroits. Sinon un pays pourrait par exemple décider de mesurer la température à l'ombre et un autre au soleil, rendant impossible de comparer ces données.

### Les normes de mesure

Les normes de mesure des variables météorologiques (température, humidité, vitesse du vent, etc.) sont extrêmement complexes. Le seul guide pour les instruments de mesure[^wmo_guide] fait presque 600 pages, dont 30 pour la mesure de la température.

Il y a plusieurs mesures de la température (air, sol, eau, routes, neige, etc.), mais celle qui nous intéresse est celle de l'air (celle qui est rapportée dans les bulletins météo).

On apprend dans le document que la température de l'air doit être mesurée par une sonde placée sous abri ventilé (protégée du soleil et de la pluie, mais exposée au vent), à une hauteur comprise entre 1,25 et 2 m du sol naturel (préférablement de l'herbe) plat, dans une zone exposée au soleil et éloignée de bâtiments, d'arbres ou autres obstacles.

Il y a aussi des directives pour ajuster les instruments de mesure en fonction de l'environnement (montagne, désert, etc.) ou du type de thermomètre, pour prendre en compte les réflexions causées par la surface d'un lac, la résistance métallique des thermomètres, etc.

Beaucoup de choses très intéressantes, mais un peu techniques pour figurer dans cet article.

Ce que je retiens c'est la recherche de normalisation pour pouvoir comparer les données du monde entier, mais aussi que les températures "scientifiques" sont bien plus strictement définies que les appareils qu'on peut poser sur le bord de la fenêtre ou que peuvent afficher certaines croix de pharmacies.

![Croix pharmacie]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/croix.jpg){: .small-medium-height}

Je me rappelle lors du précédent épisode de canicule, de nombreux médias rapportant des pics de température dans telle ou telle ville en se basant sur les chiffres affichés par les croix de pharmacie. Mais il s'avère que les thermomètres concernés sont exposés en plein soleil, à côté d'un mur, etc. Bref, ils ne suivent pas les normes de l'OMM. Comparer leurs données avec celles de Météo-France n'a donc pas de sens.

## La température ressentie

Vous avez sans doute déjà entendu parler la *température ressentie*, mais que représente-t-elle ?

![Application météo]({{ site.baseurl }}/images/post-images/2020-12-13-temperature-meteo/meteo-small.png)

La température ressentie est une grandeur qui a pour objectif de représenter l'impression subjective de chaud et de froid liée aux conditions météorologiques. Elle se décompose en deux indices : le froid ressenti, par temps froid, et la chaleur ressentie, par temps chaud.

### Avoir chaud et froid

Qu'est-ce qu'avoir chaud et froid ? Pour faire simple, on a froid quand on perd de la chaleur et on a chaud quand on gagne de la chaleur. Les sensations de chaud et de froid sont des signaux physiologiques d'un déséquilibre thermique.

Vous avez sans doute déjà remarqué que vous avez plus froid quand il y a du vent, alors que l'air a la même température. Ou qu'au bout d'une heure dans un bain vous avez froid, alors que l'eau est plus chaude que l'air de votre appartement dans lequel vous passez toute la journée sans avoir froid.

Ainsi ce qui importe dans la sensation de chaud et de froid, ce n'est pas tant la température, mais le flux.

Les échanges de chaleur, ou transferts thermiques, peuvent se faire de trois manières :

* Par *convection* : un transport de chaleur causé par le déplacement d'un fluide, comme un gaz. Cet effet ne concerne pas le corps humain.
* Par *conduction* : un transfert de l'agitation thermique deux deux matières en contact. Le corps humain en contact avec l'air échange de la chaleur ainsi. Plus la différence de température est grande, plus le flux est grand.
* Par *rayonnement* : une émission d'un rayonnement électromagnétique (et une perte de chaleur) par les atomes en mouvements. Comme toute matière au-delà du zéro absolu, le corps humain en émet, notamment dans les infrarouges.

Le principal échange de chaleur pour le corps humain est la conduction.

### Pourquoi un ressenti différent ?

Reprenons l'exemple du bain. Pourquoi avons-nous rapidement plus froid dans l'eau que dans l'air ? Tout simplement parce que les échanges thermiques se font beaucoup plus facilement entre la peau et l'eau qu'entre la peau est l'air, notamment parce que l'eau est plus dense. On peut estimer en moyenne que le flux thermique est 15 fois plus grand quand on est dans l'eau.

Et pour le vent ? Pourquoi a-t-on plus froid quand il souffle ?

On a vu que la sensation de froid est provoquée par un échange de température de notre corps vers l'extérieur, ici l'air. Mais lorsque l'air froid entre en contact avec notre peau, il se réchauffe très légèrement. Or une différence de température plus faible (même un peu) signifie une sensation de froid plus faible. Lorsque le vent souffle, l'air légèrement réchauffé autour de notre peau est remplacé par un air non réchauffé, légèrement plus froid.

> La réalité, ce n’est pas qu’il fait plus froid, c’est que vous perdez plus de chaleur à cause du vent.
>
> — Pascal Yiacouvakis, météorologue

De plus, un temps froid et humide apparaitra plus froid qu'un temps froid et sec. En effet l'air chargé d'humidité sera plus difficile à réchauffer autour de la peau qu'un air sec (puisque l'eau a une plus grande conductivité thermique).

Un dernier facteur entre en compte, c'est la transpiration. Elle est un mécanisme de régulation thermique quand le corps est trop chaud : elle consomme de l'énergie thermique en s'évaporant, réduisant ainsi la température du corps. C'est pour cette raison qu'un temps chaud et humide apparaitra plus chaud qu'un temps chaud et sec : l'air étant déjà saturé d'eau, la transpiration aura du mal à s'évaporer et donc à réduire la température du corps.

### Un indice

La température ressentie porte très mal son nom. Il ne s'agit en effet pas d'une température, mais d'un *indice*, une grandeur sans unité. Dire que la température ressentie est de 10 °C n'a pas de sens, on devrait dire qu'elle est simplement de 10.

En effet il ne s'agit pas d'une grandeur mesurable, mais d'un indice calculé, à peu près équivalent à la *température qu'il devrait faire* pour qu'on ait les mêmes sensations sans "conditions parasites" (vent, humidité).

En gros, dire "la température ressentie est de -5 °C", c'est dire "au vu des conditions de vent et d'humidité, on ressentira une sensation de froid équivalente à celle d'un air sec et sans vent s'il faisait -5 °C".

### Limites

Il ne faut pas oublier que la température ressentie n'est valable que pour la peau exposée au vent ou à l'humidité, est qu'elle est valable pour nous qui produisons de la chaleur, mais pas pour une flaque d'eau par exemple : s'il fait 1 °C et que la température ressentie est de -1 °C, l'eau ne gèle pas pour autant.

Ensuite la température ressentie, que ce soit en froid ou en chaud, n'est valable que si les conditions de vent et d'humidité sont réunies. Si la température ressentie annoncée est de -2 °C, mais que vous vous trouvez dans une zone abritée du vent, ou avec un vent différent que celui prévu, elle sera différente. De même pour l'humidité.

### Utilité

La température ressentie, malgré ses limites, peut être utile, notamment en termes de santé publique pour prévenir la population en cas de danger, notamment lors des phases de canicule ou de grand froid.

## Conclusion

Ce petit article est maintenant terminé. J'espère que vous aurez appris quelque chose.

La météorologie est un domaine passionnant et je l'aborderai peut-être dans l'avenir, par exemple sur le sujet de la modélisation des courants aériens pour prévoir la pluie.

<!-- Références -->

[^kelvin_scale]: Thomson, W. (1882). *On an Absolute Thermometric Scale founded on Carnot's Theory of the Motive Power of Heat, and calculated from Regnault's Observations*. Mathematical and Physical Papers, 1, 100‑106. <https://web.archive.org/web/20080201095927/http://zapatopi.net/kelvin/papers/on_an_absolute_thermometric_scale.html>

[^bipm]: Bureau International des Poids et Mesures. (2019). *BIPM - Brochure sur le SI : Le Système international d’unités*. BIPM. <https://www.bipm.org/fr/publications/si-brochure/>

[^wmo_guide]: World Meteorological Organization. (2018). *Guide to Instruments and Methods of Observation* (No 8). <https://library.wmo.int/doc_num.php?explnum_id=10179>
