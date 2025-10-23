# eROSITA-DE DR1 Main

O conjunto de telescópios eROSITA a bordo do satélite Spektrum Roentgen Gamma (SRG) iniciou o levantamento do céu em dezembro de 2019. O Data Release 1 (DR1) apresenta catálogos de raios X, arquivos de eventos calibrados, produtos de fontes e mapas de todo o céu do primeiro Levantamento de Todo o Céu eROSITA (eRASS1), que abrangeu seis meses de operações de dezembro de 2019 a junho de 2020. Este lançamento compreende dados cobrindo o hemisfério galáctico ocidental, a metade do céu proprietária do Consórcio Alemão eROSITA (eROSITA-DE).

Os dados do DR1 estão organizados em 2447 tiles do céu e fornecem catálogos de fontes em duas bandas primárias de raios X: um catálogo principal da faixa de energia mais sensível de 0,2–2,3 keV, e um catálogo duro da banda de 2,3–5,0 keV.

O catálogo principal eRASS1 resultante (0,2–2,3 keV) contém 930.203 entradas (903.521 fontes pontuais e 26.682 fontes estendidas) selecionadas com uma probabilidade de detecção DET_LIKE_0 ≥ 6 (ou EXT_LIKE > 0). Um catálogo menor de 5.466 fontes é apresentado da banda dura (2,3–5,0 keV), selecionado com DET_LIKE_3 ≥ 12. Este catálogo principal eRASS1 aumenta o número de fontes de raios X conhecidas na literatura publicada em mais de 60%.

As principais métricas de desempenho e características do levantamento incluem:

* **HEW mediano da PSF do levantamento (0,2–2,3 keV):** 30,0"
* **HEW mediano da PSF do levantamento (2,3–5,0 keV):** 34,4"
* **Limite de fluxo (0,5–2 keV, 50% de completude):** F(0,5–2 keV) > 5 × 10⁻¹⁴ erg s⁻¹ cm⁻²
* **Precisão de fluxo absoluto (0,5–2 keV):** ~6% de incerteza sistemática (relativo ao XMM-Newton)
* **Incerteza sistemática astrométrica:** σ₀ = 0,9" ± 0,1" (baseado no cruzamento QSO Gaia/unWISE)
* **Fração de fontes espúrias (Cat. Principal):** ~14% (para DET_LIKE_0 ≥ 6)
* **Fração de fontes espúrias (Cat. Duro):** ~8–10% (para DET_LIKE_3 ≥ 12)
* **Fração CXB resolvida (1–2 keV):** ~19% (valor mediano no limite de fluxo uniforme)

<figure class="dataset-figure">
<img src="../../images/erosita/eROSITA_DR1_Main.webp" alt="Mapa de Densidade Angular do eROSITA-DE DR1 Main">
<figcaption>Fonte da imagem: https://data.lsdb.io</figcaption>
</figure>

## Carregar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/erosita')
```

## Download com wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/erosita/
```

## Metadados do Catálogo

| Número de linhas | Número de colunas | Número de partições | Tamanho em disco |
|------------------|-------------------|---------------------|------------------|
| 930.203          | 255               | 10                  | 994 MB           |

<div class="button-container">
<a href="https://erosita.mpe.mpg.de/dr1" class="button-link">Lançamento Oficial</a>
<a href="https://erosita.mpe.mpg.de/dr1/AllSkySurveyData_dr1/Catalogues_dr1/MerloniA_DR1/eRASS1_Main.html" class="button-link">Descrições das Colunas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2024A%26A...682A..34M" class="button-link">Artigo de Pesquisa</a>
</div>
