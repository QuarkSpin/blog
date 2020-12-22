---
layout: post
title: "Différents systèmes de vote"
# date:   2020-11-16 16:08:00 +0200
categories: Politique
tags:
    - Vote
    - Mathématiques
    - Démocratie
excerpt: La France utilise un *scrutin uninominal majoritaire à deux tours* pour élire le Président de la République. Mais quels sont les différents systèmes de votes existants et théoriques ? Quels sont leurs particularités, leurs avantages et leurs inconvénients ?
image:
  path: /images/post-images/2020-12-19-systemes-vote/main.jpg
  thumbnail: /images/post-images/2020-12-19-systemes-vote/main-thumb-flat.jpg
  caption: "Image de [Paweł Czerwiński](https://unsplash.com/@pawel_czerwinski)"
---

{% include wip %}

{% include toc %}

## Introduction

Les élections présidentielles approchent, cinq candidats se présentent : Alice, Bob, Carol, Dave et Eve.

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height .inline}
![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height .inline}
![Carol]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/carol.svg){: .small-height .inline}
![Dave]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/dave.svg){: .small-height .inline}
![Eve]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/eve.svg){: .small-height .inline}
{: .image-row}

Avant de voter, les électeurs examinent les programmes des candidats. Voici leur classement préférenciel :

![Candidats]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/candidates.svg)

Ainsi :

* 33% des électeurs préfèrent Alice, puis Carol, puis Bob, puis Dave, puis Eve
* 22% des électeurs préfèrent Eve, puis Bob, puis Carol, puis Dave, puis Alice
* Etc.

On peut aussi le représenter sous forme de tableau avec la position de chaque candidat :

|     | Alice     | Bob     | Carol     | Dave     | Eve     |
|-----|-----------|---------|-----------|----------|---------|
| 33% | **1**     | 3       | 2         | 4        | 5       |
| 22% | 5         | 2       | 3         | 4        | **1**   |
| 18% | 5         | 3       | 4         | **1**    | 2       |
| 16% | 5         | 3       | **1**     | 2        | 4       |
| 7%  | 5         | **1**   | 3         | 4        | 2       |
| 4%  | 4         | **1**   | 3         | 2        | 5       |

Imaginons que chacun vote honnêtement selon ses préférences, et voyons quels seraient les résultats selon différents systèmes de vote.

### Scrutin uninominal majoritaire à un tour

Le candidat remportant le plus de vote l'emporte.

Chaque élécteur vote pour son candidat favori. Alice est élue présidente avec 33% des voix.

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height }

Ce système est notamment utilisé aux États-Unis.

### Scrutin uninominal majoritaire à deux tours

Le candidat remportant plus de 50% des votes l'emporte. Si aucun candidat n'obtient plus de 50% des votes, les deux candidats ayant remporté le plus de votes s'affrontent dans un second tour.

Chaque élécteur vote pour son candidat favori. Aucun n'obtient plus de 50% des voix.

Les deux candidats avec le plus de voix (Alice avec 33% et Eve avec 22%) s'affrontent dans un second tour.

Chaque élécteur vote pour sa candidate favorite parmis les deux restantes. Par exemple, les 18% qui avaient voté pour Dave votent pour Eve, qui est leur second candidat favori.

Eve est élue présidente avec 63% des voix.

![Eve]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/eve.svg){: .small-height }

Ce système est notamment utilisé en France.

### Vote alternatif

Le candidat remportant plus de 50% des votes l'emporte. Si aucun candidat n'obtient plus de 50% des votes, le candidat ayant obtenu le moins de vote est éliminé. Le vote des électeurs dont il était le premier choix est reporté sur leur second choix. On répète l'opération tant qu'un candidat n'a pas obtenu plus de 50% des voix.

Chaque candidant vote en indiquant son classement des candidats. Bob arrive dernier avec 11% des voix. Il est éliminé.

Parmis ceux qui l'ont placé en premier choix, 7% ont placé Eve en deuxième (qui passe à 29%) et 4% ont placé Dave en deuxième (qui passe à 22%).

|     | Alice     | Carol     | Dave     | Eve     |
|-----|-----------|-----------|----------|---------|
| 33% | **1**     | 2         | 4        | 5       |
| 22% | 5         | 3         | 4        | **1**   |
| 18% | 5         | 4         | **1**    | 2       |
| 16% | 5         | **1**     | 2        | 4       |
| 7%  | 5         | 3         | 4        | 2 ✔️   |
| 4%  | 4         | 3         | 2 ✔️    | 5       |
|-----|-----------|-----------|----------|---------|
| **Total** | **33%** | **16%** | **22%** | **29%** |

