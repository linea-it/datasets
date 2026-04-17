# NEOWISE

!!! Warning "Aviso"
    Página em construção. 





## Carregar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/wise/neowise/')
```

## Download com wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/wise/neowise/
```

## Metadados do Catálogo

| Número de linhas | Número de colunas | Número de partições | Tamanho em disco |
|-----------------|-------------------|----------------------|-----------------|
| 18,668,416,994 | 143 | 39,774 | 3.3 TiB | 

<div class="button-container">
<a href="https://wise2.ipac.caltech.edu/docs/release/neowise/neowise_2022_release_intro.html" class="button-link">Lançamento Oficial</a>
<a href="https://wise2.ipac.caltech.edu/docs/release/neowise/expsup/sec2_1a.html" class="button-link">Descrições das Colunas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2014ApJ...792...30M%2F/abstract" class="button-link">Artigo Científico</a>
</div>
