# El Sondeo DELVE – Data Release 2

El Sondeo DECam de Exploración del Volumen Local – Data Release 2 (DELVE DR2) combina nuevas observaciones obtenidas con la DECam con datos de archivo procedentes del Sondeo de Energía Oscura (DES), del Sondeo Legacy DECam (DECaLS) y de otros programas comunitarios de la DECam.
Su principal objetivo científico es descubrir y caracterizar galaxias satélite de baja luminosidad y otros sistemas estelares resueltos individualmente en el Volumen Local.
El DELVE DR2 cubre más de cuatro veces el área y contiene aproximadamente cinco veces más objetos astronómicos en comparación con la liberación de datos anterior.

---

## Cobertura del Sondeo y Catálogo

El sondeo reunió aproximadamente 160,000 exposiciones (161,380 en total) de más de 270 programas comunitarios DECam. Cubre más de 21,000 grados cuadrados de cielo, con enfoque en regiones de alta latitud galáctica (latitud galáctica absoluta mayor de 10°).
Se emplearon cuatro filtros ópticos de banda ancha e infrarrojo cercano: *g, r, i* y *z*.

La superposición de las cuatro bandas cubre aproximadamente 17,000 grados cuadrados (16,972 deg²) y proporciona fotometría completa en cuatro bandas para unas 618 millones de fuentes.
El catálogo total contiene alrededor de 2.5 mil millones de fuentes, con mediciones fotométricas por PSF y por apertura (AUTO).

---

## Métricas Principales de Rendimiento

**Calidad de imagen:**
La anchura total a media altura (FWHM) de la función de dispersión puntual (PSF) mediana varía por banda:
g = 1.24 arcsec, r = 1.10 arcsec, i = 1.02 arcsec, z = 1.00 arcsec.

**Sensibilidad (fotometría PSF, S/N = 5):**
Profundidad mediana de fuente puntual: g = 24.3 mag, r = 23.9 mag, i = 23.5 mag, z = 22.8 mag.

**Sensibilidad (fotometría AUTO, S/N = 5):**
Profundidad mediana por apertura: g = 23.9 mag, r = 23.5 mag, i = 23.0 mag, z = 22.4 mag.

**Precisión astrométrica:**
El desplazamiento angular mediano en relación con Gaia EDR3 es de 22 milisegundos de arco (mas).

**Repetibilidad fotométrica:**
La desviación cuadrática media (rms) mediana es de 4.9 mmag (banda g), 5.0 mmag (banda r), 4.5 mmag (banda i) y 5.4 mmag (banda z).

**Incertidumbre fotométrica absoluta:**
La precisión fotométrica absoluta estimada es de 20 mmag o mejor en todas las bandas.

<figure class="dataset-figure">
<img src="../../images/delve/DELVE_DR2.webp" alt="Catálogo de Fuentes Puntuales DELVE DR2">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

---

## Cargar usando LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/delve_dr2')
```

---

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/delve_dr2/
```

---

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
| --------------- | ------------------ | --------------------- | --------------- |
| 2,500,247,752   | 120                | 5,513                 | 836 GiB         |

<div class="button-container">
<a href="https://datalab.noirlab.edu/data/delve" class="button-link">Liberación Oficial</a>
<a href="https://datalab.noirlab.edu/data/delve" class="button-link">Descripciones de Columnas</a>
<a href="https://arxiv.org/abs/2203.16565" class="button-link">Artículo de Investigación</a>
</div>
