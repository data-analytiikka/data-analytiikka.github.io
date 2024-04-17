---
title: Automaattinen analysointi
layout: default
nav_order: 7
---

## Automaattinen analysointi

Paljon muuttujia sisältäville datoille ei kannata esimerkiksi frekvenssitaulukoita laskettaessa kirjoittaa koodia jokaista muuttujaa varten erikseen, vaan kannattaa automatisoida laskenta:

* Esimerkiksi frekvenssitaulukon laskentaan liittyvän koodin voi kirjoittaa omaksi funktioksi, jolle voi antaa parametriksi muuttujan.
* Koodissa voidaan kutsua omaa funktiota jokaiselle for-silmukassa läpikäytävälle muuttujalle.

[tilastoapu](https://nbviewer.org/github/taanila/selittava/blob/main/tilastoapu.ipynb)-muistiossa on luotu oma funktio frekvenssitaulukon (myös dikotomisille), ristiintaulukoinnin, tunnuslukujen, tunnuslukujen ryhmittäin ja korrelaatiokertoimien laskemiseen. Omissa funktioissa on käytetty aikaisemmissa osioissa opittuja laskentamentelmiä.

Omia funktioita kutsutaan koodissa for-silmukoiden sisältä. Muistion käyttäjän täytyy määritellä listoina kategoriset, dikotomiset ja määrälliset muuttujat. Näiden listojen mukaiset muuttujat käydään for-silmukoissa läpi.

Muistiossa käytetään XlsxWriter-moduulia, jonka avulla tulokset kirjoitetaan ja muotoillaan Excel-tiedostoon. Muistion koodien suorittamisen jälkeen tulokset sisältävä Excel-tiedosto löytyy samasta kansiosta kuin muistio.

Muistiossa ei ole selitetty XlsxWriterin käyttöä, mutta aiheesta kiinnostuneet löytävät hyvät käyttöohjeet osoitteesta [https://xlsxwriter.readthedocs.io/](https://xlsxwriter.readthedocs.io/). 

{: .new }
Harjoittele esimerkki-muistion käyttöä myös muilla datoilla. Sopivia datoja löytyy seaborn-kirjastosta. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('tips')`, `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`.
