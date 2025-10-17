# Dark Energy Spectroscopic Instrument Data Release 1

The Dark Energy Spectroscopic Instrument (DESI) Data Release 1 (DR1) presents spectroscopic data from the first 13 months of the DESI main survey (2021 May 14 through 2022 June 13), together with a uniform reprocessing of all Survey Validation (SV) data. DESI is a highly multiplexed spectrograph mounted on the Mayall 4-meter telescope at Kitt Peak National Observatory, capable of simultaneously observing 5000 targets across an 8 deg² field-of-view using robotic fiber positioning.

DR1 comprises observations across 14,000 deg² of the northern and southern Galactic caps in optical wavelengths (3600-9800 Å) spanning five broad classes of targets: Milky Way Survey (MWS) stars, Bright Galaxy Survey (BGS) galaxies (0<z<0.6), luminous red galaxies (LRGs, 0.4<z<1.1), emission-line galaxies (ELGs, 0.6<z<1.6), and quasars (QSOs, 0.9<z<4). The primary spectroscopic production for DR1 is Iron, processed using improved calibration algorithms and updated QSO templates compared to the earlier EDR release.

The resultant DR1 catalog contains high-confidence redshifts for 18.7 million unique objects across all surveys and programs, making DR1 the largest extragalactic spectroscopic redshift survey ever conducted—nearly four times larger than all previous SDSS programs combined. The main survey includes 8.5 million, 9.0 million, and 1.2 million objects from the bright, dark, and backup programs, respectively. After applying quality criteria (ZWARN=0), the sample comprises 13.1 million galaxies, 1.6 million quasars, and 4 million stars.

Key performance metrics and survey characteristics include:

* **Spectroscopic Coverage**: 9739 deg² (bright program), 9528 deg² (dark program), 2726 deg² (backup program)
* **Survey Completeness** (at end of DR1 period): 41.3% (bright), 29.0% (dark), 5.2% (backup)
* **Wavelength Precision**: 0.025 Å
* **Spectrophotometric Calibration**: 6-10% systematic uncertainty
* **Redshift Precision**: 10 km s⁻¹ (BGS, ELG), 50 km s⁻¹ (LRG), 20-125 km s⁻¹ (QSO)
* **Redshift Outlier Rate**: ≤0.3% (BGS, LRG, ELG), 0.7% (QSO z<2.1), 1.8% (QSO z>2.1)
* **Radial Velocity Precision** (MWS): ≲10 km s⁻¹
* **Sky Subtraction Residuals**: <1% systematic
* **Instrumental Resolution**: λ/Δλ = 2000-5200 (wavelength dependent)

<figure class="dataset-figure">
<img src="../../images/desi/DESI_DR1_zcat.webp" alt="Dark Energy Spectroscopic Instrument DR1 z-catalog Angular Density Map">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>

## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/desi/desi_dr1_zcat')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=2 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/desi/desi_dr1_zcat/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 28,425,963     | 136               | 75                  | 12 GiB       |

<div class="button-container">
<a href="https://data.desi.lbl.gov/doc/releases/dr1" class="button-link">Official Release</a>
<a href="https://desidatamodel.readthedocs.io/en/latest/column_descriptions.html" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250314745D" class="button-link">Research Paper</a>
</div>

## Acknowledgments

The research used data from DESI. DESI construction and operations are managed by the Lawrence Berkeley National Laboratory. Work supported by the U.S. Department of Energy, Office of Science, Office of High-Energy Physics (Contract No. DE-AC02-05CH11231), and the National Energy Research Scientific Computing Center.

Additional support from:

- U.S. National Science Foundation (NSF), Division of Astronomical Sciences (Contract No. AST-0950945)
- NSF's National Optical-Infrared Astronomy Research Laboratory
- Science and Technology Facilities Council of the United Kingdom
- Gordon and Betty Moore Foundation
- Heising-Simons Foundation
- French Alternative Energies and Atomic Energy Commission (CEA)
- National Council of Humanities, Science and Technology of Mexico (CONAHCYT)
- Ministry of Science and Innovation of Spain (MICINN)
- DESI Member Institutions (www.desi.lbl.gov/collaborating-institutions)

The DESI collaboration is permitted to conduct scientific research on I'oligam Du'ag (Kitt Peak), a mountain significant to the Tohono O'odham Nation.

Opinions, findings, and conclusions are those of the author(s) and do not necessarily reflect the views of the U.S. National Science Foundation, U.S. Department of Energy, or listed funding agencies.
