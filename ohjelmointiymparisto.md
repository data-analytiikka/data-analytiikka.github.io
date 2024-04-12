---
title: Ohjelmointiympäristö
layout: default
nav_order: 1
---

# Ohjelmointiympäristö

Data-analytiikassa kannattaa käyttää koodin kirjoittamiseen ja suorittamiseen muistio-tyyppistä ohjelmointiympäristöä. Suosittelen Google Colabin tai Minicondan käyttöä.

## Google Colab

Jos et halua asentaa ympäristöä omalle koneellesi, niin voit käyttää ilmaiseksi pilvipalvelua [Google Colab](https://colab.research.google.com/). Palvelun käyttämiseen tarvitset Google-tunnuksen.

## Miniconda

Omalle koneelle asennettavaksi ympäristöksi suosittelen [Minicondaa](https://docs.conda.io/en/latest/miniconda.html).

Valitse oma käyttöjärjestelmäsi (Windows, macOS tai Linux) ja asenna Miniconda oletusasetuksilla.

Miniconda sisältää Pythonin ja conda-paketinhallintajärjestelmän. Data-analytiikassa tarvittavat lisäpaketit täytyy asentaa condan avulla: 

* Käynnistä asennuksen jälkeen Anacondan komentorivi:
    - Windows-koneilla **Miniconda - Anaconda prompt (miniconda3)** Windowsin käynnistysvalikosta.
    - MacOS- ja Linux-koneilla **terminal/pääte**.
* Komentorivillä voit asentaa tarvitsemasi paketit. Jokaisen asennuskomennon jälkeen kestää hetken ennen kuin conda löytää sinulle sopivan version, jonka jälkeen se kysyy vielä lupaa asennukseen. Vastaa kysymykseen y-kirjaimella ja paina enter. Data-analytiikkaa varten tarvitset ainakin seuraavat asennukset:
    - conda install jupyter (jupyter on koodin kirjoittamiseen ja suorittamiseen tarvittava muistio-tyyppinen sovellus)
    - conda install pandas (data-analytiikan peruskirjasto, jonka mukana asentuu myös numeerisen laskennan peruskirjasto numpy)
    - conda install seaborn (grafiikka-kirjasto, jonka mukana asentuu myös grafiikan peruskirjasto matplotlib)
    - conda install scikit-learn </strong>(koneoppimisen kirjasto, jonka mukana asentuu myös tieteellisen laskennnan peruskirjasto scipy)
    - conda install statsmodels (tilastollisten mallien kirjasto mm. aikasarjaennustamiseen)
    - conda install openpyxl</strong> (Excel-tiedostojen avaamiseen)
    - conda install xlsxwriter (Excel-tiedostojen kirjoittamiseen).

Myöhemmin voit tarpeen mukaan asentaa muita kirjastoja.

Tutustu asennuksen jälkeen [jupyter-muistion](https://tilastoapu.wordpress.com/2017/12/13/jupyter-2/) toimintaan.
