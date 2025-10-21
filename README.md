# LIneA Datasets Documentation

This repository contains the documentation for LIneA's datasets and services, built with **MkDocs** and the **Material** theme.  
The documentation is available in multiple languages (English, Portuguese, and Spanish).

## Types of Datasets

LIneA provides access to three different types of datasets:

### LSDB Datasets
- **Source**: Data from [data.lsdb.io](https://data.lsdb.io)
- **Description**: Large-scale astronomical catalogs and datasets managed through the LSDB (Large Survey Database) system  
- **Access**: Web-based interface and API access

### LIneA Databases
- **Source**: Databases hosted directly by LIneA  
- **Description**: Curated datasets and databases maintained by LIneA's infrastructure  
- **Access**: Direct database connections and specialized interfaces

### HPC Datasets
- **Source**: Datasets accessible via High Performance Computing (HPC) systems  
- **Description**: Large-scale datasets requiring computational resources for processing and analysis  
- **Access**: HPC cluster access and specialized computational workflows

---

## Setup and Development

### Prerequisites

- **Conda** (Miniconda or Anaconda) installed

> If you don’t have Conda installed yet:
> 
> **Linux/macOS**
> ```bash
> # Install Miniconda (recommended)
> cd ~/Downloads
> curl -L -O https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
> chmod +x Miniconda3-latest-Linux-x86_64.sh
> ./Miniconda3-latest-Linux-x86_64.sh -b -p "$HOME/miniconda"
> source "$HOME/miniconda/bin/activate"
> ```
>
> **Windows:**
> Download and install [Miniconda](https://docs.anaconda.com/miniconda/) using the graphical installer.
>
> **Note:**  
> This project uses a pinned `environment.yml` file to ensure version consistency across all dependencies.

---

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd datasets
   ```

2. **Create the Conda environment from the YAML file**
   ```bash
   conda env create -f environment.yml
   ```

3. **Activate the environment**
   ```bash
   conda activate datasets
   ```

4. **Verify installation**
   ```bash
   mkdocs --version
   ```

---

## Development

### Development Commands

```bash
# Start local development server with live reload
mkdocs serve

# The documentation will be available at http://127.0.0.1:8000
# Changes to source files will automatically reload the browser
```

---

### Testing Builds

```bash
# Test build with strict mode to catch all issues
mkdocs build --strict

# The built site will be in the site/ directory
# Use this command to verify your documentation builds correctly before deployment
```

---

## Production Deployment

For production deployment, use:
```bash
mkdocs gh-deploy
```

This will build the site and push it to the `gh-pages` branch automatically.
