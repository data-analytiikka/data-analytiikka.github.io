---
title: Aikasarjaennustaminen
layout: default
nav_order: 9
---

# Aikasarjaennustaminen

Aikasarjaennustamisessa oletetaan että jo toteutunut aikasarja sisältää tietoa, joka auttaa tulevan aikasarjan ennustamisessa.

{: .important }
Aikasarjaennustaminen ei sovi kaikille aikasarjoille. Esimerkiksi pörssiosakkeiden hintaa ei yleensä kannata ennustaa aikasarjaennustamisen menetelmillä.

Tässä osiossa opit kolme erilaista eksponentiaalisen tasoituksen menetelmää. Nämä ovat suosittuja esimerkiksi kysynnän ennustamisessa.

* [forecast1](https://github.com/taanila/aikasarjat/blob/main/forecast1.ipynb)-muistiossa käytetään yksinkertaista eksponentiaalista tasoitusta. Tämä menetelmä sopii aikasarjalle, jossa ei ole tunnistettavaa trendiä tai kausivaihtelua.
* [forecast2](https://github.com/taanila/aikasarjat/blob/main/forecast2.ipynb)-muistiossa käytetään kaksinkertaista eksponentiaalista tasoitusta eli Holtin mallia. Tämä menetelmä sopii aikasarjalle, jossa on trendi.
* [forecast3](https://github.com/taanila/aikasarjat/blob/main/forecast3.ipynb)-muistiossa käytetään kolminkertaista eksponentiaalista tasoitusta eli Holt-Wintersin mallia. Tämä menetelmä sopii aikasarjalle, jossa on sekä trendi että kausivaihtlu.

{: .new }
Harjoittele aikasarjaennustamista datalla [https://taanila.fi/AirPassengers.csv](https://taanila.fi/AirPassengers.csv). Data on csv-muodossa (comma separated value) ja sen avaamiseen täytyy käyttää **read_csv**-funktiota: `df = pd.read_csv('https://taanila.fi/AirPassengers.csv')`.
