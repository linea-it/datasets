# LIneA Datasets Documentation

This repository contains the documentation for LIneA's datasets and services, built with MkDocs and Material theme. The documentation is available in multiple languages (English, Portuguese, and Spanish).

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

## Development vs Production

### Development Environment
**Purpose**: Local development, testing, and content creation

**Setup**: Follow the installation steps above, then use development commands for local work.

**Development Commands**:
```bash
# Start local development server with live reload
mkdocs serve

# The documentation will be available at http://127.0.0.1:8000
# Changes to source files will automatically reload the browser
```

### Production Environment
**Purpose**: Deploying the documentation to live servers (GitHub Pages, web servers, etc.)

**Production Build**:
```bash
# Build static site for production deployment
mkdocs build

# The built site will be in the site/ directory
# This creates optimized, static HTML files ready for web servers
```

**Production Deployment Options**:

1. **GitHub Pages** (automated deployment):
   ```bash
   mkdocs gh-deploy
   ```
   This builds the site and pushes it to the `gh-pages` branch for GitHub Pages hosting.

2. **Manual Deployment** (for other web servers):
   ```bash
   mkdocs build
   # Then upload the contents of the site/ directory to your web server
   ```

3. **CI/CD Pipeline** (for automated builds):
   Use the `mkdocs build` command in your CI/CD pipeline to generate the site automatically.

## LSDB Information

This website serves as a user interface for the LSDB.io service hosted at LIneA's datacenter. 

LSDB software is developed and maintained by LINCC frameworks.

### LSDB Documentation 

Check out their [ReadTheDocs site](https://docs.lsdb.io)
for more information on partitioning, installation, and contributing.
The scientific publication associated is ["Using LSDB to enable large-scale catalog distribution, cross-matching, and analytics"](https://ui.adsabs.harvard.edu/abs/2025arXiv250102103C).
