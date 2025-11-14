# Cómo acceder al Rubin DP1 en LIneA

Esta guía presenta un paso a paso claro para acceder al Rubin Data Preview 1 (DP1) utilizando la infraestructura del LIneA, incluyendo el entorno HPC y la plataforma Open OnDemand. Todos los enlaces a continuación forman parte de la documentación oficial del LIneA.

---

## Pasos para el acceso

### 1) Registrarse como usuario de LIneA  
Siga las instrucciones de registro y complete el proceso:  
https://docs.linea.org.br/es/primeiros_passos.html

### 2) Solicitar acceso al entorno HPC de LIneA  
Abra un ticket en el Helpdesk solicitando acceso al HPC, **indicando específicamente su interés en utilizar Open OnDemand**:  
https://docs.linea.org.br/es/suporte.html

### 3) Acceder a la plataforma Open OnDemand  
Una vez aprobado el acceso, siga la guía para ingresar:  
https://docs.linea.org.br/es/processamento/uso/openondemand.html

### 4) Crear un entorno Conda y exponer el kernel en Open OnDemand  
El procedimiento completo está documentado aquí:  
https://docs.linea.org.br/es/processamento/uso/openondemand.html#creando-kernels-python

Dentro de su entorno Conda, instale LSDB, Dask y Dask-Jobqueue:

```bash
conda install -c conda-forge lsdb dask dask-jobqueue distributed
```

### 5) Iniciar una sesión de Jupyter Lab  
Inicie una sesión siguiendo la documentación oficial:  
https://docs.linea.org.br/es/processamento/uso/openondemand.html#jupyterlab

### 6) Abrir un notebook y seleccionar el kernel creado  
Después de abrir Jupyter Lab, seleccione el kernel correspondiente a su entorno Conda.

---

## Configuración de un clúster Dask

El ejemplo siguiente incluye dos opciones: un clúster local para pruebas y un clúster SLURM para cargas de trabajo reales en el sistema HPC.

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

## Leyendo el catálogo Rubin DP1 usando LSDB

Puede abrir el catálogo Rubin DP1 directamente utilizando la variable de entorno global `DP1_CATALOGS`, que debe apuntar al directorio base que contiene las colecciones del DP1. Luego, simplemente use LSDB para cargar el catálogo.

```python
import os
import lsdb

dp1_base = os.environ.get("DP1_CATALOGS")

catalog_path = os.path.join(dp1_base, "object_collection")

cat = lsdb.open_catalog(catalog_path)
```
