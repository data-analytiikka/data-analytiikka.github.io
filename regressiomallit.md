---
title: Regressiomallit
layout: default
nav_order: 11
---

# Ohjatut regressiomallit

Tämä osio on vasta rakenteilla...

Regressiomallit on yleisnimitys koneoppimisen malleille, joissa ennustettava muuttuja eli **kohdemuuttuja** on määrällinen. Regressiomalleja voidaan hyödyntää esimerkiksi seuraavissa:

* 
* 
* 

Ohjatuissa koneoppimisen malleissa käytetään opetusdataa mallin opettamiseen. Esimerkiksi .... Opetusdatassa on mukana selittäviä muuttujia, joiden oletetaan selittävän kohdemuuttujan jo tiedossa olevia arvoja. Opetusdatan perusteella oppimisalgoritmi muodostaa mallin, jonka avulla voidaan ennustaa uudelle datalle kohdemuuttujan arvoja.

Erilaisia ohjattuja regressiomalleja on runsaasti tarjolla. Tämän hetken suosituimpia malleja ovat päätöspuihin perustuvat **satunnaismetsäregressio** ja **gradienttitehostusregressio**. Vertailun vuoksi kannattaa kokeilla myös **lineaarista regressiota**, joka on perinteisesti käytetty regressiomalli.

{: .note }
Nimestään huolimatta logistinen regressio on luokittelumalli.

Pythonin peruskirjasto koneoppimisen malleille on [scikit-learn](https://scikit-learn.org/stable/index.html), josta yleensä käytettän lyhyempää nimitystä **sklearn**.

{: .new }
