# molecular docking 2025
Title: Computational Docking Analysis of Petroselinum crispum Phenylalanine Ammonia-Lyase for Myristicin Biotransformation  
Abstract: Phenylalanine ammonia-lyase (PAL) from Anabaena flos-aquae has been identified as a novel biocatalyst for myristicin biotransformation, producing compounds with potential pharmacological applications. This study extends these findings by employing computational molecular docking to investigate the substrate specificity and binding interactions of PAL from parsley (Petroselinum crispum, PDB ID: 1W27), demonstrating the efficacy of plant-derived enzymes. Using AutoDock Vina, the parsley PAL was docked with ligands including phenylalanine, cinnamic acid, myristicin, and elemicin, following structural preparation with PDBFixer, pdb2pqr, and Open Babel. Docking was performed at pH 8.0, targeting the enzyme’s active site (residues 110, 134, 136, 488), with binding affinities calculated to assess catalytic potential. Interactive 3D visualizations generated with py3Dmol revealed favorable binding poses within a hydrophobic pocket, consistent with the enzyme’s mechanism for nucleophilic attack and ammonia uptake. Results indicate myristicin’s high binding affinity, supporting its biotransformation potential. This open-source pipeline, implemented in Google Colab, provides a scalable framework for enzyme-ligand interaction studies, with applications in drug synthesis, biofuel production, and environmental deamination. The code and visualizations are freely available on GitHub, fostering collaborative advancements in plant and algal biotechnology.

PAL Docking for Myristicin Biotransformation
This repository contains a computational pipeline for molecular docking of phenylalanine ammonia-lyase (PAL) from parsley (Petroselinum crispum, PDB ID: 1W27) with myristicin and related ligands, building on the study "Purification and Characterization of Anabaena flos-aquae Phenylalanine Ammonia-Lyase as a Novel Approach for Myristicin Biotransformation" (J. Microbiol. Biotechnol., 2020). The pipeline, implemented in Python for Google Colab, prepares protein and ligand structures, performs docking with AutoDock Vina, and visualizes binding interactions using py3Dmol. It demonstrates the capability of plant-derived PAL enzymes in biotransforming myristicin into valuable products for pharmacological applications.
Features
Protein Preparation: Downloads parsley PAL structure (1W27), fixes missing atoms with PDBFixer, assigns charges at pH 8.0 using pdb2pqr, and converts to PDBQT format with AutoDockTools.

Ligand Preparation: Converts SMILES strings of phenylalanine, cinnamic acid, myristicin, elemicin, and others into 3D MOL2 and PDBQT formats using Open Babel and AutoDockTools.

Molecular Docking: Performs docking with AutoDock Vina, targeting PAL’s active site (residues 110, 134, 136, 488), using a 20x20x20 Å grid box and exhaustiveness of 32.

Visualization: Generates interactive 3D visualizations of protein-ligand complexes and docking grids using py3Dmol, with binding affinities extracted from Vina logs.

Applications: Supports research in enzyme kinetics, plant and algal biotechnology, drug synthesis, and environmental applications like waste deamination.

Hope You enjoyed, please share my name & email in citations if you use or modify, Joseph Erickson josepherickson135@gmail.com

google colab: https://colab.research.google.com/github/400lbhacker/moleculardocking/blob/main/Joseph_Erickson_molecular_docking_2025.ipynb
