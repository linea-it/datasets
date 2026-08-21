# Datos del Photo-z Server

El Photo-z Server es una plataforma web desarrollada por LIneA como parte de la contribución in-kind de Brasil al proyecto Rubin Observatory LSST. Proporciona acceso tanto a productos de datos oficiales como a productos generados por usuarios. Los administradores del Photo-z Server mantienen y actualizan periódicamente una lista curada de recursos de datos para apoyar a la LSST Community con ejemplos de uso general.

Esta página ofrece una visión general de algunos conjuntos de datos disponibles en el Photo-z Server, junto con instrucciones de acceso. Para más detalles sobre las funcionalidades de la plataforma, consulte la [**Photo-z Server User Documentation**](https://docs.linea.org.br/es/sci-platforms/pz_server.html).

!!! info "Acceso restringido"
    De acuerdo con las políticas de datos del Rubin Observatory y de IDAC-BR, el acceso a los datos de LSST — incluidos los productos derivados alojados en el Photo-z Server — está restringido a miembros autorizados de la LSST Community con cuentas RSP válidas.

## Clasificación de conjuntos de datos

### Productos de datos oficiales

Los conjuntos de datos oficiales serán validados por Rubin's Data Management y estarán disponibles para la LSST Community a través del Photo-z Server. Estos conjuntos de datos incluirán catálogos de redshifts de referencia, conjuntos de entrenamiento y estimaciones photo-z asociadas con los data releases de LSST. Los conjuntos de datos se publicarán de forma escalonada, comenzando con el primer data release (DR1) y continuando con releases posteriores a medida que avance el relevamiento LSST. Por ahora, la página [Rubin Observatory PZ Data Products](https://pzserver.linea.org.br/oficial_products) está vacía.

### Productos de datos generados por usuarios

La mayoría de los productos de datos alojados en el Photo-z Server serán cargados o creados por usuarios, y no existe garantía de calidad para ellos. Se alienta a los usuarios a utilizar el Photo-z Server para almacenar productos de datos en cualquier etapa de desarrollo, desde muestras experimentales hasta resultados refinados asociados con publicaciones científicas.

Además de los datos cargados por usuarios, la página [User-generated Data Products](https://pzserver.linea.org.br/user_products) aloja un conjunto de datos preparado por los administradores del Photo-z Server con fines educativos, para servir como ejemplos de casos de uso en los tutoriales del Photo-z Server. Además, los productos de datos DP1 y DP2 generados por la PZ Science Unit del Rubin’s Commissioning Team, como los descritos en las tech notes [SITCOMTN-154](https://sitcomtn-154.lsst.io/) (para DP1) y [RTN-124](https://rtn-124.lsst.io) (en preparación, para DP2), también están disponibles allí. **Estos productos de datos fueron validados solo de forma muy ligera. Trátelos como provisionales y úselos con precaución.**

---

## Data Preview 2

La información detallada sobre los DR2 PZ Data Products estará disponible en la tech note [RTN-124](https://rtn-124.lsst.io) (en preparación).

!!! warning "Sección en construcción"
    Los enlaces y descripciones a continuación podrían cambiar pronto.

### Muestra de redshifts de referencia

Una compilación de redshifts de referencia producida usando el pipeline [**Combine Redshift Catalogs (CRC)**](https://docs.linea.org.br/es/sci-platforms/pz_server_crc.html), mediante la combinación de 38 catálogos con datos de 51 surveys, en su mayoría espectroscópicos, para hacer match con el catálogo LSST Object y producir conjuntos de entrenamiento y prueba para algoritmos photo-z.

| Producto de datos | Descripción | # de catálogos fuente | # de objetos | Estado |
| --- | --- | --- | --- | --- |
| [REF_Z_CLEAN_NO_DESI_LSS](https://pzserver.linea.org.br/product/318_ref_z_clean_no_desi_lss) | Objetos únicos con quality flag $\geq$ 3, excluyendo DESI DR1 | 37 |  6,616,173 | :material-check: |
| [DESI DR1 LITE](https://pzserver.linea.org.br/product/314_desi_dr1_lite) | DESI DR1 (selección de columnas) | 1 | 28,425,963 | :material-check: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

### Conjuntos de entrenamiento y prueba

| Producto de datos | Descripción | # de objetos | Estado |
| --- | --- | --- | --- |
| [MATCHED_CLEAN RTN-124](https://pzserver.linea.org.br/product/417_matched_clean_rtn124) | [REF_Z_CLEAN_NO_DESI_LSS](https://pzserver.linea.org.br/product/342_ref_z_clean_no_desi_lss) matched con DP2 Objects | 1,1940,88 | :material-check: |
| [MATCHED_DESI RTN-124](https://pzserver.linea.org.br/product/418_matched_desi_rtn124) | [DESI DR1 LITE](https://pzserver.linea.org.br/product/314_desi_dr1_lite) matched con DP2 Objects | 1,544,298 | :material-check: |
| [CLIPPED_TRAIN RTN-124 (PARQUET)](https://pzserver.linea.org.br/product/415_clipped_train_rtn124_parquet) | Muestra aleatoria del 80% de MATCHED_CLEAN recortada por exceso sesgado basado en bines de i_mag-redshift | 554,676 | :material-check: |
| [SOM_TEST RTN-124 (PARQUET)](https://pzserver.linea.org.br/product/412_som_test_rtn124_parquet) | 20% restante de MATCHED_CLEAN con muestreo basado en SOM para imitar "DP2 galaxies" | 18,400 | :material-check: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

### Resultados de entrenamiento

| Gold baseline | Gold 4 bands | Gold 6 bands |
| --- | --- | --- |
| [BPZ model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/419_bpz_model_dp2_gold_baseline_rtn124)   :material-check: | [BPZ model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/426_bpz_model_dp2_gold_4_bands_rtn124)  :material-check: | [BPZ model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/433_bpz_model_dp2_gold_6_bands_rtn124)  :material-check: |
| [DNF model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/420_dnf_model_dp2_gold_baseline_rtn124)  :material-check: | [DNF model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/427_dnf_model_dp2_gold_4_bands_rtn124)  :material-check: | [DNF model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/434_dnf_model_dp2_gold_6_bands_rtn124)   :material-check: |
| [FlexZBoost model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/421_flexzboost_model_dp2_gold_baseline_rtn124)   :material-check: | [FlexZBoost model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/428_flexzboost_model_dp2_gold_4_bands_rtn124) | [FlexZBoost model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/435_flexzboost_model_dp2_gold_6_bands_rtn124)  :material-check: |
| [GPz model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/422_gpz_model_dp2_gold_baseline_rtn124)  :material-check: | [GPz model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/429_gpz_model_dp2_gold_4_bands_rtn124)  :material-check: | [GPz model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/436_gpz_model_dp2_gold_6_bands_rtn124)  :material-check: |
| [kNN model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/423_knn_model_dp2_gold_baseline_rtn124)   :material-check: | [kNN model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/430_knn_model_dp2_gold_4_bands_rtn124)  :material-check: | [kNN model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/437_knn_model_dp2_gold_6_bands_rtn124)   :material-check: |
| [LePhare model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/424_lephare_model_dp2_gold_baseline_rtn124)  :material-check: | [LePhare model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/431_lephare_model_dp2_gold_4_bands_rtn124)  :material-check: | [LePhare model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/438_lephare_model_dp2_gold_6_bands_rtn124)  :material-check: |
| [TPZ model DP2 gold baseline RTN-124](https://pzserver.linea.org.br/product/425_tpz_model_dp2_gold_baseline_rtn124)   :material-check: | [TPZ model DP2 gold 4 bands RTN-124](https://pzserver.linea.org.br/product/432_tpz_model_dp2_gold_4_bands_rtn124)  :material-check: | [TPZ model DP2 gold 6 bands RTN-124](https://pzserver.linea.org.br/product/440_tpz_model_dp2_gold_6_bands_rtn124)   :material-check: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

### Resultados de validación

Se agregarán próximamente.

### Estimaciones Photo-z

Se agregarán próximamente.

Por ahora, se puede acceder a las Estimaciones Photo-z mediante LSDB. Para más información, visite la [página de LSDB.io](https://data.lsdb.io/Rubin/DP2/object_photoz)

---

## Data Preview 1

### Catálogos de objetos

Productos de datos que contienen tablas de objetos descritas en la Sección 2.1 y listadas en la Tabla 1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Producto de datos | Conjunto de datos | Selección | Número de objetos |
| --- | --- | --- | --- |
| DP1 (disponible en el RSP) | Complete DP1 Object Catalog | None | 2,299,757 |
| [ECDFS+EDFS+SV_95 gold SITCOMTN-154](https://pzserver.linea.org.br/product/78_ecdfsedfssv_95_gold_sitcomtn154) | ECDFS+EDFS+SV_95 | gold | 375,610 |
| [SV_38 gold_4_band SITCOMTN-154](https://pzserver.linea.org.br/product/79_sv_38_gold_4_band_sitcomtn154) | SV_38 | gold_4_band | 169,034 |

Conjunto de datos Gold completo para todos los campos de DP1 más allá de los campos ECDFS+EDFS+SV_95 y SV_38, donde hay datos espectroscópicos disponibles (conjunto de datos **no** listado en la Tabla 1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/)):

| Producto de datos | Conjunto de datos | Selección | Número de objetos |
| --- | --- | --- | --- |
| [DP1 Gold all](https://pzserver.linea.org.br/product/80_dp1_gold_all_sitcomtn154) | All fields | gold | 686,334 |

### Catálogos de redshifts de referencia

#### Catálogos de redshifts de referencia de surveys individuales

Productos de datos que contienen catálogos de redshifts de referencia (antes del matching con la tabla DP1 Object) separados por survey de origen, como se lista en la Tabla 2 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

**Nota:** Estos conjuntos de datos ya fueron filtrados al campo ECDFS y limpiados con los criterios de selección descritos en la Sección 2.2.1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Para los catálogos originales completos, consulte la sección [Conjuntos de datos externos](#conjuntos-de-datos-externos) a continuación.

| Producto de datos | Referencia | Número de redshifts |
| --- | --- | --- |
| [2dFGRS SITCOMTN-154](https://pzserver.linea.org.br/product/60_2dfgrs_sitcomtn154) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 278 |
| [2dflens SITCOMTN-154](https://pzserver.linea.org.br/product/61_2dflens_sitcomtn154) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 1 |
| [2MRS SITCOMTN-154](https://pzserver.linea.org.br/product/62_2mrs_sitcomtn154) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 9 |
| [3D-HST SITCOMTN-154](https://pzserver.linea.org.br/product/63_3dhst_sitcomtn154) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 4237 |
| [6dFGS SITCOMTN-154](https://pzserver.linea.org.br/product/64_6dfgs_sitcomtn154) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 5 |
| [astrodeep SITCOMTN-154](https://pzserver.linea.org.br/product/65_astrodeep_sitcomtn154) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M) | 35108 |
| [astrodeep_jwst SITCOMTN-154](https://pzserver.linea.org.br/product/66_astrodeep_jwst_sitcomtn154) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A&A...691A.240M) | 76748 |
| [CANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/67_candels_sitcomtn154) | [Kodra et al. (2023)](https://ui.adsabs.harvard.edu/abs/2023ApJ...942...36K) | 31440 |
| [JADES SITCOMTN-154](https://pzserver.linea.org.br/product/68_jades_sitcomtn154) | [D’Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D) | 1224 |
| [MOSDEF SITCOMTN-154](https://pzserver.linea.org.br/product/69_mosdef_sitcomtn154) | [Kriek et al. (2015)](https://ui.adsabs.harvard.edu/abs/2015ApJS..218...15K) | 51 |
| [NED SITCOMTN-154](https://pzserver.linea.org.br/product/70_ned_sitcomtn154) | [Helou et al. (1991)](https://ui.adsabs.harvard.edu/abs/1991ASSL..171...89H) | 3770 |
| [OzDES SITCOMTN-154](https://pzserver.linea.org.br/product/71_ozdes_sitcomtn154) | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L) | 1147 |
| [PRIMUS SITCOMTN-154](https://pzserver.linea.org.br/product/72_primus_sitcomtn154) | [Cool et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013ApJ...767..118C) | 7352 |
| [VANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/73_vandels_sitcomtn154) | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...647A.150G) | 450 |
| [VIMOS SITCOMTN-154](https://pzserver.linea.org.br/product/74_vimos_sitcomtn154) | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A&A...512A..12B) | 1578 |
| [VUDS SITCOMTN-154](https://pzserver.linea.org.br/product/75_vuds_sitcomtn154) | [Tasca et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017A&A...600A.110T) | 160 |
| [VVDS SITCOMTN-154](https://pzserver.linea.org.br/product/76_vvds_sitcomtn154) | [Le Fèvre et al. (2005)](https://ui.adsabs.harvard.edu/abs/2005A&A...439..845L) | 669 |

Se usaron datos espectroscópicos adicionales de DESI DR1 como conjunto de prueba independiente para validar las estimaciones photo-z. Como DESI DR1 es un conjunto de datos muy grande que se extiende más allá de la huella de DP1, fue filtrado para incluir solo el campo ECDFS.

| Producto de datos | Referencia | Número de redshifts |
| --- | --- | --- |
| [DESI DR1 inside DP1 footprint](https://pzserver.linea.org.br/product/34_desi_dr1_inside_dp1) | [DESI Collaboration et al. (2025)](https://arxiv.org/abs/2503.14745) | 50,634 |

#### Catálogo de redshifts combinado

Un único archivo que contiene todos los redshifts de referencia combinados de los surveys individuales listados arriba (excluyendo DESI), como se describe en la Sección 2.2.1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Producto de datos | Número de redshifts |
| --- | --- |
| [ComCam ECDFS z catalog SITCOMTN-154](https://pzserver.linea.org.br/product/77_comcam_ecdfs_z_catalog_sitcomtn154) | 104,070 |

### Conjuntos de entrenamiento y prueba

En el Photo-z Server, el tipo de producto "Training Set" comprende todas las muestras resultantes del matching entre un redshift de referencia y un catálogo de objetos. Esto puede incluir conjuntos de entrenamiento y prueba juntos en el mismo archivo, o submuestras independientes cargadas por separado. En este último caso, tanto los conjuntos de entrenamiento como los de prueba se etiquetan como "Training Set".

Los productos de datos que contienen conjuntos de entrenamiento y prueba generados a partir del ComCam ECDFS z catalog listado en la Tabla 1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/) son:

| Producto de datos | Conjunto de datos | Selección | Número de objetos |
| --- | --- | --- | --- |
| [training_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/81_training_v1_match_prelim_sitcomtn154) | training_v1 | match_prelim | 7,000 |
| [test_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/82_test_v1_match_prelim_sitcomtn154) | test_v1 | match_prelim | 2,437 |
| [training_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/83_training_v4_match_ecdfs_sitcomtn154) | training_v4 | match_ecdfs | 6,778 |
| [test_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/84_test_v4_match_ecdfs_sitcomtn154) | test_v4 | match_ecdfs | 2,905 |
| [test_DESI match_desi SITCOMTN-154](https://pzserver.linea.org.br/product/85_test_desi_match_desi_sitcomtn154) | test_DESI | match_desi | 2,728 |

### Resultados de entrenamiento

Los estimator data models están listados en la Tabla 7 y descritos en el Apéndice A.3 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Gold baseline | Gold DP1 optimize | Gold DP1 optimize 4band |
| --- | --- | --- |
| [BPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/90_bpz_model_gold_baseline_sitcomtn154) | [BPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/97_bpz_model_gold_dp1_optimize_sitcomtn154) | [BPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/105_bpz_model_gold_dp1_optimize_4band_sitcomtn154) |
| [CMNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/91_cmnn_model_gold_baseline_sitcomtn154) | [CMNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/98_cmnn_model_gold_dp1_optimize_sitcomtn154) | [CMNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/106_cmnn_model_gold_dp1_optimize_4band_sitcomtn154) |
| [DNF model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/92_dnf_model_gold_baseline_sitcomtn154) | [DNF model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/99_dnf_model_gold_dp1_optimize_sitcomtn154) | [DNF model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/107_dnf_model_gold_dp1_optimize_4band_sitcomtn154) |
| [FlexZBoost model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/93_flexzboost_model_gold_baseline_sitcomtn154) | [FlexZBoost model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/100_flexzboost_model_gold_dp1_optimize_sitcomtn154) | [FlexZBoost model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/108_flexzboost_model_gold_dp1_optimize_4band_sitcomtn154) |
| [GPz model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/94_gpz_model_gold_baseline_sitcomtn154) | [GPz model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/101_gpz_model_gold_dp1_optimize_sitcomtn154) | [GPz model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/109_gpz_model_gold_dp1_optimize_4band_sitcomtn154) |
| [kNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/95_knn_model_gold_baseline_sitcomtn154) | [kNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/102_knn_model_gold_dp1_optimize_sitcomtn154) | [kNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/110_knn_model_gold_dp1_optimize_4band_sitcomtn154) |
| N/A | [LePhare model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/103_lephare_model_gold_dp1_optimize_sitcomtn154) | [LePhare model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/111_lephare_model_gold_dp1_optimize_4band_sitcomtn154) |
| [TPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/96_tpz_model_gold_baseline_sitcomtn154) | [TPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/104_tpz_model_gold_dp1_optimize_sitcomtn154) | [TPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/112_tpz_model_gold_dp1_optimize_4band_sitcomtn154) |

<font size=4> Configuration Files </font><br>

Como se menciona en la Sección 3.4 y en el Apéndice A.1 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/), los archivos de configuración [dp1.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1.yaml) (el conjunto completo de configuraciones probadas, etiquetadas como analysis _flavors_) y [dp1_v4.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1_v4.yaml) (parámetros de configuración optimizados) están disponibles en el repositorio de GitHub [`rail_project_config`](https://github.com/LSSTDESC/rail_project_config).

### Resultados de validación

Las estimaciones puntuales photo-z, QP Ensembles y métricas de evaluación están relacionadas con los resultados mostrados en la Tabla 4. Los archivos fueron cargados desde directorios listados en la Tabla 7 y descritos en el Apéndice A.4 de la tech note [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Gold baseline | Gold DP1 optimize |
| --- | --- |
| [BPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/113_bpz_test_gold_baseline_sitcomtn154) | [BPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/120_bpz_test_gold_dp1_optimize_sitcomtn154) |
| [CMNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/114_cmnn_test_gold_baseline_sitcomtn154) | [CMNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/121_cmnn_test_gold_dp1_optimize_sitcomtn154) |
| [DNF test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/115_dnf_test_gold_baseline_sitcomtn154) | [DNF test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/122_dnf_test_gold_dp1_optimize_sitcomtn154) |
| [FlexZBoost test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/116_flexzboost_test_gold_baseline_sitcomtn154) | [FlexZBoost test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/123_flexzboost_test_gold_dp1_optimize_sitcomtn154) |
| [GPz test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/117_gpz_test_gold_baseline_sitcomtn154) | [GPz test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/124_gpz_test_gold_dp1_optimize_sitcomtn154) |
| [kNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/118_knn_test_gold_baseline_sitcomtn154) | [kNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/125_knn_test_gold_dp1_optimize_sitcomtn154) |
| N/A | [LePhare test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/126_lephare_test_gold_dp1_optimize_sitcomtn154) |
| [TPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/119_tpz_test_gold_baseline_sitcomtn154) | [TPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/127_tpz_test_gold_dp1_optimize_sitcomtn154) |

### Estimaciones Photo-z

#### Photo-z Tables

Las PZ Tables fueron producidas como parte de los estudios iniciales con datos de commissioning descritos en [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Los datos fueron cargados desde los directorios listados en la Tabla 7.

| Producto de datos | Número de objetos |
| --- | --- |
| [PZ Table dp1_all gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/128_pz_table_dp1_all_gold_baseline_sitcomtn154) | 686,334 |
| [PZ Table dp1_sv38 gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/129_pz_table_dp1_sv38_gold_baseline_sitcomtn154) | 169,034 |
| [PZ Table DESI gold baseline](https://pzserver.linea.org.br/product/130_pz_table_desi_gold_baseline_sitcomtn154) | 2728 |

---

## Conjuntos de datos externos

Datos públicos recopilados de la literatura y alojados en el Photo-z Server.

### Catálogos de redshifts de referencia

#### Surveys individuales

El Photo-z Server aloja varios catálogos públicos de redshifts espectroscópicos de diferentes surveys que pueden utilizarse como conjuntos de datos de referencia para el entrenamiento y la validación de estimaciones photo-z. Los productos de datos listados abajo son los catálogos originales, sin ningún filtrado ni selección de datos.

| Producto de datos | Referencia | Número de redshifts | Estado |
| --- | --- | --- | --- |
| [2dFGRS Final Data Release](https://pzserver.linea.org.br/product/170_2dfgrs_final_data_release) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 245,591 | :material-check: |
| [2dFLenS Final Data Release](https://pzserver.linea.org.br/product/171_2dflens_final_data_release) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 70,079 | :material-check: |
| [2MRS v240](https://pzserver.linea.org.br/product/172_2mrs_v240) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 240,496 | :material-check: |
| [3D-HST v415](https://pzserver.linea.org.br/product/173_3dhst_v415) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 207,967 | :material-check: |
| [6dFGS DR3](https://pzserver.linea.org.br/product/174_6dfgs_dr3) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 136,304 | :material-check: |
| ACES | - | - | :material-clock-outline: |
| AMA DR4 | - | - | :material-clock-outline: |
| [ASTRODEEP GS43](https://pzserver.linea.org.br/product/176_astrodeep_gs43) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M/abstract) | 35,108 | :material-check: |
| [ASTRODEEP JWST](https://pzserver.linea.org.br/product/177_astrodeep_jwst) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A%26A...691A.240M/abstract) | 531,173 | :material-check: |
| ATLAS DR2 | - | - | :material-clock-outline: |
| C3R2 DR2 | - | - | :material-clock-outline: |
| [C3R2 DR3](https://pzserver.linea.org.br/product/303_c3r2_dr3) | [Stanford et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021ApJS..256....9S/abstract) | 676 | :material-check: |
| CANUCS SMACS | - | - | :material-clock-outline: |
| CDB | - | - | :material-clock-outline: |
| CLASH-VLT FR | - | - | :material-clock-outline: |
| [COSMOS Specz Compilation DR1](https://pzserver.linea.org.br/product/212_cosmos_specz_compilation_dr1) | [Khostovan et al. (2025)](https://ui.adsabs.harvard.edu/abs/2026ApJS..282....6K/abstract) | 482,579 | :material-check: |
| [COSMOS Web DR1 - LEPHARE Extension](https://pzserver.linea.org.br/product/220_cosmos_web_dr1__lephare_extension) | [Shuntov et al. (2025)](https://www.aanda.org/articles/aa/abs/2025/12/aa55799-25/aa55799-25.html) | 784,016 | :material-check: |
| [COSMOS2020 CLASSIC LITE](https://pzserver.linea.org.br/product/269_cosmos2020_classic_lite) | [Weaver et al. (2022)](https://ui.adsabs.harvard.edu/abs/2022ApJS..258...11W/abstract) | 1,720,700 | :material-check: |
| DEEP2 DR4 | - | - | :material-clock-outline: |
| [DEIMOS 10K](https://pzserver.linea.org.br/product/215_deimos_10k) | [Hasinger et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018ApJ...858...77H/abstract) | 10,770 | :material-check: |
| DES IMACS | - | - | :material-clock-outline: |
| [DESI DEEP PILOT](https://pzserver.linea.org.br/product/265_desi_deep_pilot) | [Dey et al. (2026)](https://arxiv.org/pdf/2604.06143) | 7,546 | :material-check: |
| DESI DR1 | - | - | :material-clock-outline: |
| [DESI DR1 LITE](https://pzserver.linea.org.br/product/314_desi_dr1_lite) | [DESI Collaboration et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025arXiv250314745D/abstract) | 28,425,963 | :material-check: |
| DESI DR2 | - | - | :material-clock-outline: |
| [ELAISFBMC](https://pzserver.linea.org.br/product/233_elaisfbmc) | [Rowan-Robinson et al. (2004)](https://ui.adsabs.harvard.edu/abs/2004MNRAS.351.1290R/abstract) | 3,762 | :material-check: |
| [ELAISS1OID](https://pzserver.linea.org.br/product/232_elaiss1oid) | [Feruglio et al. (2008)](https://ui.adsabs.harvard.edu/abs/2008A%26A...488..417F/abstract) | 478 | :material-check: |
| [ELG_FIGS](https://pzserver.linea.org.br/product/301_elg_figs) | [Pharo et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020ApJ...888...79P/abstract) | 201 | :material-check: |
| [EUCLID Q1 GALAXY BEST RANK](https://pzserver.linea.org.br/product/300_euclid_q1_galaxy_best_rank) | [Euclid Collaboration (2025)](https://ui.adsabs.harvard.edu/abs/2025arXiv250315302E/abstract) | 3,716,438 | :material-check: |
| [FMOS-COSMOS](https://pzserver.linea.org.br/product/219_fmoscosmos) | [Kashino et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019ApJS..241...10K/abstract) | 5,484 | :material-check: |
| GAMA DR3 | - | - | :material-clock-outline: |
| [GAMA DR4](https://pzserver.linea.org.br/product/249_gama_dr4) | [Driver et al. (2022)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.513..439D/abstract) | 522,558 | :material-check: |
| GLASS DR2 | - | - | :material-clock-outline: |
| HectoMAP DR2 | - | - | :material-clock-outline: |
| [HELP DR1 - DMU23 - ELAIS-S1](https://pzserver.linea.org.br/product/234_help_dr1_dmu23_elaiss1) | [Shirley et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021MNRAS.507..129S/abstract) | 18,422 | :material-check: |
| HETDEX DR1 | - | - | :material-clock-outline: |
| [JADES DR3](https://pzserver.linea.org.br/product/179_jades_dr3) | [D'Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D/abstract) | 8,172 | :material-check: |
| [JADES DR4](https://pzserver.linea.org.br/product/253_jades_dr4) | [Curtis-Lake et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025arXiv251001033C/abstract) | 5,190 | :material-check: |
| [JADES DR5 PHOTOZ](https://pzserver.linea.org.br/product/262_jades_dr5_photoz) | [Robertson et al. (2026)](https://ui.adsabs.harvard.edu/abs/2026arXiv260115956R/abstract) | 304,366 | :material-check: |
| [JADES DR5 PHOTOZ_KRON](https://pzserver.linea.org.br/product/263_jades_dr5_photoz_kron) | [Robertson et al. (2026)](https://ui.adsabs.harvard.edu/abs/2026arXiv260115956R/abstract) | 304,366 | :material-check: |
| LCRS | - | - | :material-clock-outline: |
| LEGA-C DR3 | - | - | :material-clock-outline: |
| [MOSDEF Final Data Release](https://pzserver.linea.org.br/product/181_mosdef_final_data_release) | [Kriek et al. (2015)](https://ui.adsabs.harvard.edu/abs/2015ApJS..218...15K/abstract) | 1,791 | :material-check: |
| MOSFIRE | - | - | :material-clock-outline: |
| MUSE DR1 | - | - | :material-clock-outline: |
| N17B331 (LADUMA) | - | - | :material-clock-outline: |
| NOAO_OZDES | - | - | :material-clock-outline: |
| [OzDES DR2](https://pzserver.linea.org.br/product/182_ozdes_dr2) | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L/abstract) | 38,624 | :material-check: |
| PANSTARRS | - | - | :material-clock-outline: |
| [PRIMUS DR1](https://pzserver.linea.org.br/product/183_primus_dr1) | [Coil et al. (2011)](https://ui.adsabs.harvard.edu/abs/2011ApJ...741....8C/abstract) | 213,696 | :material-check: |
| SAGA DR2 | - | - | :material-clock-outline: |
| SDSS DR16 | - | - | :material-clock-outline: |
| [SDSS DR17 LITE](https://pzserver.linea.org.br/product/267_sdss_dr17_lite) | [Abdurro'uf et al. (2022)](https://ui.adsabs.harvard.edu/abs/2022ApJS..259...35A/abstract) | 5,801,200 | :material-check: |
| [SDSS DR19 LITE](https://pzserver.linea.org.br/product/299_sdss_dr19_lite) | [Kollmeier et al. (2025)](https://arxiv.org/abs/2507.06989) | 2,183,284 | :material-check: |
| SNLS_AAO | - | - | :material-clock-outline: |
| SNLS_FORS | - | - | :material-clock-outline: |
| SNVETO | - | - | :material-clock-outline: |
| SpARCS | - | - | :material-clock-outline: |
| SPT-GMOS | - | - | :material-clock-outline: |
| [SWIRE REVISED PHOTO-Z](https://pzserver.linea.org.br/product/245_swire_revised_photoz) | [Rowan-Robinson et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013MNRAS.428.1958R/abstract) | 1,152,665 | :material-check: |
| UDS | - | - | :material-clock-outline: |
| [VANDELS DR4](https://pzserver.linea.org.br/product/185_vandels_dr4) | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A%26A...647A.150G/abstract) | 2,165 | :material-check: |
| [VIPERS PDR-2](https://pzserver.linea.org.br/product/248_vipers_pdr2) | [Scodeggio et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018A%26A...609A..84S/abstract) | 91,507 | :material-check: |
| [VLT VIMOS V2.0.1](https://pzserver.linea.org.br/product/186_vlt_vimos_v201) | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A%26A...512A..12B/abstract) | 5,052 | :material-check: |
| [VUDS DR1](https://pzserver.linea.org.br/product/187_vuds_dr1) | [Tasca et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017A%26A...600A.110T/abstract) | 698 | :material-check: |
| [VVDS Final Data Release](https://pzserver.linea.org.br/product/188_vvds_final_data_release) | [Le Fèvre et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013A%26A...559A..14L/abstract) | 40,944 | :material-check: |
| WiggleZ | - | - | :material-clock-outline: |
| [XMM-LSS](https://pzserver.linea.org.br/product/251_xmmlss) | [Stalin et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010MNRAS.401..294S/abstract) | 487 | :material-check: |
| XXL_AAOMEGA | - | - | :material-clock-outline: |
| zCOSMOS DEEP | - | - | :material-clock-outline: |
| [zCOSMOS Final Release](https://pzserver.linea.org.br/product/218_zcosmos_final_release) | [Lilly et al. (2016)](https://www.eso.org/rm/api/v1/public/releaseDescriptions/66) | 20,689 | :material-check: |
| ZFIRE | - | - | :material-clock-outline: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

### Combined Redshift Catalogs (CRC)

Generado por el pipeline **[Combine Redshift Catalogs (CRC)](https://docs.linea.org.br/es/sci-platforms/pz_server_crc.html)** del **[Photo-z Server](https://docs.linea.org.br/es/sci-platforms/pz_server.html)**.

| Producto de datos | Fecha de publicación (MM/DD/YYYY) | # de productos | # de objetos | Estado |
| --- | --- | --- | --- | --- |
| [REF_Z_COMPLETE](https://pzserver.linea.org.br/product/339_ref_z_complete) | 07/06/2026 | 38 | 43,555,318 | :material-check: |
| [REF_Z_CLEAN](https://pzserver.linea.org.br/product/341_ref_z_clean) | 07/06/2026 | 38 | 20,856,682 | :material-check: |
| [REF_Z_CLEAN_NO_DESI_LSS](https://pzserver.linea.org.br/product/342_ref_z_clean_no_desi_lss) | 07/06/2026 | 37 | 6,668,608 | :material-check: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

### Training Set Maker (TSM)

Generado por el pipeline **[Training Set Maker (TSM)](https://docs.linea.org.br/es/sci-platforms/pz_server_tsm.html)** del **[Photo-z Server](https://docs.linea.org.br/es/sci-platforms/pz_server.html)**.

| Producto de datos | Fecha de publicación (MM/DD/YYYY) | # de objetos | Estado |
| --- | --- | --- | --- |
| [DP1_TRAIN_CMODEL](https://pzserver.linea.org.br/product/343_dp1_train_cmodel) | 07/07/2026 | 38,843 | :material-check: |

**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible

<!--
Acceso rápido mediante la biblioteca Python `pzserver`:

```python
pz_server.get_product('<dataset_name>')
```

-->
