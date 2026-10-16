# Produtos FITS do LSST DP2

O **Legacy Survey of Space and Time Data Preview 2 (LSST DP2)** reúne produtos de imagens e catálogos gerados pelo Rubin Science Pipelines v30.0.8 a partir de observações da LSSTCam obtidas entre abril de 2025 e janeiro de 2026. O Early DP2 foi lançado em 27 de julho de 2026. Nesta fase, o produto de imagem publicado é o deep coadd. Imagens de visita e de diferença entram no lançamento completo, previsto para outubro–dezembro de 2026.

- [Documentação oficial do DP2](https://dp2.lsst.io/)
- [Produtos de dados do DP2](https://dp2.lsst.io/products/index.html)
- [Citação oficial do dataset](https://doi.org/10.71929/rubin/3382528)

## Nível de acesso

!!! private "Acesso restrito"
    O DP2 é proprietário e está disponível somente para detentores de direitos de dados do Rubin, conforme a [política de dados](https://rubinobservatory.org/for-scientists/data-products/data-policy) e o documento [RDO-013](https://docushare.lsst.org/docushare/dsweb/Get/RDO-013).

## Produtos disponíveis no LIneA

!!! info "Inventário local"
    As quantidades apresentadas nesta página documentam os arquivos disponíveis na infraestrutura do LIneA.

## Cobertura do céu por banda

Os deep coadds cobrem cerca de 3.000 graus quadrados nas regiões Wide-Fast-Deep, Small Field Survey e Deep Drilling Fields. Visitas individuais cobrem cerca de 15.000 graus quadrados, mas essas imagens não fazem parte desta cópia.

A cópia local reúne 197.105 patches em 2.191 tracts, com identificadores entre 2054 e 13041. A declinação desses patches vai de −52,16° a +22,90°, e a ascensão reta percorre o círculo completo. Nem todo patch existe em todas as bandas; a tabela abaixo traz a contagem por filtro.

!!! info "Como interpretar a cobertura"
    Cada arquivo é um patch do skymap. Os deep coadds incluem somente exposições que atendem aos critérios de qualidade; patches de borda podem ter regiões sem dados, identificadas pela máscara `NO_DATA`.

Fontes oficiais: [documentação do DP2](https://dp2.lsst.io/), [deep coadd](https://dp2.lsst.io/products/images/deep_coadd.html) e [coadição de imagens](https://dp2.lsst.io/processing/coaddition/index.html).

### Deep coadd

Combinação, por banda e patch, de exposições calibradas e com background subtraído. O empilhamento é uma coadição por células, com média ponderada pelo inverso da variância. Cada arquivo é um `CellCoadd` em uma das seis bandas `u`, `g`, `r`, `i`, `z` e `y`.

- **Formato:** FITS (`.fits`)
- **Inventário local:** 925.460 arquivos, 27,71 TB
- **Conteúdo:** planos de imagem (nJy), variância (nJy²) e máscara, além de PSF, calibração fotométrica e WCS
- **Documentação oficial:** [Deep coadd](https://dp2.lsst.io/products/images/deep_coadd.html) e [coadição de imagens](https://dp2.lsst.io/processing/coaddition/index.html)

| Banda | Arquivos | Tracts | Tamanho |
|---|---:|---:|---:|
| u | 114.892 | 1.405 | 3,31 TB |
| g | 155.115 | 1.799 | 4,57 TB |
| r | 171.856 | 1.999 | 5,20 TB |
| i | 177.588 | 2.030 | 5,41 TB |
| z | 166.412 | 1.884 | 5,07 TB |
| y | 139.597 | 1.590 | 4,16 TB |

A coluna Tracts conta tracts distintos naquela banda. A união das seis bandas tem 2.191 tracts.

## Limites deste inventário

Esta página descreve somente os deep coadds da cópia local do LIneA. Não há, neste conjunto, `deep_coadd_background`, `deep_coadd_n_image` nem mapas HealSparse. O Early DP2 oficial também restringe os produtos de imagem aos deep coadds. Raw exposures, visit images, template coadds e difference images não estão registrados como disponíveis nessa cópia. Consulte o [índice de produtos do DP2](https://dp2.lsst.io/products/index.html).
