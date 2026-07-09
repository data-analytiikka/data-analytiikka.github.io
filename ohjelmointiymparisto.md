---
title: Ohjelmointiympäristö
layout: default
nav_order: 1
---

## Ohjelmointiympäristö

Data-analytiikassa kannattaa käyttää koodin kirjoittamiseen ja suorittamiseen muistio-tyyppistä ohjelmointiympäristöä. Suosittelen **Miniforge**n tai **Google Colab**in käyttöä.

### Miniforge

Omalle koneelle asennettavaksi ympäristöksi suosittelen Miniforgea. Miniforgen löydät osoitteesta [https://conda-forge.org/download/](https://conda-forge.org/download/). Valitse oma käyttöjärjestelmäsi (Windows, MacOS tai Linux) ja asenna Miniconda oletusasetuksilla.

Miniforge sisältää Pythonin ja conda-paketinhallintajärjestelmän. Data-analytiikassa tarvittavat lisäpaketit voit asentaa Miniforgen asennuksen jälkeen condan avulla: 

* Käynnistä asennuksen jälkeen Miniforgen komentorivi:
    - Windows-koneilla Windowsin käynnistysvalikosta **Miniforge Prompt**
    - MacOS- ja Linux-koneilla **terminal/pääte**.
* Komentorivillä voit asentaa tarvitsemasi paketit. Jokaisen asennuskomennon jälkeen kestää hetken ennen kuin conda löytää sinulle sopivan version, jonka jälkeen se kysyy lupaa asennukseen. Vastaa kysymykseen **y**-kirjaimella ja paina **enter**. Data-analytiikkaa varten tarvitset ainakin seuraavat asennukset:
    - `conda install jupyter` (koodin kirjoittamiseen ja suorittamiseen käytettävä ohjelmointiympäristö)
    - `conda install pandas` (data-analytiikan peruspaketti, jonka mukana asentuu myös numeerisen laskennan peruspaketti numpy)
    - `conda install seaborn` (grafiikka-paketti, jonka mukana asentuu myös grafiikan peruspaketti matplotlib, tieteellisen laskennan paketti scipy ja tilastollisten mallien paketti statsmodels)
    - `conda install scikit-learn` (koneoppimisen paketti)
    - `conda install openpyxl` (Excel-tiedostojen avaamiseen)
    - `conda install xlsxwriter` (Excel-tiedostojen kirjoittamiseen).

Myöhemmin voit tarpeen mukaan asentaa muita paketteja.

Tutustu asennuksen jälkeen [jupyter-muistion](https://tilastoapu.wordpress.com/2017/12/13/jupyter-2/) toimintaan. Jupyterin voit käynnistää Miniforgen komentoriviltä komennolla `jupyter notebook`.

### Google Colab

Jos et halua asentaa ympäristöä omalle koneellesi, niin voit käyttää ilmaiseksi pilvipalvelua [Google Colab](https://colab.research.google.com/). Palvelun käyttämiseen tarvitset Google-tunnuksen. Colab sisältää valmiiksi asennettuina useimmat data-analytiikassa tarvittavat paketit.

Voit käynnistää Googlen muistio-tyyppisen ohjelmointiympäristön valitsemalla Colabin **File/Tiedosto**-valikosta **New notebook/Uusi työkirja**. Colabillä kirjoitetut muistiot tallentuvat Google Driveen.

Jos Google Colab käynnistyy suomenkielisenä, niin voit halutessasi vaihtaa sen englanninkieliseksi valitsemalla **Ohje**-valikosta **Näytä englanniksi**.
