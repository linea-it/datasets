# DELVE Survey - Data Release 2

The DECam Local Volume Exploration Survey Data Release 2 (DELVE DR2) combines new DECam observations with archival DECam data from the Dark Energy Survey (DES), the DECam Legacy Survey (DECALS), and other DECam community programs. Its primary science goal is to discover and characterize faint satellite galaxies and other resolved stellar systems in the Local Volume. DELVE DR2 covers more than four times the area and contains roughly five times as many astronomical objects compared to the previous data release.

## Survey Coverage and Catalog

The survey assembled approximately 160,000 exposures (161,380 total) from more than 270 DECam community programs. It covers more than 21,000 square degrees of sky, focusing on high Galactic latitude regions (absolute Galactic latitude greater than 10 degrees). The survey uses four broadband optical and near-infrared filters: g, r, i, and z bands.

The 4-band intersection covers approximately 17,000 square degrees (16,972 deg²) and provides complete 4-band photometry for about 618 million sources. The total catalog contains roughly 2.5 billion sources, including both point-source and automatic aperture photometry measurements.

## Key Performance Metrics

**Image Quality:** The median point spread function (PSF) full width at half maximum (FWHM) varies by band: g-band has 1.24 arcsec, r-band has 1.10 arcsec, i-band has 1.02 arcsec, and z-band has 1.00 arcsec.

**Sensitivity (PSF photometry at S/N=5):** The median point-source depth reaches g=24.3 mag, r=23.9 mag, i=23.5 mag, and z=22.8 mag.

**Sensitivity (AUTO photometry at S/N=5):** The median automatic aperture depth reaches g=23.9 mag, r=23.5 mag, i=23.0 mag, and z=22.4 mag.

**Astrometric Accuracy:** The median angular distance offset versus Gaia EDR3 is 22 milliarcseconds (mas).

**Photometric Repeatability:** The median root-mean-square (rms) scatter is 4.9 mmag (g-band), 5.0 mmag (r-band), 4.5 mmag (i-band), and 5.4 mmag (z-band).

**Absolute Photometric Uncertainty:** The estimated absolute photometric accuracy is 20 mmag or better across all bands.

<figure class="dataset-figure">
<img src="../../images/delve/DELVE_DR2.webp" alt="2MASS Point Source Catalog">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>


## Load using LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/delve_dr2')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/delve_dr2/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 2,500,247,752  | 120               | 5,513               | 836 GiB      |

<div class="button-container">
<a href="https://datalab.noirlab.edu/data/delve" class="button-link">Official Release</a>
<a href="https://datalab.noirlab.edu/data/delve" class="button-link">Column Descriptions</a>
<a href="https://arxiv.org/abs/2203.16565" class="button-link">Research Paper</a>
</div>

