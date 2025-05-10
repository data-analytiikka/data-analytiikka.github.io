
title: Python + pandas
layout: default
nav_order: 2
---

## Python + pandas

Tässä osiossa on tarkoituksena:

* tutustua alustavasti Python-koodaukseen
* tutustua alustavasti data-analytiikan **pandas**-pakettiin.

### Opiskeluohjeita

* Oppimateriaalina on jupyter-muistio [pandas1](https://nbviewer.org/github/taanila/kuvaileva/blob/main/pandas1.ipynb).
* Lue huolellisesti muistion selitykset ja kommentit.
* Kirjoita koodisolujen koodit omaan muistioon. Siirry seuraavaan soluun vasta kun saat solun koodin onnistuneesti suoritettua. Pienimmätkin kirjoitusvirheet aiheuttavat virheilmoituksen. Virheilmoitukset ovat usein vaikeasti tulkittavia, mutta virheilmoituksesta yleensä selviää ainakin millä koodirivillä virhe sijaitsee. Virheilmoituksen viimeiseltä riviltä saatat löytää ymmärrettävän selityksen virheestä.
* Jos koodissa jokin asia askarruttaa, niin kannattaa tehdä omia kokeiluja ja kokeilla vaihtoehtoisia koodeja.
* Lisää omaan muistioosi omia kommentteja ja huomioita. Koodisoluun voit lisätä kommenttirivin kirjoittamalla rivin alkuun risuaidan **#**. Pidempiä tekstejä voit kirjoittaa **Markdown**-soluihin (Colabissa **Text**-soluihin).
* Tässä ensimmäisessä muistiossa on häkellyttävän paljon opittavaa. Tähän kannattaa käyttää aikaa, koska näin luot hyvän pohjan tulevien osioiden oppimiselle. Kaikkiin tämän muistion asioihin palataan myöhemmissä osioissa.

{: .important }
Kun avaat aiemmin kirjoitetun muistion, niin voit suorittaa kaikkien solujen koodit **Run**-valikon komennolla **Run All Cells** (Colabissa **Runtime - Run all** / **Suorituspalvelu - Suorita kaikki**). Komento auttaa myös, jos jostain syystä ajaudut umpikujaan koodin suorituksessa. Näin voi käydä, jos esimerkiksi korjailet ja suorittelet välillä aiempien solujen koodeja.

### Google Colabin käyttäjille

{: .warning }
Jos käytät Google Colabia, niin et ehkä saa avattua dataa komennolla `df = pd.read_excel('https://taanila.fi/data1.xlsx')`. Suosittelen seuraavaa menettelyä:

* Luo Google Driveen kansio, jolle annat nimeksi **data**. 
* Lataa tarvittavat datat kyseiseen kansioon. Osoitteesta [https://taanila.fi/data1.xlsx](https://taanila.fi/data1.xlsx) löydät esimerkki-muistion datan.
* Lisää jokaisen muistion ensimmäiseen soluun koodi, joka yhdistää Google Driven data-kansion oletuskansioksi:<br>
    `from google.colab import drive`  
    `drive.mount('/gdrive')`  
    `%cd /gdrive/MyDrive/data`
* Kun suoritat koodin, niin se kysyy lupaa kansion yhdistämiseen.
* Avaa data viittaamalla nettiosoitteen sijasta ainoastaan tiedoston nimeen `df = pd.read_excel('data1.xlsx')`.
