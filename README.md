# AB-DB Tutorial

A Jupyter Notebook tutorial for finding, downloading, visualizing, and retrieving analysis results from the **[AB-DB](https://mmb.irbbarcelona.org/ABDB/)** database of antibiotic ligand MD simulations and QM data.

**Authors:** Giuliano Malloci, Silvia Gervasoni, Adam Hospital, Genís Bayarri  
**Version:** July 2026  
**Institutions:** University of Cagliari · IRB Barcelona

---

## Overview

The tutorial walks through the AB-DB REST API (`https://mmb.irbbarcelona.org/ABDB/api`) step by step:

1. **Listing compounds** — browse the full AB-DB collection with FAIR IDs, families, formulae, and MDDB accessions
2. **Browsing by family** — interactive dropdown to explore compound families
3. **Searching & finding** — query compounds by keyword/family
4. **Physico-chemical descriptors** — download and inspect 250+ molecular descriptors (CSV)
5. **MD data**
   - Download PDB structure and XTC trajectory
   - Visualize interactively with NGL Viewer
   - Link out to trajectory analyses in [MDDB (MDposit)](https://mdposit.mddbr.eu/)
6. **QM data**
   - Download QM-optimized structure (SDF) and compare against the MD structure
   - Retrieve AMBER force-field parameters (`.frcmod` / `.prep`)
   - Link out to geometry optimization and single-point energy data in [ioChem-BD](https://iochem-bd.org/)

---

## Requirements

Create and activate the conda environment:

```bash
conda env create -f conda_env/environment.yml
conda activate abdb_rest
```

Key dependencies: `jupyter`, `nglview`, `simpletraj`, `pandas`, `rich`, `qgrid`

---

## Usage

```bash
jupyter notebook AB-DB_tutorial.ipynb
```

---

## Links

| Resource | URL |
|---|---|
| AB-DB website | https://mmb.irbbarcelona.org/ABDB/ |
| AB-DB REST API | https://mmb.irbbarcelona.org/ABDB/api |
| MDDB (MDposit) | https://mdposit.mddbr.eu/ |
| ioChem-BD | https://iochem-bd.org/ |
