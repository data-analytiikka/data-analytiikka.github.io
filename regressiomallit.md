---
title: Regressiomallit
layout: default
nav_order: 11
---

## Ohjatut regressiomallit

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
* selittävän muuttujan ja kohdemuuttujan määrittely
* mallin opettaminen **fit**-funktiolla
* lineerisen regressiomallin **kulmakertoimen** ja **vakiotermin** tulkinta
* mallin hyvyyden arviointi **selityskertoimen** avulla
* ennustaminen **predict**-funktiolla.

[Toisessa esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/linreg2.ipynb) mukana on useita selittäviä muuttujia. Tässä esimerkissä opetusdatasta ei eroteta testidataa, koska data on liian pieni. Ensimmäisessä esimerkissä opittujen asioiden lisäksi opit:

* tarkastelemaan korrelaatiokertoimia
* tarkastelemaan mallin hyvyyttä graafisesti.

[Kolmannessa esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/advertising.ipynb) ennustetaan myyntiä eri mainosmedioihin käytetyn rahamäärän perusteella. Esimerkissä kokeillaan kolmea eri mallia:

* lineaarinen regressio
* satunnaismetsäregressio
* gradienttitehostusregressio.

Esimerkissä koodataan aluksi **yleiskäyttöinen funktio**, joka osaa:

* opettaa funktiolle parametrina annetun mallin
* laskea selityskertoimen
* piirtää mallin hyvyyttä kuvaavat grafiikat.

Funktion avulla on helppo kokeilla eri malleja kutsumalla funktiota kunkin mallin kohdalla.

[Neljännessä esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/car_data.ipynb) ennustetaan käytetyn auton hintaa. Uutena asiana opit muuntamaan **kategoriset muuttujat dikotomisiksi muuttujiksi**. Koneoppimisen malleja varten kategoriset selittävät muuttujat täytyy muuntaa dikotomisiksi muuttujiksi. Tämä koskee myös luokittelumalleja.  

{: .new }
Opeta malli, joka ennustaa rakennuksen lämpökuorman. Lämpökuormaa tarvitaan rakennuksen lämmityslaitteiden mitoitukseen. Käytä dataa [ENB2012_data.xlsx](https://taanila.fi/ENB2012_data.xlsx). Datan lähde ja tarkempi kuvaus osoitteessa [https://www.kaggle.com/datasets/elikplim/eergy-efficiency-dataset](https://www.kaggle.com/datasets/elikplim/eergy-efficiency-dataset). Datassa selittävinä muuttujina ovat X1, X2, X3, X4, X5, X6, X7, X8 ja kohdemuuttujana Y1 (lämpökuorma). Voit myös opettaa mallin, joka ennustaa viilennyskuorman (kohdemuuttujan Y2). Voit hyödyntää mallin opettamiseen kolmannessa esimerkissä koodattua valmista funktiota.
<br><br>
Opeta malli, joka ennustaa betonin puristuslujuutta. Käytä dataa [Concrete_Data.xlsx](https://taanila.fi/Concrete_Data.xlsx). Datan lähde ja tarkempi kuvaus osoitteessa [https://www.kaggle.com/datasets/elikplim/concrete-compressive-strength-data-set](https://www.kaggle.com/datasets/elikplim/concrete-compressive-strength-data-set). Voit hyödyntää mallin opettamiseen kolmannessa esimerkissä koodattua valmista funktiota.
