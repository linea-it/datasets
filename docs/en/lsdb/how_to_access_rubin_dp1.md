# How to Access Rubin DP1 at LIneA

This guide provides a clear step-by-step workflow for accessing the Rubin Data Preview 1 (DP1) using the LIneA infrastructure, including the HPC environment and the Open OnDemand platform. All links below refer to the official LIneA documentation.

---

## Step-by-step instructions

### 1) Register as a LIneA user  
Follow the onboarding instructions and complete your registration:  
https://docs.linea.org.br/en/primeiros_passos.html

### 2) Request access to the LIneA HPC environment  
Open a ticket on the Helpdesk requesting HPC access, **specifically stating your interest in using Open OnDemand**:  
https://docs.linea.org.br/en/suporte.html

### 3) Access the Open OnDemand platform  
Once access is granted, follow the guide to log in:  
https://docs.linea.org.br/en/processamento/uso/openondemand.html

### 4) Create a Conda environment and expose the kernel to Open OnDemand  
Full instructions are available here:  
https://docs.linea.org.br/en/processamento/uso/openondemand.html#creating-python-kernels

Inside your Conda environment, install LSDB, Dask, and Dask-Jobqueue:

```bash
conda install -c conda-forge lsdb dask dask-jobqueue distributed
```

### 5) Start a Jupyter Lab session  
Launch a session following the official documentation:  
https://docs.linea.org.br/en/processamento/uso/openondemand.html#jupyterlab

### 6) Open a notebook and select your custom Conda kernel  
Once Jupyter Lab is open, select the kernel corresponding to your Conda environment.

---

## Configuring a Dask cluster

The example below includes two options: a local cluster for testing and a SLURM cluster for real workloads on the HPC system.

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

## Reading the Rubin DP1 catalog using LSDB

You can open the Rubin DP1 catalog directly using the global environment variable `DP1_CATALOGS`, which should point to the base directory containing the DP1 collections. Then, simply use LSDB to load the catalog.

```python
import os
import lsdb

dp1_base = os.environ.get("DP1_CATALOGS")

catalog_path = os.path.join(dp1_base, "object_collection")

cat = lsdb.open_catalog(catalog_path)
```
