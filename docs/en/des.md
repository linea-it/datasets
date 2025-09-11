
# Dark Energy Survey Data Release 2

The Dark Energy Survey Data Release 2 (DES DR2) is a comprehensive catalog performed with DECam. Published in January 2021, DES DR2 includes data collected from six years of observations, covering about 5,000 square degrees of the southern sky. This release provides highly detailed and precise information on over 690 million astronomical objects, including stars, galaxies, and quasars.

## Load using LSDB

```bash
>> lsdb.read_hats('https://web.archive.org/web/20250325105440/https://data.lsdb.io/hats/des/des_dr2')
```

## Download with wget

```bash
$ wget -r -np -nH --cut-dirs=6 -R "*.html" https://web.archive.org/web/20250325105440/https://data.lsdb.io/hats/des/des_dr2/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 691,483,608    | 218               | 1,582               | 769 GB       |

## References

[OFFICIAL RELEASE] [COLUMN DESCRIPTIONS] [RESEARCH PAPER]
```
10:54
```markdown
# Dark Energy Survey Y6 Gold

The Y6 Gold catalog is derived from Dark Energy Survey Data Release 2 (DES DR2) and includes all six years of g,r,i,z,Y imaging measurements. Y6 Gold was formatted for the DES final cosmological analyses, but it has very general applicability. Y6 Gold contains 669 million objects to i-band of 23.4 (S/N = 10 for extended objects).

## Load using LSDB

>> lsdb.read_hats('https://web.archive.org/web/20250325105440/https://data.lsdb.io/hats/des/des_y6_gold')

## Download with wget

```bash
$ wget -r -np -nH --cut-dirs=6 -R "*.html" https://web.archive.org/web/20250325105440/https://data.lsdb.io/hats/des/des_y6_gold/
```

## Catalog metadata

| Number of rows | Number of columns | Number of partitions | Size on disk |
|----------------|-------------------|---------------------|--------------|
| 691,483,608    | 336               | 1,582               | 1.3 TiB      |

## References

[OFFICIAL RELEASE] [COLUMN DESCRIPTIONS] [RESEARCH PAPER]