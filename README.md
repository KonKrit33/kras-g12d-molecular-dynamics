# KRAS G12D Molecular Dynamics Simulation

This repository contains a molecular dynamics project focused on the structure and dynamics of the KRAS G12D mutant. The project was developed as part of the Molecular Modeling of Biomolecules course in the MSc in Data Science & Information Technologies.

KRAS is a small GTPase that functions as an on/off molecular switch in cell signaling. The G12D mutation is one of the most important oncogenic KRAS mutations and is highly relevant to cancer biology and computational drug discovery.

## Project Overview

The objective of this project was to study the structural stability and conformational dynamics of KRAS G12D using molecular dynamics simulations.

The workflow includes:

- Structural inspection of KRAS G12D
- Protein preparation using VMD
- PSF generation using VMD/psfgen
- Solvation and ionization
- Energy minimization using NAMD
- Heating and equilibration under NVT conditions
- Production molecular dynamics simulation
- Salt-bridge distance analysis between ASP154 and ARG161
- RMSD analysis of KRAS backbone atoms
- RMSF analysis of per-residue flexibility
- Structural interpretation of flexible KRAS regions

## Biological Context

KRAS is one of the most frequently mutated oncogenes in human cancer. The G12D mutation disrupts normal GTP hydrolysis and promotes persistent KRAS activation, contributing to uncontrolled cell proliferation and tumorigenesis.

Studying the dynamics of KRAS G12D can help identify conformationally flexible regions, functionally relevant structural motifs, and potential opportunities for computational drug discovery.

## Key Analyses

### Energy Minimization

The KRAS G12D system was prepared in explicit solvent and minimized using NAMD. The potential energy decreased rapidly and reached a plateau, indicating successful structural relaxation before molecular dynamics.

### Heating and Equilibration

The system was gradually heated to 310 K and equilibrated under NVT conditions. Energy stabilization during equilibration indicated that the system reached a physically stable state before production dynamics.

### Production Molecular Dynamics

A production molecular dynamics simulation was performed under NVT conditions. Total energy and temperature remained stable during the production run, supporting the thermodynamic stability of the system.

### Salt-Bridge Analysis

The potential salt bridge between ASP154 and ARG161 was analyzed by monitoring distances between charged side-chain atoms. The analysis focused on ASP154 carboxylate oxygens and ARG161 guanidinium nitrogens.

### RMSD Analysis

Backbone Cα RMSD was calculated relative to the initial structure. The RMSD showed an initial relaxation phase followed by a stable plateau, indicating preservation of the overall KRAS fold during the simulation.

### RMSF and Flexibility Analysis

Per-residue Cα RMSF analysis identified the most flexible regions of KRAS, including:

- Switch I region
- Switch II region
- Surface loop regions
- Central flexible segments
- Hypervariable C-terminal region

These regions are functionally relevant because they participate in nucleotide-dependent conformational changes, effector interactions, and membrane-associated KRAS dynamics.

## Repository Structure

```text
.
├── KRAS_G12D_Molecular_Dynamics_Report.pdf
└── README.md
```

## Tools and Technologies

- Molecular dynamics
- VMD
- NAMD
- CHARMM force field
- PSF generation
- Protein solvation and ionization
- Energy minimization
- NVT equilibration
- RMSD analysis
- RMSF analysis
- Salt-bridge distance analysis
- Protein structure visualization
- Computational drug discovery

## Relevance

This project demonstrates practical experience in molecular modelling and simulation workflows relevant to computational drug discovery. It combines structural biology, molecular dynamics, trajectory analysis, and biological interpretation of an oncogenic protein target.

## Notes

Large trajectory files and intermediate simulation outputs are not included due to file size constraints. The repository focuses on the final report and selected analysis outputs relevant for reproducibility and scientific interpretation.
