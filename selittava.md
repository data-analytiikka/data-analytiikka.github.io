---
title: Selittävä analytiikka
layout: default
nav_order: 6
---

# Selittävä analytiikka

Selittävässä analytiikassa on mukana vähintään kaksi muuttujaa, joiden välisestä yhteydestä/riippuvuudesta ollaan kiinnostuneita. Usein toinen muuttujista on selittävän muuttujan asemassa. Selittävän analytiikan menetelmän valinta riippuu tarkasteltavien muuttujien tyypistä:

* Jos molemmat muuttujat ovat kategorisia, niin käytetään ristiintaulukointia.
* Jos selittävä muuttuja on määrällinen, mutta toinen muuttuja kategorinen, niin voidaan käyttää ristiintaulukointia. Tällöin selittävän muuttujan arvot täytyy luokitella. Luokittelusta lisätietoa edellisen osion [luokiteltu frekvenssitaulukko -muistiossa](https://nbviewer.org/github/taanila/kuvaileva/blob/main/luokiteltu_jakauma.ipynb).
* Jos selittävä muuttuja on kategorinen, mutta toinen muuttuja on määrällinen, niin voidaan laskea tunnuslukuja selittävän muuttujan määräämissä ryhmissä.
* Jos molemmat muuttujat ovat määrällisiä, niin voidaan käyttää hajontakaaviota ja korrelaatiokerrointa.

# Ristiintaulukointi

Ristiintaulukoinnit opit [ristiintaulukointi-muistiosta](https://nbviewer.org/github/taanila/selittava/blob/main/ristiintaulukointi.ipynb). Muistiossa havainnollistetaan ristiintaulukointeja myös pylväskaavioina.

Dikotomisten muuttujien kanssa toimitaan [muistion](https://nbviewer.org/github/taanila/selittava/blob/main/dummy_selittava.ipynb) mukaisesti. 

# Tunnuslukujen vertailu

Tunnuslukujen vertailua selittävän muuttujan määräämien ryhmien välillä opit [tunnuslukujen vertailu -muistiosta](https://nbviewer.org/github/taanila/selittava/blob/main/tunnuslukujen_vertailu.ipynb). Muistiossa mukana myös graafinen havainnollistaminen ruutu-ja janakaaviona.
Lisäesimerkkejä [Ryhmittelyjä groupby-funktiolla -muistiossa](https://nbviewer.org/github/taanila/data/blob/main/groupby.ipynb).

Kannattaa myös tutustua [pivot-taulukot -muistioon](https://nbviewer.org/github/taanila/selittava/blob/main/pivot.ipynb).

# Korrelaatio

[korrelaatio-muistiossa](https://nbviewer.org/github/taanila/selittava/blob/main/korrelaatio.ipynb).

## Harjoitus

Harjoittele esimerkkimuistioiden esitystapoja myös jollain muulla datalla. Sopivia datoja löytyy seaborn-kirjastosta: Esimerkiksi `sns.load_dataset('tips')`, `sns.load_dataset('penguins')` tai `sns.load_dataset('diamonds')` tai `sns.load_dataset('taxis')`.

