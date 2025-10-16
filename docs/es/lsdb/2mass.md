
# Two Micron All Sky Survey (2MASS)

El Two Micron All Sky Survey (2MASS) recopiló 25,4 Tbytes de datos de imagen en bruto entre junio de 1997 y febrero de 2001, cubriendo el 99,998% de la esfera celeste en las bandas del infrarrojo cercano J (1,25 μm), H (1,65 μm) y Ks (2,16 μm). Las observaciones se realizaron utilizando dos telescopios dedicados de 1,3 m en Mount Hopkins, Arizona, y Cerro Tololo, Chile.

El lanzamiento de datos 2MASS All-Sky resultante comprende 4.121.439 imágenes FITS y catálogos derivados del procesamiento final de datos. Los principales productos de datos incluyen un Catálogo de Fuentes Puntuales de 470.992.970 fuentes y un Catálogo de Fuentes Extendidas de 1.647.599 objetos.

La encuesta logró fotometría y astrometría uniformes y precisas. Las principales métricas de rendimiento para el Catálogo de Fuentes Puntuales incluyen:

* Sensibilidad (S/N=10): Mejor que J=15,8, H=15,1 y Ks=14,3 mag para virtualmente todo el cielo.
* Confiabilidad: Mayor que 99,95% para fuentes con S/N ≥ 10 en cualquier banda.
* Completitud: Mayor que 99% para fuentes con S/N ≥ 10 en cualquier banda.
* Precisión Fotométrica (Fuentes Brillantes): <0,03 mag (1σ).
* Precisión Astrométrica: ~100 mas (1σ) relativo al ICRS.
* Rango Dinámico: >20 mag.

Los productos de datos están públicamente disponibles a través del lanzamiento de datos 2MASS All-Sky.

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.lsdb.io/hats/two_mass')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.lsdb.io/hats/two_mass/
```

## Metadatos del catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 470,992,970     | 63                | 1,107                | 43 GB           |

<div class="button-container">
<a href="https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec2_2.html" class="button-link">Lanzamiento Oficial</a>
<a href="https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec2_2a.html" class="button-link">Descripciones de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2006AJ....131.1163S/abstract" class="button-link">Publicación Científica</a>
</div>
