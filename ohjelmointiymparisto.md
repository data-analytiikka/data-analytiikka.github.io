---
title: Etusivu
layout: default
---


<p>Ensimmäiseksi tarvitset data-analytiikkaan sopivan muistio-tyyppisen ohjelmointiympäristön.</p>
<h2>Google Colab</h2>
<p>Jos et halua asentaa ympäristöä omalle koneellesi, niin voit käyttää ilmaista <strong>Google Colab</strong> -pilvipalvelua osoitteessa <a href="https://colab.research.google.com/" target="_blank" rel="noopener">https://colab.research.google.com/</a>. Palvelun käyttämiseen tarvitset Google-tunnuksen.</p>
<h2>Miniconda</h2>
<p>Omalle koneelle asennettavaksi ympäristöksi suosittelen <strong>Minicondaa</strong>.</p>
<p>Voit katsoa Minicondan asennuksen kulun <a href="https://video.haaga-helia.fi/media/miniconda/0_34c586jq" target="_blank" rel="noopener">videolta</a>.</p>
<p>Miniconda sisältää Pythonin ja <strong>conda</strong>-paketinhallintajärjestelmän. Minicondan asennus sujuu nopeasti.
<p>Löydät Minicondan Windowsille, Macille ja Linuxille osoitteesta</p>
<p style="padding-left: 40px"><a href="https://docs.conda.io/en/latest/miniconda.html" target="_blank" rel="noopener">https://docs.conda.io/en/latest/miniconda.html</a></p>
<p>Valitse oma käyttöjärjestelmäsi (Windows, macOS tai Linux) ja asenna Miniconda oletusasetuksilla.</p>
<p>Käynnistä asennuksen jälkeen Anacondan komentorivi:</p>
<ul>
<li>Windows-koneilla <strong>Miniconda3 &#8211; Anaconda prompt (miniconda3)</strong> Windowsin käynnistysvalikosta</li>
<li>MacOS- ja Linux-koneilla <strong>terminal/pääte</strong>.</li>
</ul>
<p>Komentorivillä voit asentaa tarvitsemasi kirjastot/paketit. Jokaisen asennuskomennon jälkeen kestää hetken ennen kuin conda löytää sinulle sopivan version, jonka jälkeen se kysyy vielä lupaa asennukseen. Vastaa kysymykseen y-kirjaimella (ja paina enter). Data-analytiikkaa varten tarvitset ainakin seuraavat:</p>
<ul>
<li><strong>conda install jupyter </strong>(Jupyter Notebook on data-analytiikassa suosittu ohjelmointiympäristö).</li>
<li><strong>conda install pandas </strong>(data-analytiikan peruskirjasto, jonka mukana asentuu myös numeerisen laskennan peruskirjasto numpy).</li>
<li><strong>conda install seaborn </strong>(grafiikka-kirjasto, jonka mukana asentuu myös grafiikan peruskirjasto matplotlib).</li>
<li><strong>conda install scikit-learn </strong>(koneoppimisen kirjasto, jonka mukana asentuu myös tieteellisen laskennnan peruskirjasto scipy).</li>
<li><strong>conda install statsmodels</strong> (tilastollisten mallien kirjasto mm. aikasarjaennustamiseen).</li>
<li><strong>conda install openpyxl</strong> (Excel-tiedostojen avaamiseen).</li>
<li><strong>conda install xlsxwriter</strong> (Excel-tiedostojen kirjoittamiseen).</li>
</ul>
<p>Myöhemmin voit tarpeen mukaan asentaa muita kirjastoja.</p>
<h2>Anaconda</h2>
<p>Anaconda sisältää muiden muassa</p>
<ul>
<li>Pythonin</li>
<li>datojen analysointiin tarvittavat ohjelmakirjastot (<strong>NumPy</strong>, <strong>pandas</strong>, jne.)</li>
<li>graafiseen esittämiseen tarvittavat ohjelmakirjastot (<b>matplotlib</b>, <b>seaborn</b> jne.)</li>
<li>koneoppimisen malleihin tarvittavat ohjelmakirjastot (<strong>scikit-learn</strong> jne.)</li>
<li><strong>Jupyter Notebook</strong>in ohjelmien kirjoittamiseen ja suorittamiseen</li>
<li><strong>Conda</strong>-paketinhallintajärjestelmän, jolla voit asentaa ja päivittää ohjelmakirjastoja (paketteja) siten että kirjastojen versiot ovat keskenään yhteensopivia.</li>
</ul>
<p>Löydät Anacondan Windowsille, Macille ja Linuxille osoitteesta</p>
<p style="padding-left: 40px"><a href="https://www.anaconda.com/products/distribution" target="_blank" rel="noopener noreferrer">https://www.anaconda.com/products/distribution</a></p>
<p>Valitse oma käyttöjärjestelmäsi (Windows, macOS tai Linux) ja asenna Anaconda oletusasetuksilla.</p>
<p>Ohjeita Anacondan käyttöön löydät osoitteesta</p>
<p style="padding-left: 40px"><a href="https://docs.anaconda.com/anaconda/" target="_blank" rel="noopener noreferrer">https://docs.anaconda.com/anaconda/</a></p>
<p>Anaconda sisältää paljon kirjastoja, joita et koskaan tarvitse. Jos haluat asentaa vain tarvitsemasi, niin asenna Anacondan sijasta Miniconda.</p>
<h2>Asennuksen jälkeen</h2>
<p>Tutustu asennuksen jälkeen <a href="https://tilastoapu.wordpress.com/2017/12/13/jupyter-2/" rel="noopener">Jupyter notebookin</a> toimintaan.</p>