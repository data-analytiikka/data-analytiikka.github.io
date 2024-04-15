---
title: Kuvaileva analytiikka
layout: default
nav_order: 5
---

# Kuvaileva analytiikka

Kuvailevan analytiikan menetelmän valinta riippuu muuttujan tyypistä:

* Kategoriselle muuttujalle lasketaan frekvenssitaulukko.
* Määrälliselle muuttujalle lasketaan luokiteltu frekvenssitaulukko ja/tai tilastollisia tunnuslukuja.

# Frekvenssitaulukko kategoriselle muuttujalle

[Frekvenssijakauma-muistiossa](https://nbviewer.org/github/taanila/kuvaileva/blob/main/frekvenssijakauma.ipynb) on esimerkki frekvenssitaulukon laskemisesta ja sen havainnollistamisesta pylväskaaviona.

Dikotomisille muuttujille halutaan usein esittää monen dikotomisen muuttujan frekvessit kootusti samassa taulukossa. Katso esimerkki [muistiosta](https://nbviewer.org/github/taanila/kuvaileva/blob/main/dummy_kuvaileva.ipynb)

# Luokiteltu frekvenssitaulukko määrälliselle muuttujalle

[Luokiteltu frekvenssitaulukko -muistio](https://nbviewer.org/github/taanila/kuvaileva/blob/main/luokiteltu_jakauma.ipynb) opettaa laskemaan luokitellun frekvenssitaulukon ja havainnollistamaan sitä histogrammina.

# Tilastollisia tunnuslukuja määrälliselle muuttujalle

[Tunnuslukuja-muistiossa](https://nbviewer.org/github/taanila/kuvaileva/blob/main/tunnuslukuja.ipynb) lasketaan tilastollisia tunnuslukuja ja havainollistetaan niitä ruutu- ja janakaaviona (boxplot).

## Harjoitus

Harjoittele esimerkkimuistioiden esitystapoja myös jollain muulla datalla. Sopivia datoja löytyy seaborn-kirjastosta: Esimerkiksi `sns.load_dataset('tips')`, `sns.load_dataset('penguins')` tai `sns.load_dataset('diamonds')` tai `sns.load_dataset('taxis')`.


