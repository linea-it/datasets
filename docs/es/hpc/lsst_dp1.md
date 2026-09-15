
# LSST - Data Preview 1 (DP1)

## Acerca de

LSST DP1 fue el primer conjunto de datos preliminar basado en datos reales liberado internamente por LSST DM. Contiene productos de imágenes y catálogos resultantes del procesamiento realizado con LSST Science Pipelines v29, a partir de observaciones obtenidas con la Cámara de Comisionamiento de LSST en siete campos de aproximadamente 1 grado cuadrado, a lo largo de siete semanas a finales de 2024.

**Fecha de lanzamiento:** 30 de junio de 2022

<div class="button-container">

<a href="[https://dp1.lsst.io/](https://dp1.lsst.io/)" class="button-link">Página de documentación de DP1</a>

<a href="[https://doi.org/10.71929/rubin/2570308](https://doi.org/10.71929/rubin/2570308)" class="button-link">Información para la citación</a>

</div>

## Elegibilidad

Datos privados disponibles únicamente para miembros de la colaboración LSST: todos los científicos y estudiantes en EE. UU. y Chile, además de los miembros designados de los [equipos internacionales de contribución en especie](www\.lsst.org/scientists/international-drh-list). Para obtener más información, consulte el documento de política de datos [RDO-013](https://docushare.lsst.org/docushare/dsweb/Get/RDO-013).

## Cómo acceder

Los productos de datos alojados y mantenidos por LIneA están disponibles mediante diferentes métodos de acceso. Esta página proporciona información sobre cómo acceder a los productos de datos primarios y secundarios para su uso en el **entorno HPC**. Se puede acceder a ellos desde la plataforma [Open OnDemand](https://ondemand.linea.org.br/) de LIneA, ya sea a través del entorno JupyterLab (en el menú Interactive Apps) o del Shell Access Terminal (en el menú Clusters).

### Ubicación de los archivos

Los productos de datos se almacenan en los sistemas de archivos Lustre y NFS, según el tipo de archivo. En ambos casos, los directorios se encuentran mediante las variables de entorno `$DATA` y `$PUBLIC_DATA`, para datos bajo embargo y datos públicos, respectivamente.

### Estructura de directorios

Los productos de datos de LSST DP1 están organizados en la siguiente estructura de directorios:




```
$DATA/lsst/dp1/
    ├── primary
    │   ├── catalogs
    │   │   ├── object
    │   │   │   └── object_xxxxx_...xxx.parq # (29 files)
    │   │   ├── ss_object
    │   │   │   └──  ss_object_...xxx.parq
    │   │   └── ss_source
    │   │       └── ss_source_...xxx.parq
    │   ├── images
    │   └── maps
    └── secondary
        ├── catalogs
        │   ├── hips  # (HiPS catalog structure)
        │   └── object_collection # (LSDB HATS structure)
        └── images
            └── hips # (HiPS image structure)
```


Los conjuntos de datos *\_primary\_* son productos de datos originales proporcionados por LSST DM y transferidos al IDAC-BR, mientras que los conjuntos de datos *\_secondary\_* son productos de datos derivados generados por el equipo de LIneA.

## Información sobre los conjuntos de datos

### Object

Mediciones de objetos detectados en imágenes de coadición profunda.

Ruta: `$DATA/lsst/dp1/primary/catalogs/object/`

| Números clave |   |
|---|---|
| Número de archivos | 29 |
| Número de columnas | 1.296 |
| Número total de filas | 2.299.757 |
| Tamaño total | 6,3 GB |
| Formato del archivo (extensión) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#Object](https://sdm-schemas.lsst.io/dp1.html#Object)" class="button-link">Esquema del catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>

### SS Object

Parámetros derivados para objetos en movimiento (del Sistema Solar).

Ruta: `$DATA/lsst/dp1/primary/catalogs/ss_object/`

| Números clave |   |
|---|---|
| Número de archivos | 1 |
| Número de columnas | 3 |
| Número total de filas | 431 |
| Tamaño total | 300 KB |
| Formato del archivo (extensión) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#SSObject](https://sdm-schemas.lsst.io/dp1.html#SSObject)" class="button-link">Esquema del catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>

### SS Source

Parámetros físicos instantáneos para objetos en movimiento en el momento de cada observación.

Ruta: `$DATA/lsst/dp1/primary/catalogs/ss_source/`

| Números clave |   |
|---|---|
| Número de archivos | 1 |
| Número de columnas | 23 |
| Número total de filas | 5.988 |
| Tamaño total | 1,5 MB |
| Formato del archivo (extensión) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#SSSource](https://sdm-schemas.lsst.io/dp1.html#SSSource)" class="button-link">Esquema del catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>