---
layout: pre-publish-post
permalink: /pre-publish-systemes-vote/
# layout: post
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

La constiution des États-Unis[^us_constitution] définit les critères d'éligibilité à la fonction de président :

* Avoir au moins 35 ans
* Être citoyen américain à la naissance
* Résider depuis au moins 14 ans aux États-Unis
* Ne pas être candidat à un troisième mandat

### Les primaires

Les différents partis en compétition, notamment les deux principaux (Démocrate et Républicain), organisent des *élections primaires* un an avant les élections présidentielles pour déterminer quel candidat représentera leur parti. Les modalités de ces élections varient selon le parti et l'état où elles se déroulent. Elle ne sont pas réglementées par la loi mais par les statuts internes des différents partis.

Une fois les primaires terminées se tiennent les conventions nationales de chaque parti, où les candidats sont formellement désignés. Les candidats sont désingés par deux, formant un *ticket* avec un candidat à la présidence et un à la vice-présidence.

### Le principe

L'élection présidentielle américaine est un scrutin indirect. Les électeurs élisent pour chaque état des "grands électeurs", lors d'un scrutin *uninominal majoritaire à un tour*. Ces grands électeurs élisent ensuite le président, toujours lors d'un scrutin *uninominal majoritaire à un tour*, mais requérant la majorité absolue.

![Système électoral américain]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/system.svg)

Si les grands électeurs n'arrivent pas à élire le président à la majorité absolue, c'est la chambre des représentants qui élit le président à raison d'une voix par état. Cela ne s'est produit que deux fois, en 1800 et 1824.

### L'élection des grands électeurs

L'élection des grands électeurs se produit lors de l'*election day*, le mardi qui suit le premier lundi de novembre.

Les électeurs votent pour les grands électeurs en fonction du candidat qu'ils supportent (les bulletins portent la mention "grand ellecteur en faveur de tel candidat", ou simplement le nom du candidat). Le candidat arrivant en tête dans un état remporte tous les grands électeurs de cet état.

Chaque état a un nombre de grands électeurs définit, qui correspond au nombre de ses représentants et sénateurs (+ 3 grands électeurs pour Washington, la capitale), pour un total de 538.

#### Le nombre de représentants

Il y a 435 représentants à la Chambre. Le nombre de représentants de chaque état dépend approximativement de son poids démographique, chaque état se voyant accorder au moins un représentant.

Du fait de cette contrainte, les représentants uniques des états peu peuplés ont un poids supérieurs à ceux des autres états. Par exemple :

* Wyoming (577 000 habitants) : 1 représentant pour 577 000 habitants
* Californie (39 557 000 habitants) : 1 représentant pour 746 000 habitants

C'est à dire que la voix d'un représentant du Wyoming est 29% plus forte que celle d'un représentant de Californie.

#### Le nombre de sénateurs

Chaque état compte deux sénateurs.

Cette règle historique date des débuts des États-Unis[^us_senate_black] et a été mis en en place afin que les 13 états orginaux acceptent de ratifier la constitution. Elle est aujourd"hui l'une des plus critiquée du système législatif américain[^us_senate_orts], puisqu'elle donne autant de pouvoir à chaque états peu importe sa population. Ainsi les deux sénateurs du Wyoming, représentant 577 000 habitantys, ont autant de pouvoir que ceux les deux de la Californie, représentant 39 557 000 habitants, soit presque 69 fois plus.

#### L'attribution des grands électeurs

On a donc un nombre de grands électeurs par état correspondant au nombre de représentants et de sénateurs (55 pour la Californie, 36 pour le Texas, etc.).

Dans chaque état, les électeurs votent pour un candidat et celui qui arrive en tête remporte tout les grands électeurs de cet état, peu importe son score. Ainsi, qu'un candidat fasse en score de 51% ou 99% dans un état ne change rien au nombre de grands électeurs.

### L'élection du président

Une fois les grand électeurs élus, ceux-ci se réunnissent pour élire formellement le président. Le candidat ayant le plus de grands électeurs remporte la présidence.

### Le problème : exemple simplifié

