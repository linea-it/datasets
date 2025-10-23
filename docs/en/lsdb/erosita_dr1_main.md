# eROSITA-DE DR1 Main

The eROSITA telescope array aboard the Spektrum Roentgen Gamma (SRG) satellite began surveying the sky in December 2019. Data Release 1 (DR1) presents X-ray catalogues, calibrated event files, source products, and all-sky maps from the first eROSITA All-Sky Survey (eRASS1), which spanned six months of operations from December 2019 to June 2020. This release comprises data covering the western Galactic hemisphere, the half-sky proprietary to the German eROSITA Consortium (eROSITA-DE).

The DR1 data is organized into 2447 sky tiles and provides source catalogues in two primary X-ray bands: a main catalogue from the most sensitive 0.2–2.3 keV energy range, and a hard catalogue from the 2.3–5.0 keV band.

The resultant eRASS1 main catalogue (0.2–2.3 keV) contains 930,203 entries (903,521 point-like and 26,682 extended sources) selected with a detection likelihood DET_LIKE_0 ≥ 6 (or EXT_LIKE > 0). A smaller catalogue of 5,466 sources is presented from the hard (2.3–5.0 keV) band, selected with DET_LIKE_3 ≥ 12. This eRASS1 main catalogue increases the number of known X-ray sources in the published literature by more than 60%.

Key performance metrics and survey characteristics include:

* **Median Survey PSF HEW (0.2–2.3 keV):** 30.0"
* **Median Survey PSF HEW (2.3–5.0 keV):** 34.4"
* **Flux Limit (0.5–2 keV, 50% completeness):** F(0.5–2 keV) > 5 × 10⁻¹⁴ erg s⁻¹ cm⁻²
* **Absolute Flux Accuracy (0.5–2 keV):** ~6% systematic uncertainty (relative to XMM-Newton)
* **Astrometric Systematic Uncertainty:** σ₀ = 0.9" ± 0.1" (based on Gaia/unWISE QSO cross-matching)
* **Spurious Source Fraction (Main Cat.):** ~14% (for DET_LIKE_0 ≥ 6)
* **Spurious Source Fraction (Hard Cat.):** ~8–10% (for DET_LIKE_3 ≥ 12)
* **Resolved CXB Fraction (1–2 keV):** ~19% (median value at the uniform flux limit)


<figure class="dataset-figure">
<img src="../../images/erosita/eROSITA_DR1_Main.webp" alt="eROSITA-DE DR1 Main Angular Density Map">
<figcaption>Source image: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/erosita')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/erosita/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 930,203        | 255               | 10                  | 994 MB       |

<div class="button-container">
<a href="https://erosita.mpe.mpg.de/dr1" class="button-link">Official Release</a>
<a href="https://erosita.mpe.mpg.de/dr1/AllSkySurveyData_dr1/Catalogues_dr1/MerloniA_DR1/eRASS1_Main.html" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2024A%26A...682A..34M" class="button-link">Research Paper</a>
</div>
