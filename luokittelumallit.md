---
title: Luokittelumallit
layout: default
nav_order: 10
---

# Ohjatut luokittelumallit

Luokittelumallit on yleisnimitys koneoppimisen malleille, joissa ennustettava muuttuja eli **kohdemuuttuja** on kategorinen. Luokittelumalleja voidaan hyödyntää esimerkiksi seuraavissa:

* sähköpostiviestien luokittelu tavallisiin ja roskaposteihin
* sairauksien diagnosointi lääketieteellisten mittaustulosten perusteella
* mahdollisten petosten tunnistaminen vakuutuskorvaushakemuksista
* luottokorttipetosten tunnistaminen luottokorttitapahtumien joukosta.

Ohjatuissa koneoppimisen malleissa käytetään opetusdataa mallin opettamiseen. Esimerkiksi luottokorttitapahtumien luokittelussa opetusdatana voi toimia historiallinen data luottokorttitaphtumista, joista jo tiedetään olivatko ne petoksia vai ei. Opetusdatassa on mukana selittäviä muuttujia, joiden oletetaan selittävän kohdemuuttujan arvoja ja jo tiedossa olevia kohdemuuttujan arvoja. Opetusdatan perusteella oppimisalgoritmi muodostaa mallin, jonka avulla voidaan ennustaa uudelle datalle kohdemuuttujan arvoja.

Erilaisia ohjattuja luokittelumalleja on runsaasti tarjolla. Tämän hetken suosituimpia malleja ovat päätöspuihin perustuvat satunnaismetsä ja gradienttitehostus. Vertailun vuoksi kannattaa kokeilla myös kahta klassista mallia: yksinkertainen päätöspuu ja logistinen regressio.

Pythonin peruskirjasto koneoppimisen malleille on [scikit-learn](https://scikit-learn.org/stable/index.html), josta yleensä käytettän lyhyempää nimitystä **sklearn**.

[Ensimmäisenä esimerkinä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/iris.ipynb) on klassinen esimerkki kurjenmiekkojen luokittelusta kolmeen alalajiin (setosa, versicolor, virginica) verho- ja terälehtien pituuksien ja leveyksien perusteella. Yksinkertaisuuden vuoksi käytän ensimmäisessä esimerkissä ainoastaan yksinkertaista päätöspuuta, jonka rakennetta voin havainnolistaa päätöspuukaaviona. Esimerkin avulla opit keskeiset mallin opettamiseen liittyvät toimet:

* selittävien muuttujien ja kohdemuuttujan määrittely
* opetusdatan jakaminen varsinaiseen **opetusdataan** ja **testidataan**
* mallin opettaminen **fit**-funktiolla
* mallin hyvyyden arviointi **sekaannusmatriisi**n avulla
* ennustaminen **predict**-funktiolla.



{: .new }
Harjoittele.