# Pan-STARRS1 (objects)

!!! Warning "Aviso"
    Página en construcción. Es posible que parte del contenido esté incompleto o desactualizado.



## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/panstarrs/ps1_objects/')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/panstarrs/ps1_objects/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 10,560,724,292   | 134               | 27,161              | 2.7 TiB          |

<div class="button-container">
<a href="https://outerspace.stsci.edu/display/PANSTARRS/" class="button-link">Lanzamiento Oficial</a>
<a href="https://outerspace.stsci.edu/display/PANSTARRS/PS1+Database+object+and+detection+tables" class="button-link">Descripciones de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2016arXiv161205560C/abstract" class="button-link">Artículo de Investigación</a>
</div>