Imaginons une élection selon ce système dans une version des États-Unis composée de 3 états et où chaque état reçoit un représentant pour chaque 8000 habitants :

* L'état A a 16 000 habitants. Il a 2 représentants et 2 sénateurs, soit 4 grands électeurs.
* L'état B a 24 000 habitants. Il a 3 représentants et 2 sénateurs, soit 5 grands électeurs.
* L'état C a 40 000 habitants. Il a 5 représentants et 2 sénateurs, soit 7 grands électeurs.

Deux candidats se présentent :

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height .inline}
![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height .inline}
{: .image-row}

Les citoyens votent dans chaque état :

![Votes 1]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes1.svg){: .medium-height}

36,25% ont voté pour Alice et 63,75% pour Bob. Dans un scrutin direct, Bob serait élu.

![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height}

Mais le scrutin n'est pas direct, il est indirect. Chaque état a un nombre de grands électeurs qui élisent le président. Voici ce qui se produit avec une répartition proportionnelle des grands électeurs (chaque candidat obtenant un nombre de grand électeurs proportionnel à sa victoire dans chaque état) :

![Votes 2]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes2.svg){: .medium-height}

Les grand électeurs élisent alors Bob avec 56,25% des voix. Le vainqueur n'a pas changé, dans cette configuration, mais la représentation est déjà plus loin de la réalité (56,25% contre 63,75% en réalité).

![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height}

Mais la réalite est encore pire. En effet la règle est que le candidat arrivant en tête dans un état remporte l'ensemble des grands électeurs de cet état.

![Votes 3]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes3.svg){: .medium-height}

Les grand électeurs élisent Alice avec 56,25% des voix, alors qu'elle n'a obtenu que 36,25% des suffrages du vote populaire.

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height}

### Exemples réels

Par cinq fois dans l'histoire, un président américain a été élu tout en perdant le vote populaire :

* **John Quincy Adams** en 1824 avec 114 000 voix, contre Andrew Jackson avec 153 000 voix (34,21% de plus)
* **Rutherford B. Hayes** en 1876 avec 4 034 000 voix, contre Samuel J. Tilden avec 4 289 000 voix (6,32% de plus)
* **Benjamin Harrison** en 1888 avec 5 444 000 voix, contre Grover Cleveland avec 5 534 000 voix (1,65% de plus)
* **George W. Bush** en 2000 avec 50 456 000 voix, contre Al Gore avec 51 000 000 voix (1,07% de plus)
* **Donald Trump** en 2016 avec 62 985 000 voix, contre Hillary Clinton avec 65 854 000 voix (4,56% de plus)

### Le pire cas

Dans le pire des cas[^us_worst], un candidat pourrait être élu avec 270 grands électeurs (50,1%) en ayant obtenu uniquement 27,9% des voix du vote populaire.

![Worst case]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/worst.png){: .medium-height}

### L'autre gros problème : la majorité à un tour

Le système de vote pour l'élection présidentielle américaine n'est pas seulement indirect, il est majoritaire à un tour.

Imaginons un scénario avec trois candidats : Alice, Bob et Carol.

Deux candidats se présentent :

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height .inline}
![Bob]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/bob.svg){: .small-height .inline}
![Carol]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/carol.svg){: .small-height .inline}
{: .image-row}

Voici les résultats du vote :

![Votes 4]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes4.svg){: .medium-height}

Dans cette configuration, c'est toujours Alice qui est élue avec le plus grand nombre de grands électeurs, malgré le fait qu'elle ait obtenu seulement 22,5% des voix, soit plus que Bob (42,5%) et Carol (35%).

Supposons maintenant que Bob et Carol aient des idées proches et que Bob décide de ne pas se présenter. Supposons que 80% de ceux qui auraient voté pour Bob votent pour Carol, et 20% pour Alice. Voici les résultats :

![Votes 5]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes5.svg){: .medium-height}

Carol serait élue avec 100% des voix (pour 68,75% des voix du vote populaire).

![Carol]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/carol.svg){: .small-height}

