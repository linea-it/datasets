# Data

Welcome to the LIneA data documentation page. Here you will find information about available datasets and instructions on how to access them.

To access the main user documentation page, with information about all services and tools offered to the astronomical community and the general public, visit: [https://docs.linea.org.br](https://docs.linea.org.br).

---

## Catalogs

Access to tabular data (catalogs) is provided through different applications of the [LIneA Science Platform (LSP)](https://scienceplatform.linea.org.br/lsp), depending on the size, type, or access permission levels established by the originating astronomical survey.

To navigate, use the menu on the left and explore the different datasets organized according to usage options:

- **Download** and **programmatic access** with [LSDB](https://lsdb.io/) (data in [HATS](https://hats.readthedocs.io/en/latest/) format)
- **Query** in databases, through the [User Query](https://userquery.linea.org.br/), [Jupyter Hub](https://jupyter.linea.org.br/), or [TAP Service](https://userquery.linea.org.br/cms/services/scripted-access/) platforms
- **Processing** in the HPC environment of data stored in the Lustre system, with access through the [Open OnDemand](https://ondemand.linea.org.br) platform
- **Visualization** of catalog information overlaid on [HiPS](https://aladin.cds.unistra.fr/hips/) images

Below is a summary table of the main catalogs available for download or query through the different services:

| Survey / release      | LSDB                     | Database                 | HPC                      | HiPS Catalog             |
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
| LSST DP2              | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: |
| LSST DR1-DR11         | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: | :material-clock-outline: |
| MPC                   | -                        | :material-account-group: | -                        | -                        |
| Pan-STARRS            | :material-account-group: | -                        | :material-lock:          | -                        |
| S-PLUS                | :material-clock-outline: | -                        | :material-clock-outline: | -                        |
| SDSS DR7              | :material-account-group: | -                        | :material-lock:          | -                        |
| SIMBAD                | -                        | -                        | -                        | :material-account-group: |
| SkyMapper             | :material-account-group: | -                        | :material-lock:          | -                        |
| TESS                  | :material-account-group: | -                        | :material-lock:          | -                        |
| TNS                   | :material-account-group: | -                        | :material-lock:          | -                        |
| VSX                   | :material-account-group: | -                        | :material-lock:          | -                        |
| WISE                  | :material-account-group: | -                        | :material-lock:          | -                        |
| ZTF                   | :material-account-group: | -                        | :material-lock:          | -                        |

**Legend**<br>
:material-account-group: Public &emsp; :material-lock: Restricted access &emsp; :material-clock-outline: Planned &emsp; :material-hammer-wrench: In preparation

---

## Images

Access to astronomical images is provided through different applications of the LIneA Science Platform, depending on the image type and the originating astronomical survey.

- [HiPS](https://aladin.cds.unistra.fr/hips/) (Hierarchical Progressive Surveys) images: **global visualization** and **navigation** through the [Sky Viewer](https://skyviewer.org/) application, or for pointing to a pre-selected list of targets in the [Target Viewer](https://targetviewer.linea.org.br/).

- Coadded [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) images: **download** of cutouts through the [Target Viewer](https://targetviewer.linea.org.br/), **programmatic access** via API through [Jupyter Hub](https://jupyter.linea.org.br/), or **processing** in the HPC environment, with access through the [Open OnDemand](https://ondemand.linea.org.br) platform.

- Single-exposure [FITS](https://fits.gsfc.nasa.gov/) (Flexible Image Transport System) images: **programmatic access** via API through [Jupyter Hub](https://jupyter.linea.org.br/), or **processing** in the HPC environment, with access through the [Open OnDemand](https://ondemand.linea.org.br) platform.

Below is a summary table of the main image datasets available for download or query through the different services:

| Survey / release            | HiPS                                      | Coadded FITS                              | Single-exposure FITS                 |
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

**Legend**<br>
:material-account-group: Public &emsp; :material-lock: Restricted access &emsp; :material-clock-outline: Planned &emsp; :material-hammer-wrench: In preparation

:material-floppy: Local copy &emsp; :material-link: Remote access

---

LIneA - Laboratório Interinstitucional de e-Astronomia - is a multi-user laboratory, operated by a non-profit organization (Associação LIneA) with support from the Brazilian Ministry of Science, Technology and Innovation.

To learn more, visit [https://www.linea.org.br](https://www.linea.org.br).

