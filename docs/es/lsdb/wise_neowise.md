# NEOWISE


!!! Warning "Aviso"
    Página en construcción. Es posible que parte del contenido esté incompleto o desactualizado.


## Cargar usando LSDB
 

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/wise/neowise/')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/wise/neowise/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 18,668,416,994 | 143 | 39,774 | 3.3 TiB | 

<div class="button-container">
<a href="https://wise2.ipac.caltech.edu/docs/release/neowise/neowise_2022_release_intro.html" class="button-link">Lanzamiento Oficial</a>
<a href="https://wise2.ipac.caltech.edu/docs/release/neowise/expsup/sec2_1a.html" class="button-link">Descripciones de las Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2014ApJ...792...30M%2F/abstract" class="button-link">Artículo Científico</a>
</div>
