# Datos del Photo-z Server

!!! Warning "Aviso"
    Página en construcción. Algunos contenidos pueden estar incompletos.

El Photo-z Server (Servidor de Photo-z) es una plataforma web desarrollada por LIneA como parte de la contribución in-kind de Brasil al proyecto LSST del Observatorio Rubin.

Los administradores del Photo-z Server mantienen y actualizan periódicamente una lista curada de recursos de datos para apoyar a la Comunidad LSST con productos de datos relacionados con photo-z. Esta página proporciona una descripción general de algunos conjuntos de datos disponibles en el Photo-z Server junto con instrucciones de acceso. Para más detalles sobre las características y funcionalidades de la plataforma, consulte la [**Documentación Completa del Photo-z Server para Usuarios**](https://docs.linea.org.br/es/sci-platforms/pz_server.html).


!!! info "Acceso Restringido"
    De acuerdo con las Políticas de Datos del Observatorio Rubin e IDAC-BR, el acceso a los datos LSST — incluyendo productos derivados alojados en el Photo-z Server — está restringido a miembros autorizados de la Comunidad LSST con cuentas RSP válidas.


## Clasificación de Conjuntos de Datos   

<font size=4> Conjuntos de Datos Oficiales </font><br>

Los conjuntos de datos oficiales serán producidos por el equipo de Gestión de Datos de Rubin y estarán disponibles para la Comunidad LSST a través del Photo-z Server. Estos conjuntos de datos incluirán catálogos de redshifts de referencia, conjuntos de entrenamiento y estimaciones de photo-z asociadas a las publicaciones de datos de LSST. Los conjuntos de datos se publicarán de manera escalonada, comenzando con la primera publicación de datos (DR1) y continuando con publicaciones posteriores a medida que avance el estudio LSST.

Por ahora, la página de [Productos de Datos Oficiales del Observatorio Rubin](https://pzserver.linea.org.br/oficial_products) está vacía.

<font size=4> Conjuntos de Datos No Oficiales </font><br>

Además de los datos cargados por usuarios, la página de [Productos de Datos Generados por Usuarios](https://pzserver.linea.org.br/user_products) aloja conjuntos de datos que fueron preparados por el equipo de LIneA con fines educativos, para servir como ejemplos de casos de uso para los tutoriales del Photo-z Server. Además, los conjuntos de datos DP1 generados por la Unidad de Ciencia de PZ del Equipo de Comisionamiento de Rubin, descritos en la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/), también están disponibles allí. Todos estos conjuntos de datos no están clasificados como Conjuntos de Datos Oficiales.

--- 


## Data Preview 1 


!!! warning "ATENCIÓN: Conjuntos de Datos Preliminares"  
    Estos conjuntos de datos fueron producidos por la Unidad de Ciencia de PZ — un grupo de trabajo del Equipo de Comisionamiento de Rubin — durante los _Estudios iniciales de corrimientos al rojo fotométricos con LSSTComCam a partir de DP1_. Todos los resultados, junto con descripciones detalladas de los conjuntos de datos, están disponibles en la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

    **Estos conjuntos de datos NO están clasificados como Conjuntos de Datos Oficiales publicados por el equipo de DM de Rubin.**  



Los conjuntos de datos descritos en la nota técnica están disponibles en el [Photo-z Server](https://pzserver.linea.org.br) como productos de datos con el sufijo `SITCOMTN-154`. Sus enlaces y breves descripciones están organizados por tipos de productos a continuación.


### Catálogos de Objetos 


Productos de datos que contienen tablas de objetos descritas en la Sección 2.1 y listadas en la Tabla 1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).


| Producto de Datos                | Conjunto de Datos        | Selección    | Número de Objetos | 
|----------------------------------|--------------------------|--------------|-------------------|
| DP1 (disponible en el RSP)       | Catálogo de Objetos Completo DP1| Ninguna | 2.299.757 |  
|[ECDFS+EDFS+SV_95 gold SITCOMTN-154](https://pzserver.linea.org.br/product/78_ecdfsedfssv_95_gold_sitcomtn154) | ECDFS+EDFS+SV_95|gold|375.610|  
|[SV_38 gold_4_band SITCOMTN-154](https://pzserver.linea.org.br/product/79_sv_38_gold_4_band_sitcomtn154)| SV_38|gold_4_band|169.034| 

 
Conjunto de datos Gold completo de todos los campos DP1 más allá de los campos ECDFS+EDFS+SV_95 y SV_38, donde hay datos espectroscópicos disponibles (conjunto de datos **no** listado en la Tabla 1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/)):   


| Producto de Datos                | Conjunto de Datos        | Selección   | Número de Objetos | 
|----------------------------------|--------------------------|-------------|-------------------|
|[DP1 Gold all](https://pzserver.linea.org.br/product/80_dp1_gold_all_sitcomtn154)| Todos los campos | gold | 686.334|
   




### Catálogos de Redshifts de Referencia 

#### Catálogos de Redshifts de Referencia de Estudios Individuales 

Productos de datos que contienen catálogos de corrimientos al rojo de referencia (antes del cruce con la tabla de Objetos DP1) separados por el estudio de origen, según se lista en la Tabla 2 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

**Nota:** Estos conjuntos de datos ya han sido filtrados al campo ECDFS y limpiados con los criterios de selección descritos en la Sección 2.2.1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Para los catálogos originales completos, consulte la sección [Conjuntos de Datos Externos](#conjuntos-de-datos-externos) a continuación.

| Producto de Datos | Referencia | Número de Corrimientos al Rojo |
|-------------------|-----------|--------------------------------|
| [2dFGRS SITCOMTN-154](https://pzserver.linea.org.br/product/60_2dfgrs_sitcomtn154) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 278 |
| [2dflens SITCOMTN-154](https://pzserver.linea.org.br/product/61_2dflens_sitcomtn154) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 1 |
| [2MRS SITCOMTN-154](https://pzserver.linea.org.br/product/62_2mrs_sitcomtn154) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 9 |
| [3D-HST SITCOMTN-154](https://pzserver.linea.org.br/product/63_3dhst_sitcomtn154) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 4237 |
| [6dFGS SITCOMTN-154](https://pzserver.linea.org.br/product/64_6dfgs_sitcomtn154) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 5 |
| [astrodeep SITCOMTN-154](https://pzserver.linea.org.br/product/65_astrodeep_sitcomtn154) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M) | 35108 |
| [astrodeep_jwst SITCOMTN-154](https://pzserver.linea.org.br/product/66_astrodeep_jwst_sitcomtn154) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A&A...691A.240M) | 76748 |
| [CANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/67_candels_sitcomtn154) | [Kodra et al. (2023)](https://ui.adsabs.harvard.edu/abs/2023ApJ...942...36K) | 31440 |
| [JADES SITCOMTN-154](https://pzserver.linea.org.br/product/68_jades_sitcomtn154) | [D'Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D) | 1224 |
| [MOSDEF SITCOMTN-154](https://pzserver.linea.org.br/product/69_mosdef_sitcomtn154) | [Kriek et al. (2015)](https://ui.adsabs.harvard.edu/abs/2015ApJS..218...15K) | 51 |
| [NED SITCOMTN-154](https://pzserver.linea.org.br/product/70_ned_sitcomtn154) | [Helou et al. (1991)](https://ui.adsabs.harvard.edu/abs/1991ASSL..171...89H) | 3770 |
| [OzDES SITCOMTN-154](https://pzserver.linea.org.br/product/71_ozdes_sitcomtn154) | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L) | 1147 |
| [PRIMUS SITCOMTN-154](https://pzserver.linea.org.br/product/72_primus_sitcomtn154) | [Cool et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013ApJ...767..118C) | 7352 |
| [VANDELS SITCOMTN-154](https://pzserver.linea.org.br/product/73_vandels_sitcomtn154) | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...647A.150G) | 450 |
| [VIMOS SITCOMTN-154](https://pzserver.linea.org.br/product/74_vimos_sitcomtn154) | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A&A...512A..12B) | 1578 |
| [VUDS SITCOMTN-154](https://pzserver.linea.org.br/product/75_vuds_sitcomtn154) | [Tasca et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017A&A...600A.110T) | 160 |
| [VVDS SITCOMTN-154](https://pzserver.linea.org.br/product/76_vvds_sitcomtn154) | [Le Fèvre et al. (2005)](https://ui.adsabs.harvard.edu/abs/2005A&A...439..845L) | 669 |



Datos espectroscópicos adicionales del DESI DR1 fueron utilizados como un conjunto de prueba independiente para validación de las estimaciones de photo-z. Como el DESI DR1 es un conjunto de datos muy grande que se extiende más allá del área de cobertura de DP1, fue filtrado para incluir solo el campo ECDFS.


| Producto de Datos | Referencia       | Número de Corrimientos al Rojo | 
|-------------------|------------------|--------------------------------|
| [DESI DR1 inside DP1](https://pzserver.linea.org.br/product/34_desi_dr1_inside_dp1)| [DESI Collaboration et al. (2025)](https://arxiv.org/abs/2503.14745) |50.634 |



#### Catálogo de Redshifts Combinado

Un único archivo que contiene todos los corrimientos al rojo de referencia combinados de los estudios individuales listados arriba (excluyendo DESI), según se describe en la Sección 2.2.1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).

| Producto de Datos | Número de Corrimientos al Rojo |
|-------------------|---------------------------------|
| [ComCam ECDFS z catalog SITCOMTN-154](https://pzserver.linea.org.br/product/77_comcam_ecdfs_z_catalog_sitcomtn154) |104.070| 









### Conjuntos de Entrenamiento y Prueba 

En el Photo-z Server, el tipo de producto "Training Set" abarca todas las muestras resultantes del cruce entre una amostra de redshifts de referencia y un catálogo de objetos. Esto puede incluir conjuntos de entrenamiento y prueba juntos en un mismo archivo o submuestras independientes cargadas por separado. Para este último caso, tanto los conjuntos de entrenamiento como los de prueba están etiquetados como "Training Set".


Productos de datos que contienen conjuntos de entrenamiento y prueba generados a partir del catálogo ComCam ECDFS z listados en la Tabla 1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/) son:


| Producto de Datos                | Conjunto de Datos        | Selección    | Número de Objetos | 
|----------------------------------|--------------------------|--------------|-------------------|
| [training_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/81_training_v1_match_prelim_sitcomtn154) | training_v1 | match_prelim | 7.000 |
| [test_v1 match_prelim SITCOMTN-154](https://pzserver.linea.org.br/product/82_test_v1_match_prelim_sitcomtn154)         | test_v1     | match_prelim | 2.437 | 
| [training_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/83_training_v4_match_ecdfs_sitcomtn154)  | training_v4 | match_ecdfs  | 6.778 |
| [test_v4 match_ecdfs SITCOMTN-154](https://pzserver.linea.org.br/product/84_test_v4_match_ecdfs_sitcomtn154)          | test_v4     | match_ecdfs  | 2.905 |      
| [test_DESI match_desi SITCOMTN-154](https://pzserver.linea.org.br/product/85_test_desi_match_desi_sitcomtn154)        | test_DESI   | match_desi   | 2.728 |    



### Resultados de Entrenamiento 

Modelos de datos de estimadores listados en la Tabla 7 y descritos en el Apéndice A.3 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).


| Gold baseline | Gold DP1 optimize | Gold DP1 optimize 4band |  
|---------------|-------------------|--------------------------| 
| [BPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/90_bpz_model_gold_baseline_sitcomtn154)        | [BPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/97_bpz_model_gold_dp1_optimize_sitcomtn154)        | [BPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/105_bpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [CMNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/91_cmnn_model_gold_baseline_sitcomtn154)      | [CMNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/98_cmnn_model_gold_dp1_optimize_sitcomtn154)      | [CMNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/106_cmnn_model_gold_dp1_optimize_4band_sitcomtn154)      | 
| [DNF model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/92_dnf_model_gold_baseline_sitcomtn154)        | [DNF model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/99_dnf_model_gold_dp1_optimize_sitcomtn154)        | [DNF model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/107_dnf_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [FlexZBoost model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/93_flexzboost_model_gold_baseline_sitcomtn154) | [FlexZBoost model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/100_flexzboost_model_gold_dp1_optimize_sitcomtn154) | [FlexZBoost model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/108_flexzboost_model_gold_dp1_optimize_4band_sitcomtn154) | 
| [GPz model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/94_gpz_model_gold_baseline_sitcomtn154)        | [GPz model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/101_gpz_model_gold_dp1_optimize_sitcomtn154)        | [GPz model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/109_gpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| [kNN model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/95_knn_model_gold_baseline_sitcomtn154)        | [kNN model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/102_knn_model_gold_dp1_optimize_sitcomtn154)        | [kNN model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/110_knn_model_gold_dp1_optimize_4band_sitcomtn154)        | 
| N/A                                              | [LePhare model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/103_lephare_model_gold_dp1_optimize_sitcomtn154) | [LePhare model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/111_lephare_model_gold_dp1_optimize_4band_sitcomtn154) | 
| [TPZ model gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/96_tpz_model_gold_baseline_sitcomtn154)        | [TPZ model gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/104_tpz_model_gold_dp1_optimize_sitcomtn154)        | [TPZ model gold DP1 optimize 4band SITCOMTN-154](https://pzserver.linea.org.br/product/112_tpz_model_gold_dp1_optimize_4band_sitcomtn154)        | 



<font size=4> Archivos de Configuración </font><br>
 
Como se menciona en la Sección 3.4 y Apéndice A.1 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/), los archivos de configuración [dp1.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1.yaml) (conjunto completo de configuraciones probadas, etiquetadas como _flavors_ de análisis) y [dp1_v4.yaml](https://github.com/LSSTDESC/rail_project_config/blob/main/dp1/dp1_v4.yaml) (parámetros de configuración optimizados) están disponibles en el repositorio GitHub [`rail_project_config`](https://github.com/LSSTDESC/rail_project_config).
 

### Resultados de Validación 

Estimaciones puntuales de photo-z, QP Ensembles y métricas de evaluación relacionadas con los resultados mostrados en la Tabla 4. Archivos cargados de los directorios listados en la Tabla 7 y descritos en el Apéndice A.4 de la nota técnica [SITCOMTN-154](https://sitcomtn-154.lsst.io/).




| Gold baseline | Gold DP1 optimize | Gold DP1 optimize  4band | 
|---|---|:-:| 
| [BPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/113_bpz_test_gold_baseline_sitcomtn154)               | [BPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/120_bpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [CMNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/114_cmnn_test_gold_baseline_sitcomtn154)             | [CMNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/121_cmnn_test_gold_dp1_optimize_sitcomtn154)             | :material-hammer-wrench: |
| [DNF test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/115_dnf_test_gold_baseline_sitcomtn154)               | [DNF test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/122_dnf_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [FlexZBoost test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/116_flexzboost_test_gold_baseline_sitcomtn154) | [FlexZBoost test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/123_flexzboost_test_gold_dp1_optimize_sitcomtn154) | :material-hammer-wrench: |
| [GPz test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/117_gpz_test_gold_baseline_sitcomtn154)               | [GPz test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/124_gpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| [kNN test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/118_knn_test_gold_baseline_sitcomtn154)               | [kNN test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/125_knn_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |
| N/A   | [LePhare test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/126_lephare_test_gold_dp1_optimize_sitcomtn154)       | :material-hammer-wrench: |
| [TPZ test gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/119_tpz_test_gold_baseline_sitcomtn154)               | [TPZ test gold DP1 optimize SITCOMTN-154](https://pzserver.linea.org.br/product/127_tpz_test_gold_dp1_optimize_sitcomtn154)               | :material-hammer-wrench: |


**Leyenda**<br>
:material-hammer-wrench: En preparación




### Estimaciones de Photo-z 

#### Tablas de Photo-z 

Tablas de PZ producidas como parte de los estudios iniciales con datos de comisionamiento descritos en [SITCOMTN-154](https://sitcomtn-154.lsst.io/). Datos cargados de los directorios listados en la Tabla 7.


| Producto de Datos  | Número de Objetos |
|--------------------|-------------------|
| [PZ table dp1_all gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/128_pz_table_dp1_all_gold_baseline_sitcomtn154) | 686.334  | 
| [PZ table dp1_sv38 gold baseline SITCOMTN-154](https://pzserver.linea.org.br/product/129_pz_table_dp1_sv38_gold_baseline_sitcomtn154) | 169.034  | 
|[PZ table DESI gold baseline](https://pzserver.linea.org.br/product/130_pz_table_desi_gold_baseline_sitcomtn154) | 2728  |
| PZ table dp1_all gold dp1_optimize | :material-hammer-wrench: <!--375,610-->  | 
| PZ table dp1_sv_38 gold dp1_optimize | :material-hammer-wrench:  | 
| PZ table dp1_all gold dp1_optimize 4band | :material-hammer-wrench:  | 
| PZ table dp1_sv_38 gold dp1_optimize 4band | :material-hammer-wrench:  | 

**Leyenda**<br>
:material-hammer-wrench: En preparación




--- 

## Conjuntos de Datos Externos 

Datos públicos recopilados de la literatura y alojados en el Photo-z Server.


### Catálogos de Redshifts de Referencia 

#### Estudios Individuales

El PZ Server aloja varios catálogos públicos de corrimientos al rojo espectroscópicos de diferentes estudios que pueden ser utilizados como conjuntos de datos de referencia para entrenamiento y validación de estimaciones de photo-z. Los productos de datos listados a continuación son los catálogos originales, sin ningún filtro o selección de datos.

| Producto de Datos | Referencia | Número de Corrimientos al Rojo | Estado |
|-------------------|-----------|--------------------------------|---| 
| [2dFGRS Final Data Release](https://pzserver.linea.org.br/product/170_2dfgrs_final_data_release) | [Colless et al. (2001)](https://ui.adsabs.harvard.edu/abs/2001MNRAS.328.1039C) | 245,591 | :material-check:  | 
| [2dFLens Final Data Release](https://pzserver.linea.org.br/product/171_2dflens_final_data_release) | [Blake et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.4240B) | 70,079 | :material-check:  | 
| [2MRS v240](https://pzserver.linea.org.br/product/172_2mrs_v240) | [Huchra et al. (2012)](https://ui.adsabs.harvard.edu/abs/2012ApJS..199...26H) | 240,496 | :material-check:  | 
| [3D-HST v415](https://pzserver.linea.org.br/product/173_3dhst_v415) | [Momcheva et al. (2016)](https://ui.adsabs.harvard.edu/abs/2016ApJS..225...27M) | 207,967 | :material-check:  | 
| [6dFGS DR3](https://pzserver.linea.org.br/product/174_6dfgs_dr3) | [Jones et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.399..683J) | 136,304 | :material-check:  | 
| ACES | - | - | :material-clock-outline: | 
| AMA DR4 | - | - | :material-clock-outline: |
| ATLAS | - | - | :material-clock-outline: | 
| [ASTRODEEP GS43](https://pzserver.linea.org.br/product/176_astrodeep_gs43) | [Merlin et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A&A...649A..22M/abstract) | 35,108 | :material-check:  | 
| [ASTRODEEP JWST](https://pzserver.linea.org.br/product/177_astrodeep_jwst) | [Merlin et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024A%26A...691A.240M/abstract) | 531,173 | :material-check:  | 
| C3R2 DR3 | - | - | :material-clock-outline: | 
| CANUCS SMACS | - | - | :material-clock-outline: | 
| CDB | - | - | :material-clock-outline: | 
| CLASH-VLT FR | - | - | :material-clock-outline: | 
| [COSMOS Specz Compilation DR1](https://pzserver.linea.org.br/product/212_cosmos_specz_compilation_dr1) | [Khostovan et al. (2025)](https://ui.adsabs.harvard.edu/abs/2026ApJS..282....6K/abstract) | 482,579 | :material-check:  |
| [COSMOS Web DR1 - Column Selection](https://pzserver.linea.org.br/product/214_cosmos_web_dr1__column_selection) | [Shuntov et al. (2025)](https://www.aanda.org/articles/aa/abs/2025/12/aa55799-25/aa55799-25.html) | 784,016 | :material-check:  |
| [COSMOS Web DR1 - LEPHARE Extension](https://pzserver.linea.org.br/product/220_cosmos_web_dr1__lephare_extension) | [Shuntov et al. (2025)](https://www.aanda.org/articles/aa/abs/2025/12/aa55799-25/aa55799-25.html) | 784,016 | :material-check:  |
| DEEP2 DR4 | - | - | :material-clock-outline: | 
| [DEIMOS 10K](https://pzserver.linea.org.br/product/215_deimos_10k) | [Hasinger et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018ApJ...858...77H/abstract) | 10,770 | :material-check:  |
| DESI EDR | [DESI Collaboration et al. (2024)](https://ui.adsabs.harvard.edu/abs/2024AJ....168...58D/abstract) | 2,451,325 |  :material-hammer-wrench:  | 
| [DESI DR1 within LSST DP1](https://pzserver.linea.org.br/product/178_desi_dr1_within_lsst_dp1) | [DESI Collaboration et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025arXiv250314745D/abstract) | 50,634 | :material-check:  | 
| [ELAISS1OID](https://pzserver.linea.org.br/product/231_elaiss1oid) | [Feruglio et al. (2008)](https://ui.adsabs.harvard.edu/abs/2008A%26A...488..417F/abstract) | 478 | :material-check:  | 
| Euclid Q1 SPE | - | - | :material-clock-outline: |
| [FMOS-COSMOS](https://pzserver.linea.org.br/product/219_fmoscosmos) | [Kashino et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019ApJS..241...10K/abstract) | 5,484 | :material-check:  |
| GLASS | - | - | :material-clock-outline: |
| HectoMAP DR2 | - | - | :material-clock-outline: |
| HETDEX DR1 | - | - | :material-clock-outline: |
| [JADES DR3](https://pzserver.linea.org.br/product/179_jades_dr3) | [D'Eugenio et al. (2025)](https://ui.adsabs.harvard.edu/abs/2025ApJS..277....4D/abstract) | 8,172 | :material-check:  | 
| LEGA-C DR3 |  - | - | :material-clock-outline: |
| [MOSDEF Final Data Release](https://pzserver.linea.org.br/product/181_mosdef_final_data_release) | [Kriek et al. (2015)](https://ui.adsabs.harvard.edu/abs/2015ApJS..218...15K/abstract) | 1,791 | :material-check:  |
| MUSE DR1 | - | - | :material-clock-outline: |
| [OzDES DR2](https://pzserver.linea.org.br/product/182_ozdes_dr2) | [Lidman et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.496...19L/abstract) | 38,624 | :material-check:  |  
| [PRIMUS DR1](https://pzserver.linea.org.br/product/183_primus_dr1) | [Coil et al. (2011)](https://ui.adsabs.harvard.edu/abs/2011ApJ...741....8C/abstract) | 213,696 | :material-check:  | 
| SAGA DR2 | - |  | :material-clock-outline: |
| SDSS DR17 | - |  | :material-clock-outline: |
| SpARCS | - |  | :material-clock-outline: |
| SPT-GMOS | - |  | :material-clock-outline: |
| UDS | - |  | :material-clock-outline: |
| [VANDELS DR4](https://pzserver.linea.org.br/product/185_vandels_dr4) | [Garilli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A%26A...647A.150G/abstract) | 2,165 | :material-check:  | 
| VIPERS | - | -  | :material-clock-outline: |
| [VLT VIMOS V2.0.1](https://pzserver.linea.org.br/product/186_vlt_vimos_v201) | [Balestra et al. (2010)](https://ui.adsabs.harvard.edu/abs/2010A%26A...512A..12B/abstract) | 5,052 | :material-check:  | 
| [VUDS DR1](https://pzserver.linea.org.br/product/187_vuds_dr1) | [Tasca et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017A%26A...600A.110T/abstract) | 698 | :material-check:  | 
| [VVDS Final Data Release](https://pzserver.linea.org.br/product/188_vvds_final_data_release) | [Le Fèvre et al. (2013)](https://ui.adsabs.harvard.edu/abs/2013A%26A...559A..14L/abstract) | 40,944 | :material-check:  |
| WiggleZ | - | -  | :material-clock-outline: | 
| [zCOSMOS Final Release](https://pzserver.linea.org.br/product/218_zcosmos_final_release) | [Lilly et al. (2016)](https://www.eso.org/rm/api/v1/public/releaseDescriptions/66) | 20,689 | :material-check:  | 
| ZFIRE | - | -  | :material-clock-outline: | 


**Leyenda**<br>
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible 


### Catálogos Combinados de Redshift (CRC)

Generados por el pipeline **[Combine Redshift Catalogs](https://docs.linea.org.br/sci-platforms/pz_server_crc.html)** del **[LSST Photo-z Server](https://docs.linea.org.br/sci-platforms/pz_server.html)**.

| Producto de Datos | Fecha de Lanzamiento | # de Levantamientos | # de Objetos | Estado |
|-------------------|----------------------|----------------------|--------------|--------|
| [CRC_CAT_F3_v1](https://pzserver.linea.org.br/product/194_crc_linea_2025_11_cat_f3_v1) | 25-11-2025 | 18 | 1.569.746 | :material-check: |
| [CRC_CMD_F3_v1](https://pzserver.linea.org.br/product/193_crc_linea_2025_11_cmd_f3_v1) | 25-11-2025 | 18 | 1.569.746 | :material-check: |
| [CRC_CRD_F3_v1](https://pzserver.linea.org.br/product/195_crc_linea_2025_11_crd_f3_v1) | 25-11-2025 | 18 | 1.026.130 | :material-check: |
| [CRC_CAT_F0_v1](https://pzserver.linea.org.br/product/201_crc_cat_f0_v1) | 25-11-2025 | 18 | 1.863.704 | :material-check: |
| [CRC_CMD_F0_v1](https://pzserver.linea.org.br/product/200_crc_cmd_f0_v1) | 25-11-2025 | 18 | 1.863.704 | :material-check: |
| [CRC_CRD_F0_v1](https://pzserver.linea.org.br/product/202_crc_crd_f0_v1) | 25-11-2025 | 18 | 1.243.643 | :material-check: |

**Leyenda**  
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible


### Conjuntos de Entrenamiento (TSM)

Generados por el pipeline **[Training Set Maker (TSM)](https://docs.linea.org.br/sci-platforms/pz_server_tsm.html)** del **[LSST Photo-z Server](https://docs.linea.org.br/sci-platforms/pz_server.html)**.

| Producto de Datos | Fecha de Lanzamiento | # de Objetos | Estado |
|-------------------|----------------------|--------------|--------|
| [TSM_CATF3v1_DP1McMSFD](https://pzserver.linea.org.br/product/199_tsm_catf3v1_dp1mcmsfd) | 25-11-2025 | 34.709 | :material-check: |
| [TSM_CMDF3v1_DP1McMSFD](https://pzserver.linea.org.br/product/197_tsm_linea_2025_11_cmdf3v1_dp1mcmsfd) | 25-11-2025 | 34.709 | :material-check: |
| [TSM_CRDF3v1_DP1McMSFD](https://pzserver.linea.org.br/product/198_tsm_crdf3v1_dp1mcmsfd) | 25-11-2025 | 21.870 | :material-check: |
| [TSM_CATF0v1_DP1McMSFD](https://pzserver.linea.org.br/product/203_tsm_catf0v1_dp1mcmsfd) | 25-11-2025 | 43.134 | :material-check: |
| [TSM_CMDF0v1_DP1McMSFD](https://pzserver.linea.org.br/product/205_tsm_cmdf0v1_dp1mcmsfd) | 25-11-2025 | 43.134 | :material-check: |
| [TSM_CRDF0v1_DP1McMSFD](https://pzserver.linea.org.br/product/204_tsm_crdf0v1_dp1mcmsfd) | 25-11-2025 | 30.199 | :material-check: |

**Leyenda**  
:material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación &emsp; :material-check: Disponible


<!--
Acceso rápido mediante la biblioteca `pzserver`: 

```python
pz_server.get_product('<dataset_name>') 
``` 

--> 




