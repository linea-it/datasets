# Databases

LIneA provides public and private astronomical catalogs in **PostgreSQL** databases through the [User Query](https://userquery.linea.org.br/) platform. Users can query the data with **SQL** or **ADQL** and save results as tables in their personal area (MyDB), which is also accessible from [Target Viewer](https://target.linea.org.br/) and [JupyterHub](https://jupyter.linea.org.br/). Instructions, tutorials, and query examples are in the [platform documentation](https://docs.linea.org.br/en/sci-platforms/user_query.html).

!!! private "Restricted Access"
    Schema availability follows each project's data policy. Restricted catalogs are visible and queryable only to authorized users.

## Available content

### Dark Energy Survey — Data Release 2

`des_dr2` · [View schema](https://userquery.linea.org.br/metadata/des_dr2/)

A photometric catalog from the DES survey covering approximately 5,000 square degrees of the southern sky, with astrometry, *grizY* photometry, star/galaxy classification, and quality flags.

### DES Year 6 Gold

`des_y6_gold` · [View schema](https://userquery.linea.org.br/metadata/des_y6_gold/)

Final DES Y6 products for cosmological analyses: the Gold galaxy and star catalog, a WaZP galaxy cluster catalog, and its member galaxies, including membership probabilities and photometry.

### Gaia Data Release 3

`gaia_dr3` · [View schema](https://userquery.linea.org.br/metadata/gaia_dr3/)

Gaia DR3 astrometric and photometric data, including positions, parallaxes, proper motions, radial velocities, variability, astrophysical parameters, and source classifications.

### LSST Data Preview 1

`lsst_dp1` · [View schema](https://userquery.linea.org.br/metadata/lsst_dp1/) · :material-lock: Restricted Access

Catalogs produced from Rubin Observatory Data Preview 1, with source and object measurements derived from the first LSSTComCam observations and related products.

### Minor Planet Center - SBN mirror

`mpc_sbn` · [View schema](https://userquery.linea.org.br/metadata/mpc_sbn/)

A mirror of Minor Planet Center data provided by the Small Bodies Node, with observations, orbits, designations, names, and observatory information for small Solar System bodies.

### Two Micron All Sky Survey

`twomass` · [View schema](https://userquery.linea.org.br/metadata/twomass/)

The 2MASS Point Source Catalog, from a near-infrared survey of nearly the entire sky, containing positions, magnitudes, and quality indicators in the *J*, *H*, and *Ks* bands.
