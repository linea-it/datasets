# GALEX Merged Catalog of Sources

O GALEX Merged Catalog of Sources (MCAT) é o catálogo principal de fontes da missão Galaxy Evolution Explorer (GALEX), operada pela NASA entre 2003 e 2012. O telescópio realizou levantamentos do céu em duas bandas ultravioletas: far-UV (FUV, ~1350–1750 Å) e near-UV (NUV, ~1750–2800 Å).

O MCAT combina detecções de múltiplas observações individuais (visitas) para gerar uma lista consolidada de fontes únicas, fornecendo fotometria UV e propriedades básicas para centenas de milhões de objetos. Ele abrange diferentes profundidades de levantamento, desde o All-Sky Imaging Survey (AIS, mais raso, cobrindo ~26.000 graus²) até o Deep Imaging Survey (DIS, mais profundo, com exposições de dezenas de milhares de segundos).


<figure class="dataset-figure">
<img src="../../images/galex/point_density.webp" alt="Catálogo GALEX MCAT">
<figcaption>Fonte da imagem: https://data.lsdb.io</figcaption>
</figure>


---

## Carregar usando LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/galex')
```

---

## Download com wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/galex/
```

---

## Metadados do Catálogo

| Número de linhas | Número de colunas | Número de partições | Tamanho em disco | Versão do Builder               |
| ---------------- | ----------------- | ------------------- | ---------------- |---------------------------------|
| 292,296,119      | 368               | 1,595               | 343.7 GiB        | hats-import v0.9.2, hats v0.9.2 | 


<div class="button-container">
<a href="https://archive.stsci.edu/missions-and-data/galex" class="button-link">Lançamento Oficial</a>
<a href="https://www.galex.caltech.edu/wiki/Public:Documentation/Appendix_A.1" class="button-link">Descrições das Colunas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2017ApJS..230...24B/abstract" class="button-link">Artigo Científico</a>
</div>
