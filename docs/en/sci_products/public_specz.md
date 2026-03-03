LIneA provides a collection of spectroscopic *redshift* (spec-z) catalogs that have been publicly released and thoroughly described in the scientific literature by their originating projects. These catalogs were collected over the years of operation of the Dark Energy Survey (DES) and systematically assembled using a tool from the DES Science Portal (*pipeline* Spectroscopic Sample, [Gschwend et al., 2018](https://ui.adsabs.harvard.edu/abs/2018A%26C....25...58G/abstract)) to form the basis of a training set for machine learning–based photometric *redshift* estimation algorithms. The original version of the compiled catalog used in the DES context includes proprietary data from the OzDES survey ([Yuan et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.452.3047Y/abstract)) as well as other proprietary data from smaller surveys.

A reduced version of the sample containing approximately ~3.6 million *redshifts*, along with the result of its cross-match with DES DR2 photometric data, is temporarily available for download in Parquet format (see commands below).

Soon, this sample will be made available to users of the [**LIneA Science Platform**](https://scienceplatform.linea.org.br/lsp), with access through the [**User Query**](https://docs.linea.org.br/sci-platforms/user_query.html) interface or programmatically via the [**TAP Service**](https://docs.linea.org.br/sci-platforms/user_query.html#tap-service), and it will undergo regular updates with the addition of data from new surveys.

## Compiled Catalog of Public Spectroscopic *Redshifts*

### Download

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_specz_compilation.pq
```

### Characterization

A detailed characterization of the compiled catalog of public spectroscopic *redshifts* can be found in [this notebook](https://datasets.linea.org.br/redshifts/public-specz-compilation.html). **Note: the data access method used in the notebook is outdated; please disregard it.**

## Public Training Set for Photometric *Redshifts*

### Download

```bash
$ wget -c https://datasets.linea.org.br/redshifts/public_pz_training_set.pq
```

### Characterization

A detailed characterization of the public training set for photometric *redshifts* can be found in [this notebook](https://datasets.linea.org.br/redshifts/public-training-set-des-dr2.html). **Note: the data access method used in the notebook is outdated; please disregard it.**
