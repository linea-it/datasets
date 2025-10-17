# Dark Energy Spectroscopic Instrument Data Release 1

El Dark Energy Spectroscopic Instrument (DESI) Data Release 1 (DR1) presenta datos espectroscópicos de los primeros 13 meses del sondeo principal de DESI (14 de mayo de 2021 hasta 13 de junio de 2022), junto con un reprocesamiento uniforme de todos los datos de Validación del Sondeo (SV). DESI es un espectrógrafo altamente multiplexado montado en el telescopio Mayall de 4 metros en el Observatorio Nacional de Kitt Peak, capaz de observar simultáneamente 5000 objetivos en un campo de visión de 8 deg² usando posicionamiento robótico de fibras.

DR1 comprende observaciones en 14.000 deg² de los hemisferios norte y sur galácticos en longitudes de onda ópticas (3600-9800 Å) abarcando cinco clases amplias de objetivos: estrellas del Milky Way Survey (MWS), galaxias del Bright Galaxy Survey (BGS, 0<z<0,6), galaxias rojas luminosas (LRGs, 0,4<z<1,1), galaxias de línea de emisión (ELGs, 0,6<z<1,6) y cuásares (QSOs, 0,9<z<4). La producción espectroscópica principal para DR1 es Iron, procesado usando algoritmos de calibración mejorados y plantillas de QSO actualizadas en comparación con el lanzamiento EDR anterior.

El catálogo resultante DR1 contiene corrimientos al rojo de alta confianza para 18,7 millones de objetos únicos en todos los sondeos y programas, haciendo de DR1 el mayor sondeo espectroscópico de corrimiento al rojo extragaláctico jamás realizado—casi cuatro veces más grande que todos los programas SDSS anteriores combinados. El sondeo principal incluye 8,5 millones, 9,0 millones y 1,2 millones de objetos de los programas bright, dark y backup, respectivamente. Después de aplicar criterios de calidad (ZWARN=0), la muestra comprende 13,1 millones de galaxias, 1,6 millones de cuásares y 4 millones de estrellas.

Las principales métricas de rendimiento y características del sondeo incluyen:

* **Cobertura Espectroscópica**: 9739 deg² (programa bright), 9528 deg² (programa dark), 2726 deg² (programa backup)
* **Completitud del Sondeo** (al final del período DR1): 41,3% (bright), 29,0% (dark), 5,2% (backup)
* **Precisión de Longitud de Onda**: 0,025 Å
* **Calibración Espectrofotométrica**: 6-10% de incertidumbre sistemática
* **Precisión de Corrimiento al Rojo**: 10 km s⁻¹ (BGS, ELG), 50 km s⁻¹ (LRG), 20-125 km s⁻¹ (QSO)
* **Tasa de Valores Atípicos de Corrimiento al Rojo**: ≤0,3% (BGS, LRG, ELG), 0,7% (QSO z<2,1), 1,8% (QSO z>2,1)
* **Precisión de Velocidad Radial** (MWS): ≲10 km s⁻¹
* **Residuos de Sustracción del Cielo**: <1% sistemático
* **Resolución Instrumental**: λ/Δλ = 2000-5200 (dependiente de la longitud de onda)

<figure class="dataset-figure">
<img src="../../images/desi/DESI_DR1_zcat.webp" alt="Mapa de Densidad Angular del Dark Energy Spectroscopic Instrument DR1 z-catalog">
<figcaption>Fuente de la imagen: https://data.lsdb.io</figcaption>
</figure>

## Cargar usando LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/desi/desi_dr1_zcat')
```

## Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/desi/desi_dr1_zcat/
```

## Metadatos del Catálogo

| Número de filas | Número de columnas | Número de particiones | Tamaño en disco |
|-----------------|-------------------|----------------------|-----------------|
| 28.425.963      | 136                | 75                   | 12 GiB          |

<div class="button-container">
<a href="https://data.desi.lbl.gov/doc/releases/dr1" class="button-link">Lanzamiento Oficial</a>
<a href="https://desidatamodel.readthedocs.io/en/latest/column_descriptions.html" class="button-link">Descripciones de Columnas</a>
<a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250314745D" class="button-link">Artículo de Investigación</a>
</div>

## Agradecimientos

La investigación utilizó datos de DESI. La construcción y operación de DESI son gestionadas por el Lawrence Berkeley National Laboratory. Trabajo apoyado por el Departamento de Energía de EE.UU., Oficina de Ciencia, Oficina de Física de Alta Energía (Contrato No. DE-AC02-05CH11231) y por el Centro Nacional de Computación Científica de Investigación en Energía.

Apoyo adicional de:

- Fundación Nacional de Ciencia de EE.UU. (NSF), División de Ciencias Astronómicas (Contrato No. AST-0950945)
- Laboratorio Nacional de Investigación en Astronomía Óptica-Infrarroja de la NSF
- Consejo de Instalaciones de Ciencia y Tecnología del Reino Unido
- Fundación Gordon y Betty Moore
- Fundación Heising-Simons
- Comisión Francesa de Energías Alternativas y Energía Atómica (CEA)
- Consejo Nacional de Humanidades, Ciencia y Tecnología de México (CONAHCYT)
- Ministerio de Ciencia e Innovación de España (MICINN)
- Instituciones Miembro de DESI (www.desi.lbl.gov/collaborating-institutions)

La colaboración DESI tiene permiso para conducir investigación científica en I'oligam Du'ag (Kitt Peak), una montaña significativa para la Nación Tohono O'odham.

Las opiniones, hallazgos y conclusiones son de los autores y no reflejan necesariamente las opiniones de la Fundación Nacional de Ciencia de EE.UU., Departamento de Energía de EE.UU. o agencias de financiamiento listadas.