Ce système de vote est particulièrement vulnérable aux alternatives, c'est à dire que l'introduction d'un candidat de poids va systématiquement désavantager le candidat dont il est le plus proche et favoriser celui dont il est le plus éloigné. Cet particularité est à l'origine du bipartisme fort et de la polarisation des idées aux États-Unis, les "petits candidats" ayant des scores extrêmement faibles (quelques dizièmes de pourcent).

### Récapitulatif

Sans considérer les problèmes pratiques (bulletins peu clairs, découpages partisans des contés, manque de bureaux de votes, etc.), l'élection présidentielle américaine révèle plusieurs gros problèmes :

* Un poids exagérément grand donné aux états les moins peuplés (atteignant parfois un poids par habitant 69 fois plus grand).
* Un manque fondamental de représentativité, un candidat ayant largement perdu le vote populaire pouvant être élu.
* Une grande vulnérabilité aux alternatives, avec un désavantage systématique des candidats proches de chaque nouveau candidat.

Dans la suite de cet article nous allons voir comment le système français rend les choses un peu plus équitables, mais pas tellement. Nous verrosn quels sont les différents critères pour évaluer un système de vote, comment mesurer sa solidité et la fiabilité de se représentativité, et passer en revu différents systèmes existants ou théoriques.

## D'autres modes de scrutin

### Un système direct a deux tours ?

Le mode de scrutin pour l'élection présidentielle en France est fondamentalement différent du système américain sur deux points importants :

* Il est direct, donc il n'y a pas de système de grands électeurs entrainant une représentation faussée.
* Il comporte deux tours, un candidat doit dont impérativement recevoir plus de 50% des voix pour être élu.

Malgré tout il comporte de sérieuses failles, que nous allons voir brièvement.

Reprenons notre scénario initial :

![Candidats]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/candidates.svg)

Imaginons que chacun vote pour le candidat qu'il préfère réellement. Voici la répartition des votes :

![Votes 6]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes6.svg){: .medium-height}

Dans le système français, l'élection se déroule en deux tours (sauf si l'un des candidats obtient plus de 50% au premier tour).

Les deux candidats ayant obtenu les plus de vote au premier tour sont Alice et Eve. Elles s'affrontent donc au second tour.

![Alice]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/alice.svg){: .small-height .inline}
![Eve]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/eve.svg){: .small-height .inline}
{: .image-row}

Ceux ayant voté pour l'une d'elles gardent leur vote. Les autres doivent choisir laquelle ils préfèrent :

![Votes 7]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes7.svg){: .medium-height}

Parmis les 45% d'électeurs n'ayant pas voté pour Alice ou Eve au premier tour, 41% préfèrent Eve.

![Votes 8]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/votes8.svg){: .medium-height}

Eve est élue avec 63% des voix.

![Eve]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/eve.svg){: .small-height}

Ce système est plus représentatif que le système américain, mais cependant la représentation reste faussée.

Évaluons la satisfaction de la population pour le résultat.

Nous connaissons l'ordre dans lequel différentes parties de la population ont classé les candidats selon leurs préférences. Pour simplifier, considérons que le candidat en 1ère position est approuvé à 100%, le 2ème à 75%, etc. :

| Classement | Approbation |
|------------|-------------|
| #1         | 100 %       |
| #2         | 75 %        |
| #3         | 50 %        |
| #4         | 25 %        |
| #5         | 0 %         |

Voici l'approbation moyenne pour chaque candidat :

![Approval 2]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approval2.svg){: .medium-height}

Ici, c'est Carol qui reçoit l'approbation la plus grande, avec 61,75%, légèrement devant Bob avec 61,00%. Eve, pourtant élue, arrive troisième avec seulement 54,50% d'approbation.

Le scrutin a deux tours fait donc à priori mieux qu'un système à un tour (qui aurait élu Alice, qui a pourtant la plus faible approbation moyenne), mais n'est pas parfait, puisqu'on a deux candidats avec plus d'approbation que celle qui a été élue.

### Un vote par approbation ?

