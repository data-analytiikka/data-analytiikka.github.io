---
title: Selittävä analytiikka
layout: default
nav_order: 6
---

## Selittävä analytiikka

Selittävässä analytiikassa on mukana vähintään kaksi muuttujaa, joiden välisestä yhteydestä/riippuvuudesta ollaan kiinnostuneita. Usein toinen muuttujista on selittävän muuttujan asemassa. Selittävän analytiikan menetelmän valinta riippuu tarkasteltavien muuttujien tyypeistä:

* Jos **molemmat muuttujat ovat kategorisia**, niin käytetään ristiintaulukointia.
* Jos **selittävä muuttuja on määrällinen** ja **toinen muuttuja on kategorinen**, niin käytetään ristiintaulukointia. Tällöin selittävän muuttujan arvot täytyy luokitella. Luokittelusta lisätietoa edellisen osion [luokiteltu_jakauma](https://github.com/taanila/kuvaileva/blob/main/luokiteltu_jakauma.ipynb)-muistiossa.
* Jos **selittävä muuttuja on kategorinen** ja **toinen muuttuja on määrällinen**, niin vertaillaan tunnuslukuja selittävän muuttujan määräämissä ryhmissä.
* Jos **molemmat muuttujat ovat määrällisiä**, niin käytetään hajontakaaviota ja korrelaatiokerrointa.

### Ristiintaulukointi

* Oppimateriaalina on [ristiintaulukointi](https://github.com/taanila/selittava/blob/main/ristiintaulukointi.ipynb)-muistio. Muistiossa on mukana myös graafisia esityksiä pylväskaavioina.
* Dikotomisten muuttujien oppimateriaalina on [dummy_selittava](https://github.com/taanila/selittava/blob/main/dummy_selittava.ipynb)-muistio.

### Tunnuslukujen vertailu

* Oppimateriaalina on [tunnuslukujen vertailu](https://github.com/taanila/selittava/blob/main/tunnuslukujen_vertailu.ipynb) -muistio. Muistiossa on mukana myös graafisia esityksiä ruutu-ja janakaavioina.
* Lisäesimerkkejä [groupby](https://github.com/taanila/data/blob/main/groupby.ipynb)-muistiossa.
* Lisäesimerkkejä [pivot](https://github.com/taanila/selittava/blob/main/pivot.ipynb)-muistiossa, jossa opit tekemään monenlaisia yhteenvetoja pivot-taulukoinnilla.

### Hajontakaavio ja Korrelaatio

* Oppimateriaalina on [korrelaatio](https://github.com/taanila/selittava/blob/main/korrelaatio.ipynb)-muistio.

{: .new }
Harjoittele esimerkki-muistioiden esitystapoja myös muilla datoilla. Sopivia datoja löytyy seaborn-kirjastosta. Kokeile esimerkiksi seuraavilla komennoilla aukeavia datoja: `sns.load_dataset('tips')`, `sns.load_dataset('penguins')`, `sns.load_dataset('diamonds')`, `sns.load_dataset('taxis')`.
