# Pan-STARRS1 (detection)


!!! Warning "Warning"
    Page under construction. 


## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/panstarrs/ps1_detection/')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/panstarrs/ps1_detection/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|-----------------|-------------------|----------------------|-----------------|
| 73,951,333,592   | 61                | 83,004              | 20.8 TiB         |  

<div class="button-container">
<a href="https://outerspace.stsci.edu/display/PANSTARRS/" class="button-link">Official Release</a>
<a href="https://outerspace.stsci.edu/display/PANSTARRS/PS1+Database+object+and+detection+tables" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2016arXiv161205560C/abstract" class="button-link">Research Paper</a>
</div>
