# Productos FITS del LSST DP2

El **Legacy Survey of Space and Time Data Preview 2 (LSST DP2)** contiene productos de imágenes y catálogos generados por Rubin Science Pipelines v30.0.8 a partir de observaciones de LSSTCam obtenidas entre abril de 2025 y enero de 2026. El Early DP2 se publicó el 27 de julio de 2026. En esta fase, el producto de imagen publicado es el deep coadd. Las imágenes de visita y de diferencia forman parte del lanzamiento completo, previsto para octubre–diciembre de 2026.

- [Documentación oficial del DP2](https://dp2.lsst.io/)
- [Productos de datos del DP2](https://dp2.lsst.io/products/index.html)
- [Citación oficial del conjunto](https://doi.org/10.71929/rubin/3382528)

## Nivel de acceso

!!! private "Acceso restringido"
    El DP2 es propietario y está disponible solamente para titulares de derechos de datos de Rubin, según la [política de datos](https://rubinobservatory.org/for-scientists/data-products/data-policy) y el documento [RDO-013](https://docushare.lsst.org/docushare/dsweb/Get/RDO-013).

## Productos disponibles en LIneA

!!! info "Inventario local"
    Las cantidades presentadas en esta página documentan los archivos disponibles en la infraestructura de LIneA.

## Cobertura del cielo por banda

Los deep coadds cubren cerca de 3.000 grados cuadrados en las regiones Wide-Fast-Deep, Small Field Survey y Deep Drilling Fields. Las visitas individuales cubren cerca de 15.000 grados cuadrados, pero esas imágenes no forman parte de esta copia.

La copia local reúne 197.105 patches en 2.191 tracts, con identificadores entre 2054 y 13041. La declinación de esos patches va de −52,16° a +22,90°, y la ascensión recta recorre el círculo completo. No todos los patches existen en todas las bandas; la tabla siguiente muestra el conteo por filtro.

!!! info "Cómo interpretar la cobertura"
    Cada archivo es un patch del skymap. Los deep coadds incluyen solamente exposiciones que cumplen los criterios de calidad; los patches de borde pueden contener regiones sin datos, identificadas por la máscara `NO_DATA`.

Fuentes oficiales: [documentación del DP2](https://dp2.lsst.io/), [deep coadd](https://dp2.lsst.io/products/images/deep_coadd.html) y [coadición de imágenes](https://dp2.lsst.io/processing/coaddition/index.html).

### Deep coadd

Combinación, por banda y patch, de exposiciones calibradas y con el fondo sustraído. El apilado es una coadición por celdas, con media ponderada por el inverso de la varianza. Cada archivo es un `CellCoadd` en una de las seis bandas `u`, `g`, `r`, `i`, `z` e `y`.

- **Formato:** FITS (`.fits`)
- **Inventario local:** 925.460 archivos, 27,71 TB
- **Contenido:** planos de imagen (nJy), varianza (nJy²) y máscara, además de PSF, calibración fotométrica y WCS
- **Documentación oficial:** [Deep coadd](https://dp2.lsst.io/products/images/deep_coadd.html) y [coadición de imágenes](https://dp2.lsst.io/processing/coaddition/index.html)

| Banda | Archivos | Tracts | Tamaño |
|---|---:|---:|---:|
| u | 114.892 | 1.405 | 3,31 TB |
| g | 155.115 | 1.799 | 4,57 TB |
| r | 171.856 | 1.999 | 5,20 TB |
| i | 177.588 | 2.030 | 5,41 TB |
| z | 166.412 | 1.884 | 5,07 TB |
| y | 139.597 | 1.590 | 4,16 TB |

La columna Tracts cuenta tracts distintos en esa banda. La unión de las seis bandas tiene 2.191 tracts.

## Límites de este inventario

Esta página describe solamente los deep coadds de la copia local de LIneA. En este conjunto no hay `deep_coadd_background`, `deep_coadd_n_image` ni mapas HealSparse. El Early DP2 oficial también limita los productos de imagen a los deep coadds. Raw exposures, visit images, template coadds y difference images no están registrados como disponibles en esta copia. Consulta el [índice de productos del DP2](https://dp2.lsst.io/products/index.html).
