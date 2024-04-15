---
title: Kuvaileva analytiikka
layout: default
nav_order: 5
---

## Kuvaileva analytiikka

Kuvailevan analytiikan menetelmä määräytyy muuttujan tyypistä:

* Kategoriselle muuttujalle lasketaan frekvenssitaulukko.
* Määrälliselle muuttujalle lasketaan luokiteltu frekvenssitaulukko ja/tai tilastollisia tunnuslukuja.

### Frekvenssitaulukko kategoriselle muuttujalle

[Frekvenssijakauma-muistiossa](https://nbviewer.org/github/taanila/kuvaileva/blob/main/frekvenssijakauma.ipynb) on esimerkki frekvenssitaulukon laskemisesta ja sen havainnollistamisesta pylväskaaviona.

Dikotomisille muuttujille halutaan usein esittää monen dikotomisen muuttujan frekvenssit kootusti samassa taulukossa. Katso esimerkki muistiosta [dummy_kuvaileva](https://nbviewer.org/github/taanila/kuvaileva/blob/main/dummy_kuvaileva.ipynb).

### Luokiteltu frekvenssitaulukko määrälliselle muuttujalle

Muistio [luokiteltu_jakauma](https://nbviewer.org/github/taanila/kuvaileva/blob/main/luokiteltu_jakauma.ipynb) opettaa laskemaan luokitellun frekvenssitaulukon ja havainnollistamaan sitä histogrammina.

### Tilastollisia tunnuslukuja määrälliselle muuttujalle

Muistiossa [tunnuslukuja](https://nbviewer.org/github/taanila/kuvaileva/blob/main/tunnuslukuja.ipynb) lasketaan tilastollisia tunnuslukuja ja havainollistetaan niitä ruutu- ja janakaaviona (boxplot).

### Harjoitus

Harjoittele esimerkki-muistioiden esitystapoja myös muilla datoilla. Sopivia datoja löytyy seaborn-kirjastosta. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('tips')`, `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`.
