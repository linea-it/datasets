# Gaia Data Release 3

El Gaia Data Release 3 (DR3) presenta una actualización significativa de los datos de la misión Gaia de la Agencia Espacial Europea, expandiendo sustancialmente el Early Third Data Release (Gaia EDR3). Aunque repite la astrometría (posiciones, paralajes, movimientos propios) y fotometría de banda ancha (G, GBP, GRP) para aproximadamente 1,8 mil millones de fuentes del Gaia EDR3, el Gaia DR3 introduce una riqueza de nueva información astrofísica derivada de los primeros 34 meses de datos de la misión. Este lanzamiento constituye la mayor colección hasta la fecha de espectrofotometría de todo el cielo, velocidades radiales, información de variabilidad y parámetros astrofísicos.

El catálogo Gaia DR3 incorpora datos del instrumento astrométrico de Gaia (banda G: 330–1050 nm), los fotómetros BP/RP (proporcionando espectros de baja resolución cubriendo 330–680 nm y 640–1050 nm, respectivamente) y el Espectrómetro de Velocidad Radial (RVS, cubriendo 846–870 nm). La lista de fuentes permanece idéntica al Gaia EDR3.

El catálogo proporciona nuevas velocidades radiales medias para más de 33 millones de objetos, espectros medios BP/RP para alrededor de 220 millones de fuentes y espectros medios RVS para aproximadamente 1 millón de fuentes. El análisis de la fotometría de época produce clasificaciones y parámetros para alrededor de 10 millones de fuentes variables en 24 tipos. Se proporcionan parámetros astrofísicos para aproximadamente 470 millones de fuentes, con probabilidades de clase de objeto para alrededor de 1,5 mil millones de fuentes. Además, las soluciones orbitales o parámetros de tendencia están disponibles para aproximadamente 800.000 estrellas no-simples, y se incluyen datos para más de 150.000 objetos del Sistema Solar.

Las principales métricas de rendimiento y características del sondeo incluyen:

* **Período de Observación:** 34 meses
* **Marco de Referencia Astrométrica:** Gaia-CRF3 (alineado con ICRF3 a ~0,01 mas RMS en J2016.0)
* **Sesgo Global de Paralaje:** –17 µas
* **Resolución Espectral BP/RP (R = λ/Δλ):** ~30–100 (BP), ~70–100 (RP)
* **Resolución Espectral RVS (R = λ/Δλ):** ~11.500
* **Rango de Longitud de Onda RVS (procesado):** 846–870 nm
* **Límite de Magnitud de Velocidad Radial:** GRVS < 14
* **Rango de Temperatura de Velocidad Radial:** 3100 ≤ Teff ≤ 14.500 K
* **Límite de Magnitud de los Espectros Medios BP/RP:** Principalmente G < 17,65

<figure class="dataset-figure">
<img src="../../images/gaia/Gaia_DR3.webp" alt="Mapa de Densidad Angular del Gaia Data Release 3">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/gaia_dr3')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/gaia_dr3/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 1.812.731.847   | 152                | 2.016                | 1,1 TiB         |

<div class="button-container">
<a href="https://www.cosmos.esa.int/web/gaia/dr3" class="button-link">Lanzamiento Oficial</a>
<a href="https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html" class="button-link">Descripciones de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220800211G/abstract" class="button-link">Artículo de Investigación</a>
</div>
