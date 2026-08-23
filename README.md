# VietHeritageLOD

VietHeritageLOD is a Linked Open Data knowledge graph project for Vietnamese
cultural heritage. It will collect and normalize source data, represent it as
RDF, link entities to external datasets, and expose the graph through SPARQL.

## Status

Phase 0: the repository and Python package foundation are in place. No
ontology classes or project business logic have been implemented.

## Setup

```bash
python -m venv .venv
```

Activate the virtual environment:

```bash
# macOS/Linux
source .venv/bin/activate

# Windows PowerShell
.venv\Scripts\Activate.ps1
```

Install the package and development dependencies:

```bash
python -m pip install -e ".[dev]"
```

## Quality Checks

```bash
python -m ruff check .
python -m pytest
```

## Repository Structure

```text
src/vietheritage_lod/  Python package and pipeline modules
ontology/              VietHeritageLOD ontology
data/                  Raw, processed, and RDF data directories
sparql/                SPARQL query directory
tests/                 Automated tests
docs/                  Project documentation and canonical context
```
