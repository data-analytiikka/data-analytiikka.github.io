---
title: Ohjelmointiympäristö
layout: default
nav_order: 1
---

## Ohjelmointiympäristö

Data-analytiikassa kannattaa käyttää koodin kirjoittamiseen ja suorittamiseen muistio-tyyppistä ohjelmointiympäristöä. Suosittelen **Miniconda**n, **Anaconda**n tai **Google Colab**in käyttöä. Kaikissa edellä mainituissa käytetään [jupyteriin](https://jupyter.org/) perustuvaa muistio-tyyppistä ympäristöä.

### Miniconda

Omalle koneelle asennettavaksi ympäristöksi suosittelen Minicondaa. Lue kuitenkin [Minicondan ja Anacondan vertailu](https://docs.anaconda.com/free/distro-or-miniconda/) ennen kuin valitset Mincondan ja Anacondan väliltä.

Minicondan löydät osoitteesta [https://docs.anaconda.com/free/miniconda/](https://docs.anaconda.com/free/miniconda/). Valitse oma käyttöjärjestelmäsi (Windows, MacOS tai Linux) ja asenna Miniconda oletusasetuksilla.

Miniconda sisältää Pythonin ja conda-paketinhallintajärjestelmän. Data-analytiikassa tarvittavat lisäpaketit täytyy asentaa Minicondan asennuksen jälkeen condan avulla: 

* Käynnistä asennuksen jälkeen Minicondan komentorivi:
    - Windows-koneilla Windowsin käynnistysvalikosta **Miniconda - Anaconda prompt (miniconda3)**
    - MacOS- ja Linux-koneilla **terminal/pääte**.
* Komentorivillä voit asentaa tarvitsemasi paketit. Jokaisen asennuskomennon jälkeen kestää hetken ennen kuin conda löytää sinulle sopivan version, jonka jälkeen se kysyy lupaa asennukseen. Vastaa kysymykseen **y**-kirjaimella ja paina **enter**. Data-analytiikkaa varten tarvitset ainakin seuraavat asennukset:
    - `conda install jupyter` (koodin kirjoittamiseen ja suorittamiseen käytettävä ohjelmointiympäristö)
    - `conda install pandas` (data-analytiikan peruspaketti, jonka mukana asentuu myös numeerisen laskennan peruspaketti numpy)
    - `conda install seaborn` (grafiikka-paketti, jonka mukana asentuu myös grafiikan peruspaketti matplotlib)
    - `conda install scikit-learn` (koneoppimisen paketti, jonka mukana asentuu myös tieteellisen laskennnan peruspaketti scipy)
    - `conda install statsmodels` (tilastollisten mallien paketti, josta löytyy mm. aikasarjaennustamisen menetelmiä)
    - `conda install openpyxl` (Excel-tiedostojen avaamiseen)
    - `conda install xlsxwriter` (Excel-tiedostojen kirjoittamiseen).

Myöhemmin voit tarpeen mukaan asentaa muita paketteja.

Tutustu asennuksen jälkeen [jupyterin](https://tilastoapu.wordpress.com/2017/12/13/jupyter-2/) toimintaan. Jupyterin voit käynnistää Minicondan komentoriviltä komennolla `jupyter notebook`.

### Anaconda

Anaconda sisältää valmiiksi asennettuna jupyterin ja useimmat data-analytiikassa tarvittavat paketit. Asennusohjeet löydät osoitteesta [https://docs.anaconda.com/free/anaconda/install/](https://docs.anaconda.com/free/anaconda/install/).

Tutustu asennuksen jälkeen [jupyterin](https://tilastoapu.wordpress.com/2017/12/13/jupyter-2/) toimintaan.

### Google Colab

Jos et halua asentaa ympäristöä omalle koneellesi, niin voit käyttää ilmaiseksi pilvipalvelua [Google Colab](https://colab.research.google.com/). Palvelun käyttämiseen tarvitset Google-tunnuksen. Colab sisältää valmiiksi asennettuina useimmat data-analytiikassa tarvittavat paketit.

Voit käynnistää Googlen version jupyteristä valitsemalla Colabin **File/Tiedosto**-valikosta **New notebook/Uusi työkirja**. Colabillä kirjoitetut muistiot tallentuvat Google Driveen.

Jos Google Colab käynnistyy suomenkielisenä, niin voit halutessasi vaihtaa sen englanninkieliseksi valitsemalla **Ohje**-valikosta **Näytä englanniksi**.
