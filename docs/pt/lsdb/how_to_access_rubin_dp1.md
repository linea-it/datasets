# Como acessar o Rubin DP1 no LIneA

Este guia apresenta um passo a passo simples para acessar o Rubin Data Preview 1 (DP1) usando a infraestrutura do LIneA, incluindo o uso do ambiente HPC e da plataforma Open OnDemand. Todos os links indicados abaixo fazem parte do fluxo oficial de uso do ecossistema do LIneA.

---

## Passo a passo para acesso

### 1) Registrar-se como usuário do LIneA  
Acesse o guia oficial de primeiros passos e complete o registro:  
https://docs.linea.org.br/primeiros_passos.html

### 2) Solicitar acesso ao ambiente HPC do LIneA  
Abra um ticket no Helpdesk informando que deseja acesso ao HPC **com interesse específico em utilizar o Open OnDemand**:  
https://docs.linea.org.br/suporte.html

### 3) Acessar a plataforma Open OnDemand  
Após liberação, entre na plataforma seguindo o guia:  
https://docs.linea.org.br/processamento/uso/openondemand.html

### 4) Criar um ambiente Conda e disponibilizar o kernel no Open OnDemand  
O processo completo está documentado aqui:  
https://docs.linea.org.br/processamento/uso/openondemand.html#criando-kernels-python

No ambiente Conda criado, instale o LSDB, o Dask e o Dask-Jobqueue:

```bash
conda install -c conda-forge lsdb dask dask-jobqueue distributed
```

### 5) Iniciar uma sessão no Jupyter Lab  
Abra uma sessão seguindo as instruções:  
https://docs.linea.org.br/processamento/uso/openondemand.html#jupyterlab

### 6) Abrir um notebook e selecionar o kernel criado  
Após iniciar o Jupyter Lab, escolha o kernel correspondente ao seu ambiente Conda.

---

## Configurando um cluster Dask

O exemplo abaixo mostra duas opções: cluster local para testes e cluster SLURM para rodar workloads reais no HPC.

```python
from dask.distributed import Client

CLUSTER_TYPE = "slurm"

if CLUSTER_TYPE == "local":
    from dask.distributed import LocalCluster
    
    cluster = LocalCluster(
        n_workers=3,
        threads_per_worker=1,
        memory_limit="2GB"
    )
    
    client = Client(cluster)

if CLUSTER_TYPE == "slurm":
    from dask_jobqueue import SLURMCluster

    minimum_jobs = 5
    maximum_jobs = 10
    
    cluster = SLURMCluster(
        n_workers=minimum_jobs,
        queue="cpu",
        account="hpc-bpglsst",
        cores=8,
        memory="16GB",
        processes=1,
        interface="ib0",
        walltime="01:00:00",
        job_extra_directives=[
            "--propagate"
        ]
    )
    
    cluster.adapt(minimum_jobs=minimum_jobs, maximum_jobs=maximum_jobs)

    client = Client(cluster)

    client.wait_for_workers(minimum_jobs, timeout=15)
```

---

## Lendo o catálogo Rubin DP1 com LSDB

Após configurar o ambiente e o cluster, você pode abrir o catálogo usando:

```python
import lsdb

cat = lsdb.open_catalog("path/to/collection")
```

Substitua `"path/to/collection"` pelo caminho disponibilizado na sua área de trabalho do HPC conforme a organização do dataset DP1.
