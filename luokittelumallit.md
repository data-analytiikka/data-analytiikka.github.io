---
title: Luokittelumallit
layout: default
nav_order: 10
---

# Ohjatut luokittelumallit

Luokittelumallit on yleisnimitys koneoppimisen malleille, joissa ennustettava muuttuja eli **kohdemuuttuja** on kategorinen. Luokittelumalleja voidaan hyödyntää esimerkiksi seuraavissa:

* sairauksien diagnosointi lääketieteellisten mittaustulosten perusteella
* mahdollisten petosten tunnistaminen vakuutuskorvaushakemuksista
* luottokorttipetosten tunnistaminen luottokorttitapahtumien joukosta.

Ohjatuissa koneoppimisen malleissa käytetään opetusdataa mallin opettamiseen. Esimerkiksi luottokorttitapahtumien luokittelussa opetusdatana voi toimia historiallinen data luottokorttitaphtumista, joista jo tiedetään olivatko ne petoksia vai ei. Opetusdatassa on mukana selittäviä muuttujia, joiden oletetaan selittävän kohdemuuttujan jo tiedossa olevia arvoja. Opetusdatan perusteella oppimisalgoritmi muodostaa mallin, jonka avulla voidaan ennustaa uudelle datalle kohdemuuttujan arvoja.

Erilaisia ohjattuja luokittelumalleja on runsaasti tarjolla. Tämän hetken suosituimpia malleja ovat päätöspuihin perustuvat **satunnaismetsä** ja **gradienttitehostus**. Vertailun vuoksi kannattaa kokeilla myös kahta klassista mallia: **yksinkertainen päätöspuu** ja **logistinen regressio**.

Pythonin peruskirjasto koneoppimisen malleille on [scikit-learn](https://scikit-learn.org/stable/index.html), josta yleensä käytetään lyhyempää nimitystä **sklearn**.

[Ensimmäisessä esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/iris.ipynb) on klassinen esimerkki kurjenmiekkojen luokittelusta kolmeen alalajiin (setosa, versicolor, virginica). Selittävinä muuttujina käytetään verho- ja terälehtien pituuksia ja leveyksiä. Yksinkertaisuuden vuoksi käytän ensimmäisessä esimerkissä ainoastaan yksinkertaista päätöspuuta, jonka rakennetta voin havainnolistaa päätöspuukaaviona. Esimerkin avulla opit toteuttamaan Pythonilla keskeiset mallin opettamiseen liittyvät toimet:

* selittävien muuttujien ja kohdemuuttujan määrittely
* opetusdatan jakaminen varsinaiseen **opetusdataan** ja **testidataan**
* mallin opettaminen **fit**-funktiolla
* mallin tarkkuuden laskeminen sekä varsinaiselle opetusdatalle että testidatalle
* mallin hyvyyden arviointi **sekaannusmatriisi**n avulla
* ennustaminen **predict**-funktiolla.

[Toisessa esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/heart.ipynb) opetetaan malli, jonka avulla ennustetaan potilaan riskiä sydänperäiseen kuolemaan. Esimerkissä kokeillaan neljää eri mallia:

* logistinen regressio
* päätöspuu
* satunnaismetsä
* gradienttitehostus.

[Kolmannessa esimerkissä](https://nbviewer.org/github/taanila/koneoppiminen/blob/main/creditcard.ipynb) opetetaan malli, joka tunnistaa petollisia luottokorttitapahtumia. Uutena asiana opit tasapainottamaan opetusdataa. Toteutuneista luottokorttitapahtumista vain murto-osa osoittautuu petoksiksi. Tämän seurauksena opetusdatastakin vain murto-osa on petollisia tapahtumia. Yleensä tällaisen epätasapainoisen opetusdatan avulla ei saada kovin hyviä malleja. Opetusdataa voidaan tasapainottaa lisäämällä siihen alkuperäisten aliedustettujen havaintojen perusteella laskettuja keinotekoisia havaintoja.

{: .new }
Lisää kurjenmiekka-muistioon (ensimmäinen esimerkki) päätöspuun lisäksi logistinen regressio, satunnaismetsä ja gradienttitehostus. Vertaile malleja sekaannusmatriiseja käyttäen.
<br><br>
Opeta malli, joka tunnistaa viinin kemiallisten ominaisuuksien perusteella rypälelajikkeen, josta viini on valmistettu. Datana [wine.xlsx](https://taanila.fi/wine.xlsx) ja datan tarkemman kuvauksen osoitteesta [https://archive.ics.uci.edu/dataset/109/wine](https://archive.ics.uci.edu/dataset/109/wine). Ensimmäinen muuttuja ilmaisee rypälelajikkeen (1, 2 tai 3) ja muut muuttujat liittyvät viinin kemiallisiin ominaisuuksiin. Vertaile malleja sekaannusmatriiseja käyttäen.
<br><br>
Opeta malli, jonka avulla tunnistetaan potentiaalisia lehden tilaajia. Datana [KidCreative.xlsx](https://taanila.fi/KidCreative.xlsx). Kohdemuuttujana on Buy (0 = ei tilaa, 1 = tilaa). Havainnon numeroa (Obs No.) ei kannata ottaa selittäväksi muuttujaksi. Vertaile eri malleja sekaannusmatriiseja käyttäen. Kokeile, saatko paremman mallin tasapainottamalla datan.
<br><br>
Opeta malli, joka tunnistaa potentiaalisia määräaikaistalletuksen valitsevia asiakkaita. Datana [banking.csv](https://taanila.fi/banking.csv). Datan tarkempi kuvaus [https://archive.ics.uci.edu/dataset/222/bank+marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing). Muista tasapainottaa data. Vertaile eri malleja sekaannusmatriiseja käyttäen. 
