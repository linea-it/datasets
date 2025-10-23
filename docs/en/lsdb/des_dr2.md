# Dark Energy Survey - Data Release 2

The Dark Energy Survey Data Release 2 (DES DR2) presents reduced single-epoch and coadded images, source catalogs, and associated data products from six years of DES science operations (2013 August–2019 January) using the Dark Energy Camera (DECam) on the 4 m Blanco telescope at Cerro Tololo Inter-American Observatory in Chile.

DES DR2 comprises data from the wide-area survey covering approximately 5000 deg² of the southern Galactic cap in five broad photometric bands (grizY). The release consists of 96,263 single-epoch exposures processed into 10,169 coadded image tiles of 0.534 deg² each, derived from 76,217 science-quality exposures.

The resultant DES DR2 catalog contains 691,483,608 distinct astronomical objects detected across the footprint. After basic quality selection, benchmark samples include 543 million galaxies and 145 million stars.

The survey achieved uniform, deep photometry and precise astrometry. Key performance metrics include:

* **Median PSF FWHM**: g=1.11", r=0.95", i=0.88", z=0.83", Y=0.90"
* **Photometric Depth** (1.95" aperture, S/N=10): g=24.7, r=24.4, i=23.8, z=23.1, Y=21.7 mag
* **95% Completeness Limit**: g=24.6, r=24.3, i=24.0, z=23.7, Y=23.4 mag
* **Photometric Uniformity**: <3 mmag (1σ) relative to Gaia DR2 G band
* **Absolute Photometric Accuracy**: ~11 mmag systematic uncertainty
* **Astrometric Precision**: ~27 mas (1σ) internal precision in coadd
* **Spurious Object Rate**: ~1%
* **Star-Galaxy Separation**: >99% galaxy efficiency, >94% stellar efficiency for 19.0<i<22.5

DES DR2 constitutes the largest photometric data set to date at the achieved depth and photometric precision. 

<figure class="dataset-figure">
<img src="../../images/des/DES_DR2.webp" alt="Dark Energy Survey Data Release 2 Angular Density Map">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/des2/des_dr2')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/des2/des_dr2/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 662,428,385    | 215               | 1,523               | 667 GB       |

<div class="button-container">
<a href="https://www.darkenergysurvey.org/dr2/" class="button-link">Official Release</a>
<a href="https://des.ncsa.illinois.edu/releases/dr2/dr2-access" class="button-link">Column Descriptions</a>
<a href="https://arxiv.org/abs/2101.05765" class="button-link">Research Paper</a>
</div>
