# AllWISE


!!! Warning "Aviso"
    Página em construção. 





## Carregar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/wise/allwise/')
```

## Download com wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/wise/allwise/
```


## Metadados do Catálogo

| Número de linhas | Número de colunas | Número de partições | Tamanho em disco |
|-----------------|-------------------|----------------------|-----------------|
| 747,634,026      | 299              |	768                  |	258.0 GiB   |


<div class="button-container">
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/" class="button-link">Lançamento Oficial</a>
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html" class="button-link">Descrições das Colunas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2010AJ....140.1868W/abstract" class="button-link">Artigo Científico</a>
</div>
