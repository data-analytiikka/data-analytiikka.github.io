---
title: Python + pandas
layout: default
nav_order: 2
---

# Python + pandas

Tässä osiossa on tarkoituksena

* tutustua alustavasti Python-koodaukseen
* oppia Pythonin keskeiset tietorakenteet **lista** (list) ja **sanakirja** (dictionary)
* tutustua alustavasti data-analytiikan **pandas**-pakettiin (pakettia voidaan kutsua myös kirjastoksi) ja erityisesti oppia käyttämään pandas-paketissa määriteltyä **dataframe**-tietorakennetta.

## Opiskeluohjeita

* Oppimateriaalina on muistio [pandas1](https://nbviewer.org/github/taanila/kuvaileva/blob/main/pandas1.ipynb).
* Lue huolellisesti muistion selitykset ja kommentit.
* Kirjoita koodisolujen koodit omaan muistioosi ja siirry seuraavaan soluun vasta kun saat koodin onnistuneesti suoritettua. Pienimmätkin kirjoitusvirheet ja kielioppivirheet aiheuttavat virheilmoituksen. Virheilmoitukset ovat usein vaikeasti tulkittavia, mutta virheilmoituksesta kannattaa selvittää: millä rivillä virhe on ja virheilmoituksen viimeiseltä riviltä saatat saada selville minkälainen virhe on kyseessä?
* Jos koodissa jokin asia askarruttaa, niin kannattaa tehdä omia kokeiluja ja kokeilla vaihtoehtoisia koodeja.
* Lisää omia kommentteja ja huomautuksia. Koodisoluun voit lisätä kommenttirivin kirjoittamalla rivin alkuun risuaidan **#**. Pidempiä tekstejä voit kirjoittaa *Markdown**-soluihin (Colabissa **Text**-soluihin).
* Tässä ensimmäisessä muistiossa on häkellyttävän paljon opittavaa, varsinkin jos et ole aikaisemmin koodannut. Tähän kannattaa käyttää aikaa, koska näin luot hyvän pohjan tulevien osioiden oppimiselle. Kaikkiin tämän muistion asioihin palataan myöhemmissä osioissa.

{: .important }
Kun avaat aiemmin kirjoitetun muistion, niin voit suorittaa kaikkien solujen koodit **Run**-valikon komennolla **Run All Cells** (Colabissa **Runtime - Run all**/**Suorituspalvelu - Suorita kaikki**). Komento auttaa myös usein, jos jostain syystä ajaudut umpikujaan koodin suorituksessa (näin voi käydä, jos esimerkiksi korjailet ja suorittelet välillä aiempien solujen koodeja).


## Google Colabin käyttäjille

{: .warning }
Jos käytät Google Colabia, niin et ehkä saa avattua dataa komennolla `df = pd.read_excel('https://taanila.fi/data1.xlsx')`. Suosittelen seuraavaa menettelyä:

* Luo Google Driveen kansio, jolle annat nimeksi **data**. 
* Lataa tarvittavat datat kyseiseen kansioon. [Pandas1](https://nbviewer.org/github/taanila/kuvaileva/blob/main/pandas1.ipynb)-muistion datan löydät osoitteesta [https://taanila.fi/data1.xlsx](https://taanila.fi/data1.xlsx).
* Lisää jokaisen muistion ensimmäiseen soluun koodi, joka yhdistää Google Driven data-kansion oletuskansioksi:

    `from google.colab import drive`  
    `drive.mount('/gdrive')`  
    `%cd /gdrive/MyDrive/data`

* Kun suoritat koodin, niin se kysyy lupaa kansion yhdistämiseen.
* Avaa data viittaamalla nettiosoitteen sijasta tiedoston nimeen `df = pd.read_excel('data1.xlsx')`.