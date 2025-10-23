# Dark Energy Survey – Data Release 2

El Dark Energy Survey – Data Release 2 (DES DR2) presenta imágenes reducidas de época única y coadicionadas, catálogos de fuentes y productos de datos asociados de seis años de operaciones científicas del DES (agosto de 2013–enero de 2019) utilizando la Dark Energy Camera (DECam) en el telescopio Blanco de 4 m en el Observatorio Interamericano de Cerro Tololo, Chile.

El DES DR2 comprende datos del sondeo de área amplia cubriendo aproximadamente 5000 deg² del hemisferio sur galáctico en cinco bandas fotométricas amplias (grizY). El lanzamiento consiste en 96.263 exposiciones de época única procesadas en 10.169 imágenes coadicionadas de 0,534 deg² cada una, derivadas de 76.217 exposiciones de calidad científica.

El catálogo resultante del DES DR2 contiene 691.483.608 objetos astronómicos distintos detectados a lo largo de la huella del sondeo. Después de la selección básica de calidad, las muestras de referencia incluyen 543 millones de galaxias y 145 millones de estrellas.

El sondeo logró fotometría uniforme y profunda, además de astrometría precisa. Las principales métricas de rendimiento incluyen:

* **FWHM mediano de la PSF**: g=1,11", r=0,95", i=0,88", z=0,83", Y=0,90"
* **Profundidad fotométrica** (apertura 1,95", S/N=10): g=24,7, r=24,4, i=23,8, z=23,1, Y=21,7 mag
* **Límite de completitud 95%**: g=24,6, r=24,3, i=24,0, z=23,7, Y=23,4 mag
* **Uniformidad fotométrica**: <3 mmag (1σ) relativo a la banda G del Gaia DR2
* **Precisión fotométrica absoluta**: ~11 mmag de incertidumbre sistemática
* **Precisión astrométrica**: ~27 mas (1σ) de precisión interna en la coadición
* **Tasa de objetos espurios**: ~1%
* **Separación estrella-galaxia**: >99% de eficiencia para galaxias, >94% de eficiencia para estrellas en 19,0<i<22,5

El DES DR2 constituye el mayor conjunto de datos fotométricos hasta la fecha en la profundidad y precisión fotométrica alcanzadas.

<figure class="dataset-figure">
<img src="../../images/des/DES_DR2.webp" alt="Mapa de Densidad Angular del DES DR2">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/des2/des_dr2')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/des2/des_dr2/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 662.428.385     | 215                | 1.523                | 667 GB          |

<div class="button-container">
<a href="https://www.darkenergysurvey.org/dr2/" class="button-link">Lanzamiento Oficial</a>
<a href="https://des.ncsa.illinois.edu/releases/dr2/dr2-access" class="button-link">Descripciones de Columnas</a>
<a href="https://arxiv.org/abs/2101.05765" class="button-link">Artículo de Investigación</a>
</div>
