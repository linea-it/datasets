# AllWISE


!!! Warning "Aviso"
    Página en construcción. Es posible que parte del contenido esté incompleto o desactualizado.



## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/wise/allwise/')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/wise/allwise/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 747,634,026      | 299              |	768                  |	258.0 GiB   |


<div class="button-container">
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/" class="button-link">Lanzamiento Oficial</a>
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html" class="button-link">Descripción de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2010AJ....140.1868W/abstract" class="button-link">Paper de Investigación</a>
</div>
