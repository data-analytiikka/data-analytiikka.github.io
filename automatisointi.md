---
title: Automaattinen analysointi
layout: default
nav_order: 7
---

## Automaattinen analysointi

Paljon muuttujia sisältävälle datalle ei kannata esimerkiksi frekvenssitaulukoita laskettaessa kirjoittaa koodia jokaista muuttujaa varten erikseen, vaan kannattaa automatisoida laskenta:

* Frekvenssitaulukon laskentaan liittyvän koodin voi kirjoittaa omaksi funktioksi, jolle voi antaa parametriksi muuttujan nimen.
* Koodissa voidaan kutsua omaa funktiota jokaiselle for-silmukassa läpikäytävälle muuttujalle.

[tilastoapu](https://nbviewer.org/github/taanila/selittava/blob/main/tilastoapu.ipynb)-muistiossa on oma funktio frekvenssitaulukon (myös dikotomisille), ristiintaulukoinnin, tunnuslukujen (myös ryhmittäin) ja korrelaatiokertoimien laskemiseen. Omissa funktioissa on käytetty aikaisemmissa osioissa opittuja laskentamenetelmiä.

Omia funktioita kutsutaan koodissa for-silmukoiden sisältä. Muistion käyttäjän pitää määritellä listoina kategoriset, dikotomiset ja määrälliset muuttujat, jotta automatiikka osaa valita kullekin muuttujalle sopivat menetelmät. 

Muistiossa käytetään XlsxWriter-moduulia, jonka avulla tulokset kirjoitetaan ja muotoillaan Excel-tiedostoon. Muistion koodien suorittamisen jälkeen tulokset sisältävä Excel-tiedosto löytyy samasta kansiosta kuin muistio.

Muistiossa ei ole selitetty XlsxWriterin käyttöä, mutta aiheesta kiinnostuneet löytävät hyvät käyttöohjeet osoitteesta [https://xlsxwriter.readthedocs.io/](https://xlsxwriter.readthedocs.io/). 

{: .new }
Harjoittele esimerkki-muistion käyttöä myös muilla datoilla. Sopivia datoja löytyy seaborn-kirjastosta. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('tips')`, `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`.
