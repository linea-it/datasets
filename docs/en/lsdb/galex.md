# GALEX Merged Catalog of Sources

The GALEX Merged Catalog of Sources (MCAT) is the primary source catalog from the Galaxy Evolution Explorer (GALEX) mission, a NASA Small Explorer that operated between 2003 and 2012. The telescope conducted sky surveys in two ultraviolet bands: far-UV (FUV, ~1350–1750 Å) and near-UV (NUV, ~1750–2800 Å).

The MCAT combines detections from multiple individual observations (visits) to generate a consolidated list of unique sources, providing UV photometry and basic properties for hundreds of millions of objects. It covers different survey depths, from the shallow All-Sky Imaging Survey (AIS, covering ~26,000 deg²) to the deep Deep Imaging Survey (DIS, with exposures of tens of thousands of seconds).


<figure class="dataset-figure">
<img src="../../images/galex/point_density.webp" alt="GALEX MCAT Catalog">
<figcaption>Image source: https://data.lsdb.io</figcaption>
</figure>


---

## Loading with LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/galex')
```

---

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/galex/
```

---

## Catalog Metadata

| Number of rows | Number of columns | Number of partitions | Disk size | Builder Version               |
| ---------------- | ----------------- | ------------------- | ---------------- |---------------------------------|
| 292,296,119      | 368               | 1,595               | 343.7 GiB        | hats-import v0.9.2, hats v0.9.2 | 


<div class="button-container">
<a href="https://archive.stsci.edu/missions-and-data/galex" class="button-link">Official Release</a>
<a href="https://www.galex.caltech.edu/wiki/Public:Documentation/Appendix_A.1" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2017ApJS..230...24B/abstract" class="button-link">Scientific Paper</a>
</div>

