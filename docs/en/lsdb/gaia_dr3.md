# Gaia Data Release 3

Gaia Data Release 3 (DR3) presents a major update to the data from the European Space Agency’s Gaia mission, significantly expanding upon the Early Third Data Release (Gaia EDR3). While repeating the astrometry (positions, parallaxes, proper motions) and broadband photometry (G, GBP, GRP) for approximately 1.8 billion sources from Gaia EDR3, Gaia DR3 introduces a wealth of new astrophysical information derived from the first 34 months of mission data. This release constitutes the largest collection to date of all-sky spectrophotometry, radial velocities, variability information, and astrophysical parameters.

The Gaia DR3 catalogue incorporates data from Gaia’s astrometric instrument (G-band: 330–1050 nm), the BP/RP photometers (providing low-resolution spectra covering 330–680 nm and 640–1050 nm, respectively), and the Radial Velocity Spectrometer (RVS, covering 846–870 nm). The source list remains identical to Gaia EDR3.

The catalogue provides new mean radial velocities for over 33 million objects, mean BP/RP spectra for about 220 million sources, and mean RVS spectra for roughly 1 million sources. Analysis of epoch photometry yields classifications and parameters for around 10 million variable sources across 24 types. Astrophysical parameters are provided for approximately 470 million sources, with object class probabilities for about 1.5 billion sources. Additionally, orbital solutions or trend parameters are available for around 800,000 non-single stars, and data for more than 150,000 Solar System objects are included.

Key performance metrics and survey characteristics include:

* **Observation Period:** 34 months
* **Astrometric Reference Frame:** Gaia-CRF3 (aligned with ICRF3 to ~0.01 mas RMS at J2016.0)
* **Global Parallax Bias:** –17 µas
* **BP/RP Spectral Resolution (R = λ/Δλ):** ~30–100 (BP), ~70–100 (RP)
* **RVS Spectral Resolution (R = λ/Δλ):** ~11,500
* **RVS Wavelength Range (processed):** 846–870 nm
* **Radial Velocity Magnitude Limit:** GRVS < 14
* **Radial Velocity Temperature Range:** 3100 ≤ Teff ≤ 14,500 K
* **Mean BP/RP Spectra Magnitude Limit:** Primarily G < 17.65

<figure class="dataset-figure">
<img src="../../images/gaia/Gaia_DR3.webp" alt="Gaia Data Release 3 Angular Density Map">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/gaia_dr3')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/gaia_dr3/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 1,812,731,847  | 152               | 2,016               | 1.1 TiB      |

<div class="button-container">
<a href="https://www.cosmos.esa.int/web/gaia/dr3" class="button-link">Official Release</a>
<a href="https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_main_source_catalogue/ssec_dm_gaia_source.html" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220800211G/abstract" class="button-link">Research Paper</a>
</div>