Carol arrive dernière avec 16% des voix. Elle est éliminée.

On redistribue de nouveau des voix en fonction des préférences des électeurs sur les candidats restants. Les électeurs ayant voté pour Carol préfèrent tous Dave aux deux autres. Il obtient 38% des voix. Alice est toujours à 33% et Eve à 29%.

|     | Alice     | Dave     | Eve     |
|-----|-----------|----------|---------|
| 33% | **1**     | 4        | 5       |
| 22% | 5         | 4        | **1**   |
| 18% | 5         | **1**    | 2       |
| 16% | 5         | 2 ✔️    | 4       |
| 7%  | 5         | 4        | 2 ✔️   |
| 4%  | 4         | 2 ✔️    | 5       |
|-----|-----------|-----------|----------|
| **Total** | **33%** | **38%** | **29%** |

Eve arrive dernière avec 29% des voix. Elle est éliminée.

On redistribue de nouveau des voix en fonction des préférences des électeurs sur les candidats restants. Les électeurs ayant voté pour Eve préfèrent Dave à Alice (même s'il n'est qu'en 4ème position de préférence).

Dave est élu président avec 67% des voix.

![Dave]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/dave.svg){: .small-height }

Ce système est notamment utilisé en Australie.

### Méthode Borda

Les électeurs classent les candidats selon leurs préférences sur un bulletin. Pour chaque bulletin, chaque candidat se voit attribuer un nombre de point égal au nombre de candidats placé sous eux. S'il y a 5 candidats, le candidat en première position sur un bulletin remporte 4 points, le deuxième 3 points, etc. et le dernier 0 points.

Reprenons notre tableau de préférences et supposons qu'il y ait 1000 électeurs pour simplifier les chiffres.

Alice est placée en première position par 330 électeurs (ce qui vaut 330 × 4 = 1320 points), en quatrième position par 40 électeurs (ce qui vaut 40 × 1 = 40 points) et en cinquième position par le reste (ce qui vaut 0 points). Elle obtient donc 1360 points au total.

On répète le calcul pour chaque candidat (les points correspondant au classement sont indiqués entre parenthèses) :

|     | Alice         | Bob         | Carol         | Dave         | Eve         |
|-----|---------------|-------------|---------------|--------------|-------------|
| 33% | **1** (4)     | 3 (2)       | 2 (3)         | 4 (1)        | 5 (0)       |
| 22% | 5 (0)         | 2 (3)       | 3 (2)         | 4 (1)        | **1** (4)   |
| 18% | 5 (0)         | 3 (2)       | 4 (1)         | **1** (4)    | 2 (3)       |
| 16% | 5 (0)         | 3 (2)       | **1** (4)     | 2 (3)        | 4 (1)       |
| 7%  | 5 (0)         | **1** (4)   | 3 (2)         | 4 (1)        | 2 (3)       |
| 4%  | 4 (1)         | **1** (4)   | 3 (2)         | 2 (3)        | 5 (0)       |
|-----|---------------|-------------|---------------|--------------|-------------|
| **Points** | **1360** | **2440** | **2470** | **1940** | **1790** |

Carol est élue présidente avec 2470 points.

![Carol]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/carol.svg){: .small-height }

Ce système est notamment utilisé à Nauru.

### Méthode Condorcet

Ce système choisit comme vainqueur le candidat préféré à tous les autres par une majorité de votants. Les électeurs indiquent leur classement sur un bulletin. Le dépouillement consiste à simuler *l'ensemble des duels possibles*. Le candidat qui l'emporte est celui qui a remporté le plus de duels.

Dans notre exemple avec 5 candidats, chaque candidat participe à 4 duels, pour 10 duels au total.

* **Alice vs Bob** : Bob l'emporte avec 67%
* **Alice vs Carol** : Carol l'emporte avec 67%
* **Alice vs Dave** : Dave l'emporte avec 67%
* **Alice vs Eve** : Eve l'emporte avec 63%
* **Bob vs Carol** : Bob l'emporte avec 51%
* **Bob vs Dave** : Bob l'emporte avec 66%
* **Bob vs Eve** : Bob l'emporte avec 60%
* **Carol vs Dave** : Carol l'emporte avec 78%
* **Carol vs Eve** : Carol l'emporte avec 53%
* **Dave vs Eve** : Dave l'emporte avec 71%

