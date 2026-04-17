# Sloan Digital Sky Survey Data Release 7 (spectra)


!!! Warning "Warning"
    Page under construction. 




## Load using LSDB

```bash
>> lsdb.open_catalog('https://linea.data.lsdb.io/hats/sdss_dr7_spectra')
```


## Download with wget

```bash
$ wget -e robots=off -r -np -nH --cut-dirs=1 -c -R "index.html*" -l 0 https://linea.data.lsdb.io/hats/sdss_dr7_spectra/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 1,640,953        | 23              | 1,304               | 86.2 GiB         |

<div class="button-container">
<a href="https://classic.sdss.org/dr7" class="button-link">Official Release</a>
<a href="https://ui.adsabs.harvard.edu/abs/2009ApJS..182..543A/abstract" class="button-link">Research Paper</a>
</div>

