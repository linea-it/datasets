# Dark Energy Survey Y6 Gold

The Dark Energy Survey Year 6 (DES Y6) Gold presents a curated photometric data set derived from the full six years of DES observations (2013 August–2019 January) using the Dark Energy Camera on the 4m Blanco telescope at Cerro Tololo Inter-American Observatory in Chile, specifically optimized for static-sky cosmology analyses.

DES Y6 Gold is assembled from DES Data Release 2 and comprises approximately 5000 deg² of grizY imaging in the southern Galactic cap. The data set incorporates advanced multi-epoch photometry, improved calibration, enhanced object classification, and comprehensive ancillary products including footprint masks, survey property maps, and photometric redshift estimates.

The resultant Y6 Gold catalog contains 669 million high-quality objects detected across the survey footprint. After quality selections, benchmark samples include 448 million galaxies and 120 million stars.

The survey achieved uniform, deep photometry with precise astrometry and robust object classification. Key performance metrics include:

* **Median PSF FWHM**: g=1.13", r=0.99", i=0.90", z=0.87", Y=0.93"
* **Survey Coverage**: 4923 deg² (requiring ≥2 exposures in griz)
* **Photometric Depth** (1.95" aperture, S/N=10): g=24.7, r=24.4, i=23.8, z=23.1, Y=21.7 mag
* **Multi-Epoch Galaxy Depth** (S/N=10, BDF model): i=23.4 mag
* **90% Completeness Limit** (extended objects): g=23.9, r=23.2, i=22.7, z=22.4 mag
* **Photometric Uniformity**: <2 mmag relative to Gaia G band
* **Astrometric Precision**: ~27 mas (median internal precision)
* **Star-Galaxy Classification** (17.5≤i≤22.5): Galaxy efficiency 98.6% with 0.8% contamination; Stellar efficiency 94.6% with 1.5% contamination
* **Object Density**: 37.4 arcmin⁻² overall; 28.9 arcmin⁻² for high-confidence galaxies

<figure class="dataset-figure">
<img src="../../images/des/DES_Y6_Gold.webp" alt="Dark Energy Survey Y6 Gold Angular Density Map">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/des/des_y6_gold')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/des/des_y6_gold/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 691,483,608    | 336               | 1,582               | 1.3 TiB      |

<div class="button-container">
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6gold" class="button-link">Official Release</a>
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6gold" class="button-link">Column Descriptions</a>
<a href="https://arxiv.org/abs/2501.05739" class="button-link">Research Paper</a>
</div>
