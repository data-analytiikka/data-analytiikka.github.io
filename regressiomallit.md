---
title: Regressiomallit
layout: default
nav_order: 11
---

# Ohjatut regressiomallit

Tämä osio on vasta rakenteilla...

Regressiomallit on yleisnimitys koneoppimisen malleille, joissa ennustettava muuttuja eli **kohdemuuttuja** on määrällinen. Regressiomalleja voidaan hyödyntää esimerkiksi seuraavissa:

* kesämökin hinnan ennakointi tontin koon, rantaviivan pituuden, rakennusmateriaalin ym. ominaisuuksien perusteella
* tuotteen myynnin ennustaminen eri mainosmedioihin käytetyn rahamäärän perusteella
* käytetyn auton hinnan ennakointi auton ominaisuuksien perusteella

Ohjatuissa koneoppimisen malleissa käytetään opetusdataa mallin opettamiseen. Esimerkiksi kesämökin hintamallia opetettaessa opetusdatana voi toimia historiallinen data myytyjen kesämökkien hinnoista ja ominaisuuksista. Opetusdatan perusteella oppimisalgoritmi muodostaa mallin, jonka avulla voidaan ennustaa uudelle datalle kohdemuuttujan arvoja.

Erilaisia ohjattuja regressiomalleja on runsaasti tarjolla. Tämän hetken suosituimmat mallit ovat päätöspuihin perustuvat **satunnaismetsäregressio** ja **gradienttitehostusregressio**. Vertailun vuoksi kannattaa kokeilla myös **lineaarista regressiota**, joka on perinteisesti käytetty regressiomalli.

{: .important }
Nimestään huolimatta logistinen regressio on luokittelumalli.

Pythonin peruskirjasto koneoppimisen malleille on [scikit-learn](https://scikit-learn.org/stable/index.html), josta yleensä käytettän lyhyempää nimitystä **sklearn**.

[Ensimmäisessä esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/linreg1.ipynb) opit käyttämään lineaarista regressiota yhden selittävän muuttujan tapauksessa. Tässä esimerkissä opetusdatasta ei eroteta testidataa, koska data on liian pieni. Keskeisiä vaiheita ovat:

* graafinen tarkastelu
* selittävän muuttujien ja kohdemuuttujan määrittely
* mallin opettaminen **fit**-funktiolla
* lineerisen regressiomallin **kulmakertoimen** ja **vakiotermin** tulkinta
* mallin hyvyyden arviointi **selityskertoimen** avulla
* ennustaminen **predict**-funktiolla.

[Toisessa esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/linreg2.ipynb) mukana on useita selittäviä muuttujia. Tässä esimerkissä opetusdatasta ei eroteta testidataa, koska data on liian pieni. Ensimmäisessä esimerkissä opittujen asioiden lisäksi opit:

* tarkastelemaan korrelaatiokertoimia
* tarkastelemaan mallin hyvyyttä graafisesti
* laskemaan kattavan kokoelman lineaariseen regressioon liittyviä tunnuslukuja **statsmodels**-kirjaston avulla.

[Neljännessä esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/advertising.ipynb) ennustetaan myyntiä eri mainosmedioihin käytetyn rahamäärän perusteella. Esimerkissä kokeillaan kolmea eri mallia:

* lineaarinen regressio
* satunnaismetsäregressio
* gradienttitehostusregressio.

Esimerkissä koodataan aluksi yleiskäyttöinen funktio, joka osaa:

* sovittaa parametrina annetun mallin
* laskee selityskertoimen
* piirtää mallin hyvyyttä kuvaavat grafiikat.

Funktion avulla on helppo kokeilla eri malleja kutsumalla funktiota kunkin mallin kohdalla.

[Viidennessä esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/car_data.ipynb) ennustetaan käytetyn auton hintaa.



  

{: .new }
x
