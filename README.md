# LIneA Datasets Documentation

This repository contains the documentation for LIneA's datasets and services, built with MkDocs and Material theme. The documentation is available in multiple languages (English, Portuguese, and Spanish).

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

## Setup and Development

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd datasets
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   
   On Linux/macOS:
   ```bash
   source venv/bin/activate
   ```
   
   On Windows:
   ```bash
   venv\Scripts\activate
   ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Development

### Development Commands
```bash
# Start local development server with live reload
mkdocs serve

# The documentation will be available at http://127.0.0.1:8000
# Changes to source files will automatically reload the browser
```

### Testing Builds
```bash
# Test build with strict mode to catch all issues
mkdocs build --strict

# The built site will be in the site/ directory
# Use this command to verify your documentation builds correctly before deployment
```

## Production Deployment

For production deployment, use:
```bash
mkdocs gh-deploy
```

