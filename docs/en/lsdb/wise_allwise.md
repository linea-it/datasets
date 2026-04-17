# AllWISE

!!! Warning "Warning"
    Page under construction. 


## Load using LSDB

```python
>>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/wise/allwise/')
```

## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/wise/allwise/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|-----------------|-------------------|----------------------|-----------------|
| 747,634,026      | 299              |	768                  |	258.0 GiB   |


<div class="button-container">
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/" class="button-link">Official Release</a>
<a href="https://wise2.ipac.caltech.edu/docs/release/allwise/expsup/sec2_1a.html" class="button-link">Column Descriptions</a>
<a href="https://ui.adsabs.harvard.edu/abs/2010AJ....140.1868W/abstract" class="button-link">Research Paper</a>
</div>
