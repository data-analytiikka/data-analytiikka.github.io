---
title: Grafiikka
layout: default
nav_order: 4
---

## Grafiikka

Graafisen esittämisen peruspaketti on **matplotlib**. Matplotlibin päälle rakennetun **seaborn**-paketin avulla voit tehdä grafiikkaa suoraan alkuperäisestä datasta ilman yhteenvetotaulukoiden laskentaa. Seabornin avulla voit mainiosti tutustua dataan jo ennen varsinaisten analyysien tekemistä.

Käytän esimerkeissä joitain vasta versioon 0.13 tulleita ominaisuuksia. Voit tarkistaa käyttämäsi version tuomalla seaborn-paketin `import seaborn as sns` ja suorittamalla sen jälkeen komennon `sns.__version__`. Päivitä tarvittaessa seaborn:

* Minicondassa ja Anacondassa komentorivillä komennolla `conda install seaborn -c conda-forge`. Parametri `-c conda-forge` määrittää että kanavana (channel) käytetään condan oletuskanavan sijasta conda-forge -kanavaa, josta löytyy monista paketeista oletuskanavaa uudempi versio.
* Colabissa on jo käytössä versio 0.13 tai uudempi.

Tässä osiossa tutustut joihinkin graafisen esittämisen perustapauksiin. Myöhemmissä osioissa palataan graafiseen esittämiseen ja seaborn-kirjastoon useasti.

* Oppimateriaalina on jypyter-muistio [seaborn](https://github.com/taanila/kaaviot/blob/master/seaborn.ipynb).

{: .new }
Harjoittele esimerkki-muistion esitystapoja myös joillain muilla datoilla. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`. Samoilla datoilla voit harjoitella ja kerrata myös edellisessä osiossa käsiteltyjä taitoja dataan tutustuminen, suodattaminen ja muuntaminen) 
