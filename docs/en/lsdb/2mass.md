# Two Micron All Sky Survey (2MASS)

The Two Micron All Sky Survey (2MASS) collected 25.4 Tbytes of raw imaging data between 1997 June and 2001 February, covering 99.998% of the celestial sphere in the near-infrared J (1.25 μm), H (1.65 μm), and Ks (2.16 μm) bandpasses. Observations were conducted using two dedicated 1.3 m telescopes at Mount Hopkins, Arizona, and Cerro Tololo, Chile.

The resultant 2MASS All-Sky Data Release comprises 4,121,439 FITS images and catalogs derived from final data processing. The principal data products include a Point Source Catalog of 470,992,970 sources and an Extended Source Catalog of 1,647,599 objects.

The survey achieved uniform, precise photometry and astrometry. Key performance metrics for the Point Source Catalog include:

* Sensitivity (S/N=10): Better than J=15.8, H=15.1, and Ks=14.3 mag for virtually the entire sky.
* Reliability: Greater than 99.95% for sources with S/N ≥ 10 in any one band.
* Completeness: Greater than 99% for sources with S/N ≥ 10 in any one band.
* Photometric Accuracy (Bright Sources): <0.03 mag (1σ).
* Astrometric Accuracy: ~100 mas (1σ) relative to the ICRS.
* Dynamic Range: >20 mag.

<figure class="dataset-figure">
<img src="../../images/2mass/2MASS_PSC.webp" alt="2MASS Point Source Catalog">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/two_mass')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/two_mass/
```

## Catalog metadata

| Number of rows     | Number of columns | Number of partitions | Size on disk |
|--------------------|-------------------|---------------------|--------------|
| 470,992,970        | 63                | 1,107               | 43 GB        |

<div class="button-container">
<a href="https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec2_2.html" class="button-link">Official Release</a>
<a href="https://irsa.ipac.caltech.edu/data/2MASS/docs/releases/allsky/doc/sec2_2a.html" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2006AJ....131.1163S/abstract" class="button-link">Research Paper</a>
</div>
