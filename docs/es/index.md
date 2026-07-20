# Datos

Bienvenido a la página de documentación de datos del LIneA. Aquí encontrará información sobre los conjuntos de datos disponibles e instrucciones para acceder a ellos.


### Perfiles de usuario y niveles de acceso
LIneA ofrece diferentes perfiles de usuario, cada uno con niveles de acceso específicos a los datos y servicios disponibles. Para conocer qué servicios están disponibles para cada perfil, consulte la [tabla](https://docs.linea.org.br/es/sci-platforms/index.html#acceso-a-los-servicios-y-plataformas-de-linea) disponible en la página de información sobre las plataformas científicas en el sitio de [documentación para usuarios](https://docs.linea.org.br/es/). 



---

## Catálogos

El acceso a datos tabulares (catálogos) se realiza a través de diferentes aplicaciones de la [LIneA Science Platform (LSP)](https://scienceplatform.linea.org.br/lsp), según el tamaño, el tipo o los niveles de permiso de acceso establecidos por el estudio astronómico de origen.

Para navegar, utilice el menú de la izquierda y explore los diferentes conjuntos de datos organizados según las opciones de uso:

- **Descarga** y **acceso programático** con [LSDB](https://lsdb.io/) (datos en formato [HATS](https://hats.readthedocs.io/en/latest/))
- **Consulta** en base de datos, a través de las plataformas [User Query](https://userquery.linea.org.br/), [Jupyter Hub](https://jupyter.linea.org.br/) o [TAP Service](https://userquery.linea.org.br/cms/services/scripted-access/)
- **Procesamiento** en el entorno HPC de datos almacenados en el sistema Lustre, con acceso a través de la plataforma [Open OnDemand](https://ondemand.linea.org.br)
- **Visualización** de información de catálogos superpuesta a imágenes [HiPS](https://aladin.cds.unistra.fr/hips/)

A continuación se muestra una tabla resumen de los principales catálogos disponibles para descarga o consulta a través de los diferentes servicios:

| Survey / release      | LSDB                     | Base de datos            | HPC                      | HiPS Catalog             |
|-----------------------|--------------------------|--------------------------|--------------------------|--------------------------|
| 2MASS PSC             | :material-account-group: | :material-account-group: | :material-lock:          | :material-account-group: |
| COSMO DC2             | -                        | -                        | :material-lock:          | -                        |
| DELVE DR2             | :material-account-group: | -                        | :material-lock:          | -                        |
| DES DR2 Main          | :material-account-group: | :material-account-group: | :material-lock:          | :material-account-group: |
| DES DR2 Y6 Gold       | :material-account-group: | :material-account-group: | :material-lock:          | :material-hammer-wrench: |
| DESI DR1              | :material-account-group: | -                        | :material-lock:          | -                        |
| eRASS1 Main           | :material-account-group: | -                        | :material-lock:          | -                        |
| Euclid Q1             | :material-account-group: | -                        | :material-lock:          | -                        |
| Gaia DR3 Source       | :material-account-group: | :material-account-group: | :material-lock:          | -                        |
| GALEX                 | :material-account-group: | -                        | :material-lock:          | :material-account-group: |
| HSC                   | :material-account-group: | -                        | :material-lock:          | -                        |
| LSST DP0.1            | -                        | -                        | :material-lock:          | -                        |
| LSST DP0.2            | -                        | :material-lock:          | :material-lock:          | -                        |
| LSST DP1              | :material-lock:          | :material-lock:          | :material-lock:          | :material-lock:          |
| LSST DP2              | :material-hammer-wrench: | :material-hammer-wrench: | :material-hammer-wrench: | :material-hammer-wrench: |
| LSST DR1-DR11         | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: |
| MPC                   | -                        | :material-account-group: | -                        | -                        |
| Pan-STARRS            | :material-account-group: | -                        | :material-lock:          | -                        |
| S-PLUS                | :material-clock-outline: | -                        | :material-clock-outline: | -                        |
| SDSS DR7              | :material-account-group: | -                        | :material-lock:          | -                        |
| SkyMapper             | :material-account-group: | -                        | :material-lock:          | -                        |
| TESS                  | :material-account-group: | -                        | :material-lock:          | -                        |
| TNS                   | :material-account-group: | -                        | :material-lock:          | -                        |
| VSX                   | :material-account-group: | -                        | :material-lock:          | -                        |
| WISE                  | :material-account-group: | -                        | :material-lock:          | -                        |
| ZTF                   | :material-account-group: | -                        | :material-lock:          | -                        |

**Leyenda**<br>
:material-account-group: Público &emsp; :material-lock: Acceso restringido &emsp; :material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación

---

## Imágenes

El acceso a las imágenes astronómicas se realiza a través de diferentes aplicaciones de la LIneA Science Platform, según el tipo de imagen y el estudio astronómico de origen.

- Imágenes [HiPS](https://aladin.cds.unistra.fr/hips/) (Hierarchical Progressive Surveys): **visualización global** y **navegación** a través de la aplicación [Sky Viewer](https://skyviewer.org/), o para apuntar a una lista de objetivos preseleccionados en el [Target Viewer](https://targetviewer.linea.org.br/).

- Imágenes [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) coadicionadas: **descarga** de cutouts a través del [Target Viewer](https://targetviewer.linea.org.br/), **acceso programático** vía API a través de [Jupyter Hub](https://jupyter.linea.org.br/) o **procesamiento** en el entorno HPC, con acceso a través de la plataforma [Open OnDemand](https://ondemand.linea.org.br).

- Imágenes [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) de exposición única: **acceso programático** vía API a través de [Jupyter Hub](https://jupyter.linea.org.br/) o **procesamiento** en el entorno HPC, con acceso a través de la plataforma [Open OnDemand](https://ondemand.linea.org.br).

A continuación se muestra una tabla resumen de los principales conjuntos de imágenes disponibles para descarga o consulta a través de los diferentes servicios:

| Survey / release            | HiPS                                      | FITS coadicionadas                        | FITS de exposición única             |
|-----------------------------|-------------------------------------------|-------------------------------------------|--------------------------------------|
| DES DR2                     | :material-account-group: :material-floppy:| :material-account-group: :material-floppy:| :material-lock: :material-floppy:    |
| Rubin First Look            | :material-account-group: :material-floppy:| -                                         | -                                    |
| LSST DP0.1                  | -                                         | :material-lock: :material-link:           | :material-lock: :material-link:      |
| LSST DP0.2                  | :material-lock: :material-floppy:         | :material-lock: :material-link:           | :material-lock: :material-link:      |
| LSST DP1                    | :material-lock: :material-floppy:         | :material-lock: :material-floppy:         | :material-lock: :material-link:      |
| LSST DP2                    | :material-clock-outline: :material-floppy:| :material-clock-outline: :material-floppy:| :material-clock-outline: :material-link:|
| LSST DR1-DR11               | :material-clock-outline: :material-floppy:| :material-clock-outline: :material-floppy:| :material-clock-outline: :material-link:|
| 2MASS colored               | :material-account-group: :material-link:  | -                                         | -                                    |
| AllWISE                     | :material-account-group: :material-link:  | -                                         | -                                    |
| DECaPS DR2                  | :material-account-group: :material-link:  | -                                         | -                                    |
| DSS Colored                 | :material-account-group: :material-link:  | -                                         | -                                    |
| DSS2 Red (F+R)              | :material-account-group: :material-link:  | -                                         | -                                    |
| Density Map Gaia EDR3       | :material-account-group: :material-link:  | -                                         | -                                    |
| Fermi Color                 | :material-account-group: :material-link:  | -                                         | -                                    |
| GALEXGR6_7 NUV              | :material-account-group: :material-link:  | -                                         | -                                    |
| GLIMPSE360                  | :material-account-group: :material-link:  | -                                         | -                                    |
| Halpha                      | :material-account-group: :material-link:  | -                                         | -                                    |
| IRAC color I1,I2,I4         | :material-account-group: :material-link:  | -                                         | -                                    |
| IRAC colored                | :material-account-group: :material-link:  | -                                         | -                                    |
| Mellinger colored           | :material-account-group: :material-link:  | -                                         | -                                    |
| PanSTARRS DR1 colored       | :material-account-group: :material-link:  | -                                         | -                                    |
| PanSTARRS DR1 g             | :material-account-group: :material-link:  | -                                         | -                                    |
| SDSS9 band-g                | :material-account-group: :material-link:  | -                                         | -                                    |
| SDSS9 colored               | :material-account-group: :material-link:  | -                                         | -                                    |
| VTSS-Ha                     | :material-account-group: :material-link:  | -                                         | -                                    |
| eROSITA-DE DR1 RGB          | :material-account-group: :material-link:  | -                                         | -                                    |

**Leyenda**<br>
:material-account-group: Público &emsp; :material-lock: Acceso restringido &emsp; :material-clock-outline: Planificado &emsp; :material-hammer-wrench: En preparación

:material-floppy: Copia local &emsp; :material-link: Acceso remoto

---

LIneA - Laboratorio Interinstitucional de e-Astronomía - es un laboratorio multiusuario, operado por una organización sin fines de lucro (Asociación LIneA) con el apoyo del Ministerio de Ciencia, Tecnología e Innovación de Brasil.

Para obtener más información, visite [https://www.linea.org.br](https://www.linea.org.br).