# LSST - Data Preview 1 (DP1)

## Sobre

O LSST DP1 foi o primeiro conjunto de dados preliminar baseado em dados reais liberado internamente pelo LSST DM. Ele contém produtos de imagens e catálogos resultantes do processamento realizado com o LSST Science Pipelines v29, a partir de observações obtidas com a Câmera de Comissionamento do LSST em sete campos de aproximadamente 1 grau quadrado, ao longo de sete semanas no final de 2024.

**Data de lançamento:** 30 de junho de 2022

<div class="button-container">

<a href="[https://dp1.lsst.io/](https://dp1.lsst.io/)" class="button-link">Página de documentação do DP1</a>

<a href="[https://doi.org/10.71929/rubin/2570308](https://doi.org/10.71929/rubin/2570308)" class="button-link">Informações para citação</a>

</div>

## Elegibilidade

Dados privados disponíveis apenas para membros da colaboração LSST: todos os cientistas e estudantes nos EUA e no Chile, além dos membros nomeados das [equipes internacionais de contribuição em espécie](www\.lsst.org/scientists/international-drh-list). Para mais informações, consulte o documento de política de dados [RDO-013](https://docushare.lsst.org/docushare/dsweb/Get/RDO-013).

## Como acessar

Os produtos de dados hospedados e mantidos pelo LIneA estão disponíveis por meio de diferentes métodos de acesso. Esta página apresenta informações sobre como acessar os produtos de dados primários e secundários para uso no **ambiente HPC**. Eles podem ser acessados pela plataforma [Open OnDemand](https://ondemand.linea.org.br/) do LIneA, tanto pelo ambiente JupyterLab (no menu Interactive Apps) quanto pelo Shell Access Terminal (no menu Clusters).

### Localização dos arquivos

Os produtos de dados são armazenados nos sistemas de arquivos Lustre e NFS, dependendo do tipo de arquivo. Em ambos os casos, os diretórios podem ser acessados por meio das variáveis de ambiente `$DATA` e `$PUBLIC_DATA`, para dados sob embargo e dados públicos, respectivamente.

### Estrutura de diretórios

Os produtos de dados do LSST DP1 estão organizados na seguinte estrutura de diretórios:


```
$DATA/lsst/dp1/
    ├── primary
    │   ├── catalogs
    │   │   ├── object
    │   │   │   └── object_xxxxx_...xxx.parq # (29 files)
    │   │   ├── ss_object
    │   │   │   └──  ss_object_...xxx.parq
    │   │   └── ss_source
    │   │       └── ss_source_...xxx.parq
    │   ├── images
    │   └── maps
    └── secondary
        ├── catalogs
        │   ├── hips  # (HiPS catalog structure)
        │   └── object_collection # (LSDB HATS structure)
        └── images
            └── hips # (HiPS image structure)
```

Os conjuntos de dados *\_primary\_* são produtos de dados originais fornecidos pelo LSST DM e transferidos para o IDAC-BR, enquanto os conjuntos de dados *\_secondary\_* são produtos de dados derivados gerados pela equipe do LIneA.

## Informações sobre os conjuntos de dados

### Object

Medições de objetos detectados em imagens de coadição profunda.

Caminho: `$DATA/lsst/dp1/primary/catalogs/object/`

| Números principais |   |
|---|---|
| Número de arquivos | 29 |
| Número de colunas | 1.296 |
| Número total de linhas | 2.299.757 |
| Tamanho total | 6,3 GB |
| Formato do arquivo (extensão) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#Object](https://sdm-schemas.lsst.io/dp1.html#Object)" class="button-link">Schema do catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>

### SS Object

Parâmetros derivados para objetos em movimento (do Sistema Solar).

Caminho: `$DATA/lsst/dp1/primary/catalogs/ss_object/`

| Números principais |   |
|---|---|
| Número de arquivos | 1 |
| Número de colunas | 3 |
| Número total de linhas | 431 |
| Tamanho total | 300 KB |
| Formato do arquivo (extensão) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#SSObject](https://sdm-schemas.lsst.io/dp1.html#SSObject)" class="button-link">Schema do catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>

### SS Source

Parâmetros físicos instantâneos para objetos em movimento no momento de cada observação.

Caminho: `$DATA/lsst/dp1/primary/catalogs/ss_source/`

| Números principais |   |
|---|---|
| Número de arquivos | 1 |
| Número de colunas | 23 |
| Número total de linhas | 5.988 |
| Tamanho total | 1,5 MB |
| Formato do arquivo (extensão) | Parquet (`.parq`) |

<div class="button-container">

<a href="[https://sdm-schemas.lsst.io/dp1.html#SSSource](https://sdm-schemas.lsst.io/dp1.html#SSSource)" class="button-link">Schema do catálogo</a>

<a href="../../en/hpc/rubin_dp1_qa.html" class="button-link">Notebook de QA</a>

</div>