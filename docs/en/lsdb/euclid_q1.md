# Euclid Quick Data Release 1

The Euclid mission, an ESA space mission primarily aimed at studying dark matter and dark energy using weak lensing and galaxy clustering, commenced its nominal wide survey operations in February 2024. The first Euclid Quick Data Release (Q1), made public in March 2025, provides an early look at the survey's capabilities. Q1 comprises visible and near-infrared space-based imaging and spectroscopic data from the VIS instrument and the Near-Infrared Spectrometer and Photometer (NISP), supplemented by ground-based photometry in u, g, r, i, and z bands, processed with early versions of the Euclid pipelines.

Q1 encompasses 63.1 square degrees covering three Euclid Deep Fields (EDF-N, EDF-S, EDF-F) observed to the nominal single-visit depth of the Euclid Wide Survey (EWS). The data includes imaging in VIS (IE) and NISP (YE, JE, HE) bands, as well as NISP slitless spectroscopy using the red grism (1.206–1.892 µm). Ground-based data primarily originates from the UNIONS survey for EDF-N and the Dark Energy Survey (DES) and other DECam observations for EDF-S and EDF-F. Q1 also includes deeper observations (about 17 times EWS exposure) of a 0.5 square degree area in the LDN 1641 dark cloud.

The Q1 catalogue contains approximately 30 million objects across the three EDF areas.

Key performance metrics and survey characteristics include:

* **VIS Spatial Resolution:** 0.18"
* **NISP Spatial Resolution:** 0.3" per pixel
* **Photometric Depth (Ground-based, 10σ, 2" aperture, typical for EDF-N):** g ≈ 25.3, r ≈ 24.3, i ≈ 23.7, z ≈ 23.6 mag
* **Astrometric Calibration Frame:** Gaia DR3
* **Absolute Photometric Calibration Frame:** HST CALSPEC
* **Internal Photometric Scatter (Ground-based coadds vs Gaia synthetic):** ~1% (NMAD)
* **Spectroscopic Targets:** Sources with HE ≤ 22.5
* **Spectroscopic Redshift Success Rate:** Expected to be below 10% for automated measurements in Q1 processing

<figure class="dataset-figure">
<img src="../../images/euclid/Euclid_Q1.webp" alt="Euclid Quick Data Release 1 Angular Density Map">
<figcaption>Source image: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/euclid_q1')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/euclid_q1/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 29,767,806     | 472               | 85                  | 23 GiB       |

<div class="button-container">
<a href="https://www.cosmos.esa.int/en/web/euclid/euclid-q1-data-release" class="button-link">Official Release</a>
<a href="https://euclid.esac.esa.int/dr/q1/dpdd/merdpd/dpcards/mer_finalcatalog.html#detailed-description-of-the-data-product" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250315302E/abstract" class="button-link">Research Paper</a>
</div>
