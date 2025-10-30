# DES Y6 Gold WaZP Cluster Catalogs

!!! Warning "Warning"
    Page under construction. Some content may be incomplete or out of date.



## Overview
Benoist et al. (2025) present a galaxy cluster catalog from the WaZP cluster finder, independent of red-sequence detection, using six years of Dark Energy Survey data (DES-Y6). The full catalog includes over 400,000 clusters with Ngals > 5, reaching redshifts up to z = 1.3. A homogenized version for cosmology contains 33,000 rich clusters (Ngals > 25).

Comparison with the previous DES-Y1 WaZP catalog shows nearly all clusters within the overlapping footprint and depth are recovered. Deeper DES-Y6 observations and a more complete spectroscopic redshift sample improve redshift estimates, with an average scatter of 1.4% and a mean offset of 0.2%.

Optical clusters are cross-matched with SZE clusters from SPT and ACT. Nearly all SZE clusters in overlapping regions have a WaZP counterpart, and 90% of optical clusters with richness > 150 match SZE detections in deep survey areas. About 15–20% of SZE-matched systems have multiple WaZP counterparts within R500c at the same redshift, indicating possible interacting or unrelaxed systems. WaZP and SZE cluster centers are consistent when accounting for beam sizes.


## Data Access


- Cluster catalog: [y6a2_dnf_wazp_v5.0.12.6801_clusters.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits)
- Cluster members: [y6a2_dnf_wazp_v5.0.12.6801_members.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits)
- Footprint map: [y6a2_dnf_wazp_v5.0.12.6801_footprint.fits](https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits)


### Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_clusters.fits
```


```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_members.fits
```

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://datasets.linea.org.br/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fitshttps://datasets/wazp/y6a2_dnf_wazp_v5.0.12.6801_footprint.fits
```


<div class="button-container">
<a href="https://des.ncsa.illinois.edu/releases/y6a2/Y6cluster-wazp" class="button-link">Column Descriptions</a>
<a href="https://arxiv.org/abs/2507.05360t" class="button-link">Research Paper</a>
</div>
