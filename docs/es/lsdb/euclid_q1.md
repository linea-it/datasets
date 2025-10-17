# Euclid Quick Data Release 1

La misión Euclid, una misión espacial de la ESA dirigida principalmente al estudio de materia oscura y energía oscura usando lente gravitacional débil y agrupamiento de galaxias, comenzó sus operaciones nominales de sondeo amplio en febrero de 2024. El primer Euclid Quick Data Release (Q1), puesto a disposición pública en marzo de 2025, proporciona una visión temprana de las capacidades del sondeo. Q1 comprende datos de imagen y espectroscopia espaciales visibles e infrarrojos cercanos del instrumento VIS y del Espectrómetro y Fotómetro Infrarrojo Cercano (NISP), suplementados por fotometría terrestre en las bandas u, g, r, i y z, procesados con versiones tempranas de los pipelines de Euclid.

Q1 abarca 63,1 grados cuadrados cubriendo tres Campos Profundos Euclid (EDF-N, EDF-S, EDF-F) observados hasta la profundidad nominal de visita única del Euclid Wide Survey (EWS). Los datos incluyen imágenes en las bandas VIS (IE) y NISP (YE, JE, HE), así como espectroscopia sin rendija de NISP usando el grism rojo (1,206–1,892 µm). Los datos terrestres se originan principalmente del sondeo UNIONS para EDF-N y del Dark Energy Survey (DES) y otras observaciones DECam para EDF-S y EDF-F. Q1 también incluye observaciones más profundas (aproximadamente 17 veces la exposición EWS) de un área de 0,5 grado cuadrado en la nube oscura LDN 1641.

El catálogo Q1 contiene aproximadamente 30 millones de objetos en las tres áreas EDF.

Las principales métricas de rendimiento y características del sondeo incluyen:

* **Resolución Espacial VIS:** 0,18"
* **Resolución Espacial NISP:** 0,3" por pixel
* **Profundidad Fotométrica (Terrestre, 10σ, apertura 2", típica para EDF-N):** g ≈ 25,3, r ≈ 24,3, i ≈ 23,7, z ≈ 23,6 mag
* **Marco de Calibración Astrométrica:** Gaia DR3
* **Marco de Calibración Fotométrica Absoluta:** HST CALSPEC
* **Dispersión Fotométrica Interna (Coadiciones terrestres vs sintética Gaia):** ~1% (NMAD)
* **Objetivos Espectroscópicos:** Fuentes con HE ≤ 22,5
* **Tasa de Éxito de Corrimiento al Rojo Espectroscópico:** Esperada por debajo del 10% para mediciones automatizadas en el procesamiento Q1

<figure class="dataset-figure">
<img src="../../images/euclid/Euclid_Q1.webp" alt="Mapa de Densidad Angular del Euclid Quick Data Release 1">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/euclid_q1')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/euclid_q1/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 29.767.806      | 472                | 85                   | 23 GiB          |

<div class="button-container">
<a href="https://www.cosmos.esa.int/en/web/euclid/euclid-q1-data-release" class="button-link">Lanzamiento Oficial</a>
<a href="https://euclid.esac.esa.int/dr/q1/dpdd/merdpd/dpcards/mer_finalcatalog.html#detailed-description-of-the-data-product" class="button-link">Descripciones de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250315302E/abstract" class="button-link">Artículo de Investigación</a>
</div>
