# Sloan Digital Sky Survey Data Release 7 (spectra)

!!! Warning "Aviso"
    Página en construcción. Es posible que parte del contenido esté incompleto o desactualizado.




## Cargar usando LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/sdss_dr7_spectra')
```

---

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/sdss_dr7_spectra/
```

---

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
| --------------- | ------------------ | --------------------- | --------------- |
| 1,640,953        | 23                | 1,304                 | 86.2 GiB         |

<div class="button-container">
<a href="https://classic.sdss.org/dr7" class="button-link">Liberación Oficial</a>
<a href="https://ui.adsabs.harvard.edu/abs/2016arXiv161205560C/abstract" class="button-link">Artículo de Investigación</a>
</div>
