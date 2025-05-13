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

Snippet mentions a PAL mutant Y110F that showed a very significant loss of activity, indicating that Tyrosine at position 110 is crucial for catalysis or substrate binding in PAL.
Snippet  refers to Tyr110 as an analogous residue in parsley PAL (PcPAL, which corresponds to 1W27) and mentions its location near the substrate entrance channel to the MIO group, which is the catalytic center of PAL.   
Snippet  explicitly lists Tyr110 (UniProt numbering) as a catalytic residue in PDB entry 1w27, noting its role in making ammonia a better leaving group. It also mentions Asp351 (corresponding to your 349 in PDB numbering, so likely related to your 348 or 349) as deprotonating the substrate. While your list doesn't have 349/351, it's in the vicinity.   
Snippet  also mentions other essential residues determined by mutagenesis, such as His83, Arg283, Met382, Tyr53, Tyr280, Asn195, and Glu414 (using the numbering from a related enzyme, PpHAL). While these numbers don't directly match yours, they highlight that the active site involves multiple key residues.   
Snippet  mentions Lys486 as being located on the active site helices and contributing to MIO cofactor stabilization. This is close to your residue 488.   

Cofactor: MIO is a crucial cofactor involved in the catalytic reaction of phenylalanine ammonia-lyase (PAL).
Electrophilic Nature: It's a highly electrophilic moiety that sits in the active site of PAL.  This electrophilicity is enhanced by its location atop the positive pole of three polar helices in the active site.    
Formation: MIO is formed autocatalytically within the enzyme from a conserved Ala-Ser-Gly tripeptide segment through cyclization and dehydration.    
Mechanism: In the catalytic mechanism, the aromatic ring of L-phenylalanine attacks the MIO, activating the C-H bond for deprotonation.  The MIO then facilitates the elimination of ammonia.    
Active Site Component: The active site of PAL contains the MIO group, which is non-covalently bonded to three helices.  Specific residues like Leu266, Asn270, Val269, Leu215, Lys486, and Ile472 are located on these active site helices and Phe413, Glu496, and Gln500 contribute to its stabilization.    
Comparison to other enzymes: MIO is also found in other ammonia lyases like histidine ammonia-lyase (HAL) and aminomutases.   
In essence, the MIO group is the essential chemical component within the active site of PAL that directly participates in the deamination reaction of phenylalanine (and potentially other substrates like myristicin).

