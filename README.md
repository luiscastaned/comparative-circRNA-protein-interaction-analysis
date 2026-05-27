# comparative-circRNA-protein-interaction-analysis
Automated comparative analysis of circRNA–protein interactions using HDOCK docking complexes.

# 🧬 Comparative circRNA–Protein Interaction Analysis Pipeline

This pipeline performs large-scale comparative analysis of RNA–protein interactions using docking-derived structural complexes.

The workflow was designed to analyze up to 300 complexes generated with HDOCK, corresponding to three experimental conditions:

- Wild-type helicase EHI_151600/circRNA
- UAP56 Human/circRNA
- EHI_151600 AAAA mutant/circRNA

The pipeline automatically:

- extracts docking complexes from compressed archives
- identifies protein and RNA atoms
- analyzes the interaction region (aa 179–182)
- computes intermolecular contacts using distance-based criteria
- classifies interactions into:
  - Hydrogen bonds
  - Aromatic stacking
  - Salt bridges
  - Hydrophobic interactions
  - Van der Waals contacts
  - Steric clashes
- calculates interaction favorability scores
- generates comparative statistics between conditions
- creates publication-ready plots
- exports CSV and Excel summary files

The workflow uses:

- MDAnalysis
- NumPy
- Pandas
- Seaborn
- NetworkX

and was designed for reproducible comparative analysis of circRNA recognition mechanisms in RNA-binding proteins.
