# Catálogos de Cúmulos WaZP DES Y6 Gold

!!! Warning "Aviso"
    Página en construcción. Algunos contenidos pueden estar incompletos o desactualizados.

## Resumen
Benoist et al. (2025) presentan un catálogo de cúmulos de galaxias detectado con el WaZP cluster finder, independiente de la detección por secuencia roja, utilizando seis años de datos del Dark Energy Survey (DES-Y6). El catálogo completo incluye más de 400,000 cúmulos con Ngals > 5, alcanzando corrimientos al rojo de hasta z = 1,3. Una versión homogenizada para uso en cosmología contiene 33,000 cúmulos ricos (Ngals > 25).

La comparación con el catálogo WaZP anterior basado en los datos del primer año del DES (DES-Y1) muestra que casi todos los cúmulos dentro de la huella y profundidad superpuestas son recuperados. Las observaciones más profundas del DES-Y6 y una muestra espectroscópica más completa mejoran las estimaciones de corrimiento al rojo, con una dispersión media de 1,4% y un offset medio de 0,2%.

Los cúmulos ópticos se cruzaron con muestras SZE de los telescopios SPT y ACT. Casi todos los cúmulos SZE en regiones superpuestas tienen un correspondiente WaZP, y el 90% de los cúmulos ópticos con riqueza > 150 tienen equivalentes en las regiones profundas de los estudios SZE. Aproximadamente el 15–20% de los sistemas SZE emparejados presentan múltiples cúmulos WaZP dentro de R500c al mismo corrimiento al rojo, indicando sistemas posiblemente interactuantes o no relajados. Los centrados de cúmulos WaZP y SZE son consistentes considerando los tamaños de los haces.

## Acceso a Datos

- Catálogo de cúmulos: [y6a2_dnf_wazp_v5.0.12.6801_clusters.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits)
- Miembros de los cúmulos: [y6a2_dnf_wazp_v5.0.12.6801_members.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits)
- Mapa de cobertura: [y6a2_dnf_wazp_v5.0.12.6801_footprint.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits)

### Descargar con wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits
```

```
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits
```

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits
```

<div class="button-container"> <a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6cluster-wazp" class="button-link">Descripción de Columnas</a> <a href="https://arxiv.org/abs/2507.05360t" class="button-link">Artículo Científico</a> </div>