A ce stade, on pourrait se dire que c'est Carol qui devrait être élue. On prendrait ferait la moyenne de l'approbation de la population, en attribuant un nombre de points selon l'ordre du candidat sur un bulletin où tous seraient classés, comme avec la méthode Borda vue dans l'introduction.

Seulement cette méthode a un problème. Nous avons accordé, pour chaque bulletin, 100 points au premier, 75 au deuxième, etc. (ou dans la méthode borda 4 points au premier, 3 au deuxième, etc.). Mais pourquoi l'écart de points est-il le même entre chaque position surt le classement ?

Considérons la première ligne des préférences dans le tableau :

![Line 1]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/line1.svg){: .medium-height}

On voit que 33% des électeurs préfèrent Alice, puis Carol, puis Bob, puis Dave, puis Eve. Mais préfèrent-ils Alice à Carol autant qu'ils préfèrent Carol à Bob ? Peut-être qu'Alice et Carol ont toutes deux des idées qui plaisent beaucoup à ces 33%, celles d'Alice leur plaisant très légèrement plus, et que Bob, Dave et Eve ont tous des idées qui leur déplaisent énormément ?

Quelle serait l'approbation moyenne si les écarts n'étaient pas réguliers ? Par exemple :

| Classement | Approbation |
|------------|-------------|
| #1         | 90 %        |
| #2         | 60 %        |
| #3         | 50 %        |
| #4         | 20 %        |
| #5         | 15 %        |

On obtient :

![Approval 3]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approval3.svg){: .medium-height}

Cette fois-ci c'est Bob qui est en tête !

Et si on avait ces valeurs :

| Classement | Approbation |
|------------|-------------|
| #1         | 60 %        |
| #2         | 15 %        |
| #3         | 5 %         |
| #4         | 0 %         |
| #5         | 0 %         |

On aurait :

![Approval 4]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approval4.svg){: .medium-height}

Alice serait en tête !

Et si on avait ces valeurs :

| Classement | Approbation |
|------------|-------------|
| #1         | 99 %        |
| #2         | 50 %        |
| #3         | 49 %        |
| #4         | 48 %        |
| #5         | 5 %         |

On aurait :

![Approval 5]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approval5.svg){: .medium-height}

Eve serait en tête !

Encore plus compliqué maintenant, imaginons que les écarts ne sont pas les mêmes dans chaque tranche de la population !

Par exemple :

![Approvals]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approvals.svg){: .medium-height}

* 33% de la population approuve Alice à 97%, Carol à 90%, etc.
* 22% de la population approuve Eve à 84%, Bob à 82%, etc.
* Etc.

Et, dans la réalité, le problème est encore bien plus complexes, car dans la tranche de la population qui classe les candidats dans un même ordre, tout le monde n'a pas la même approbation pour chacun. Par exemple parmi les 33% de la première ligne, on a peut-être ça :

![Approvals 2]({{ site.baseurl }}/images/post-images/2020-12-19-systemes-vote/approvals2.svg){: .medium-height}

Quel système pourrait résoudre ce problème ?

## Étude de cas : les élections européennes ???

<!-- www.youtube.com/watch?v=h4Uu5eyN6VU -->

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

[^us_constitution]: United States Senate. (2020, 21 janvier). *Constitution of the United States*. Senate.gov. <https://www.senate.gov/civics/constitution_item/constitution.htm>

[^us_senate_orts]: Orts, E. W. (2019, 4 janvier). *Here’s How to Fix the Senate*. The Atlantic. <https://www.theatlantic.com/ideas/archive/2019/01/heres-how-fix-senate/579172/>

[^us_senate_black]: Black, E. (2018, 20 juillet). *The House, the Senate and the historical reasons for (un)equal representation*. MinnPost. <https://www.minnpost.com/eric-black-ink/2018/07/house-senate-and-historical-reasons-unequal-representation/>

[^us_worst]: Brown, A. (2020, 10 décembre). *You could win just 11 counties and still win the presidency*. Tableau. <https://public.tableau.com/profile/ari.brown#!/vizhome/MinimumCounties/MinimumCounties?publish=yes>
