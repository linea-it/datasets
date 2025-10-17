# Dark Energy Survey Y6 Gold

El Dark Energy Survey Year 6 (DES Y6) Gold presenta un conjunto de datos fotométricos curados derivado de los seis años completos de observaciones del DES (agosto de 2013–enero de 2019) utilizando la Dark Energy Camera en el telescopio Blanco de 4m en el Observatorio Interamericano de Cerro Tololo, Chile, específicamente optimizado para análisis de cosmología de cielo estático.

El DES Y6 Gold está ensamblado a partir del Dark Energy Survey Data Release 2 y comprende aproximadamente 5000 deg² de imágenes grizY en el hemisferio sur galáctico. El conjunto de datos incorpora fotometría multi-época avanzada, calibración mejorada, clasificación de objetos mejorada y productos auxiliares comprensivos, incluyendo máscaras de huella, mapas de propiedades del sondeo y estimaciones de corrimiento al rojo fotométrico.

El catálogo resultante Y6 Gold contiene 669 millones de objetos de alta calidad detectados a lo largo de la huella del sondeo. Después de las selecciones de calidad, las muestras de referencia incluyen 448 millones de galaxias y 120 millones de estrellas.

El sondeo logró fotometría uniforme y profunda con astrometría precisa y clasificación robusta de objetos. Las principales métricas de rendimiento incluyen:

* **FWHM mediano de la PSF**: g=1,13", r=0,99", i=0,90", z=0,87", Y=0,93"
* **Cobertura del Sondeo**: 4923 deg² (requiriendo ≥2 exposiciones en griz)
* **Profundidad fotométrica** (apertura 1,95", S/N=10): g=24,7, r=24,4, i=23,8, z=23,1, Y=21,7 mag
* **Profundidad de galaxias multi-época** (S/N=10, modelo BDF): i=23,4 mag
* **Límite de completitud 90%** (objetos extendidos): g=23,9, r=23,2, i=22,7, z=22,4 mag
* **Uniformidad fotométrica**: <2 mmag relativo a la banda G del Gaia
* **Precisión astrométrica**: ~27 mas (precisión interna mediana)
* **Clasificación estrella-galaxia** (17,5≤i≤22,5): Eficiencia de galaxias 98,6% con 0,8% de contaminación; Eficiencia estelar 94,6% con 1,5% de contaminación
* **Densidad de objetos**: 37,4 arcmin⁻² en total; 28,9 arcmin⁻² para galaxias de alta confianza

<figure class="dataset-figure">
<img src="../../images/des/DES_Y6_Gold.webp" alt="Mapa de Densidad Angular del Dark Energy Survey Y6 Gold">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/des/des_y6_gold')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/des/des_y6_gold/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 691.483.608     | 336                | 1.582                | 1,3 TiB         |

<div class="button-container">
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6gold" class="button-link">Lanzamiento Oficial</a>
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6gold" class="button-link">Descripciones de Columnas</a>
<a href="https://arxiv.org/abs/2501.05739" class="button-link">Artículo de Investigación</a>
</div>
