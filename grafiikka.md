---
title: Grafiikka
layout: default
nav_order: 4
---

## Grafiikka

Graafisen esittämisen peruspaketti on **matplotlib**. Matplotlibin päälle rakennetun **seaborn**-paketin avulla voit tehdä grafiikkaa suoraan alkuperäisestä datasta ilman yhteenvetotaulukoiden laskentaa. Seabornin avulla voit mainiosti tutustua dataan jo ennen varsinaisten analyysien tekemistä.

Tätä kirjoittaessani Minicondassa, Anacondassa ja Colabissa on oletuksena käytössä seabornin versio 12. Käytän esimerkeissä joitain version 13 ominaisuuksia, joten päivitä seaborn ennen esimerkkien suorittamista:

* Minicondassa ja Anacondassa komentorivillä komennolla `conda install seaborn -c conda-forge`. Parametri `-c conda-forge` määrittää että kanavana (channel) käytetään condan oletuskanavan sijasta conda-forge -kanavaa, josta löytyy monista paketeista oletuskanavaa uudempi versio.
* Colabissa voit päivittää seabornin suoraan muistiosta käsin kirjoittamalla ja suorittamalla komennon `!pip install seaborn==0.13`. Huutomerkki ohjaa komennon suoritettavaksi Colabin taustalla pyörivän Linuxin komentoriville. Colabissä pitää käyttää condan sijasta pip-paketinhallintajärjestelmää.

Tässä osiossa tutustut joihinkin graafisen esittämisen perustapauksiin. Myöhemmissä osioissa palataan graafiseen esittämiseen ja seaborn-kirjastoon useasti.

Oppimateriaali: [seaborn-muistio](https://nbviewer.org/github/taanila/kaaviot/blob/master/seaborn1.ipynb).

### Harjoitus

Harjoittele esimerkki-muistion esitystapoja myös jollain muilla datoilla. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`.

Samoilla datoilla voit harjoitella ja kerrata myös edellisessä osiossa käsiteltyjä taitoja (dataan tutustuminen, suodattaminen, muuntaminen). 