On compte ensuite le nombre de duels remportés par chaque candidat :

* Alice : 0 / 4
* Bob : 4 / 4
* Carol : 3 / 4
* Dave : 2 / 4
* Eve : 1 / 4

Bob est élu président avec 4 duels remportés sur 4.

![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height }

Ce système n'est actuellement pas utilisé pour des élections dans aucun état. Il est utilisé par certaines organisation, comme la fondation Debian.

### Résumé

Ce que nous venons de voir est très intéressant. A partir des mêmes préférences initiales, nous avons obtenu 5 résultats différents avec 5 systèmes différents !

Les candidats et les préférences des électeurs n'ont pas changé, seulement les systèmes de vote.

Se pose donc une série de question : quel système devrions-nous adopter ? lequel représente le mieux la volonté des électeurs ? quels sont leurs avantages et inconvénients en termes de représentativité, complexité, etc. ? C'est ce que nous allons voir dans cet article.

## Étude de cas : l'élection présidentielle aux États-Unis

Avant de nous intéresser aux différents mode de scrutin, aux critères importants, à leurs inconvénients et avantages, étudions le cas de l'élection présidentielle aux États-Unis.

Le système électoral pour la présidentielle américaine est l'un des pires système de vote en termes de représentativité des citoyens, même considéré comme le pire de toutes les démocraties occidentales par nombre de spécialistes. [^us_elections_norris] [^us_elections_norris2] [^us_elections_cowan] [^us_elections_prokop]

Étudier son fonctionnement permet de mieux saisir certains problèmes et d'en discuter plsu facilement par la suite.

### Son fonctionnement

#### Éligibilité

La consti

### Exemple simplifié

### Les problèmes

## Un bon système ?

Il y a plusieurs critères à prendre en compte dans l'évaluation des systèmes de vote, notamment avoir la meilleure représentativité possible des citoyens. Mais il y en a d'autres.

###







<!--
Explorer : faisabilité, avantages et inconvenients, stratégies (pour candidats et votants), etc.

Adresser le problème de l'écart dans le classement des préférences (ex : candidats 1 et 2 préférés de peu, mais très loin des cnadidats 3, 4 et 5 = même classement si 1, 2 et 3 proches en tête et 4 et 5 en loin derrière)

Ressources à consulter :

* <https://fr.wikipedia.org/wiki/Syst%C3%A8me_%C3%A9lectoral>
* <https://www.youtube.com/watch?v=yhO6jfHPFQU>
* <https://www.youtube.com/watch?v=PaxVCsnox_4>
* <https://www.youtube.com/watch?v=v7gZPEeOh1I>
* <https://www.youtube.com/watch?v=vfTJ4vmIsO4>
* <https://cortecs.org/chiffres-graphiques/le-jugement-majoritaire-et-ses-alternatives/>
* <https://en.wikipedia.org/wiki/Random_ballot>
* <https://www.youtube.com/watch?v=r9rGX91rq5I>
* <https://www.youtube.com/watch?v=pkpfFuiZkcs> => que seraient les USA si le sénat était représentatif de la population et que le président était élu au vote populaire (faire les calculs pour différentes éléections depuis les années 2000)
* https://www.youtube.com/watch?v=A-4dIImaodQ


A aborder

* Systèmes de vote pour élire une personne unique (e.g. un président) et pour élire un collège de représentants.
* Critères pour les systèles électoraux
* Les problèmes avec les systèmes actuels, comparaison des plus connus, etc.

-->

[^us_elections_norris]: Norris, P. (2016, 24 mars). *American elections ranked worst among Western democracies. Here’s why*. The University of Sydney. <https://www.sydney.edu.au/news-opinion/news/2016/03/24/american-elections-ranked-worst-among-western-democracies--heres.html>

[^us_elections_cowan]: Cowan, D. (2020, 2 novembre). *Four ways of electing a president - ranked from worst to best*  Electoral Reform Society. <https://www.electoral-reform.org.uk/four-ways-of-electing-a-president-ranked-from-worst-to-best/>

[^us_elections_prokop]: Prokop, A. (2016, 19 décembre). Why the Electoral College is the absolute worst, explained. Vox. <https://www.vox.com/policy-and-politics/2016/11/7/12315574/electoral-college-explained-presidential-elections-2016>

[^us_elections_norris2]: Norris, P. (2017). *Why American Elections Are Flawed (And How to Fix Them)*. Cornell University Press.
