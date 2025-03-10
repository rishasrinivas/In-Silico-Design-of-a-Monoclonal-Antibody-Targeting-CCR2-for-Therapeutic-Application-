<h1>In Silico Design of a Monoclonal Antibody Targeting CCR2 for Therapeutic Applications</h1>

This repository contains the computational design and characterization of a monoclonal antibody (mAb) targeting CCR2, the receptor involved in non-alcoholic steatohepatitis (NASH). The aim is to develop a therapeutic intervention with high binding affinity and stability against CCR2.

<h3>Table of Contents</h3>

Introduction

Installation

Usage

Results

Future Work

Contributors


<h3>Introduction</h3>
	
Non-alcoholic steatohepatitis (NASH) is a severe form of non-alcoholic fatty liver disease (NAFLD) characterized by fat accumulation, inflammation, and liver cell 	damage. CCR2, a chemokine receptor, plays a crucial role in the recruitment of immune cells involved in chronic inflammation and fibrosis. This project focuses on 	designing a monoclonal antibody targeting CCR2 to mitigate the inflammatory and fibrotic processes in NASH.

<h3>Installation</h3>

To run this project, you will need the following:
 
Python 3.x
   
Required libraries: Biopython, NumPy, Matplotlib, PyMOL, ClusPro, PRODIGY, GROMACS
   
You can install the required libraries using pip:
    
				pip install biopython numpy matplotlib pymol
      
For ClusPro, PRODIGY, and GROMACS, follow the installation instructions provided on their respective websites.
    
<h3>Usage</h3>

Sequence Alignment and Epitope Prediction:

Use Clustal Omega for sequence alignment.
  
Predict epitopes using the IEDB Linear Epitope Prediction tool and Ellipro.
  
Antibody Modeling:

Select an appropriate antibody template (e.g., PDB ID: 2BDN).
  
Use ABodyBuilder2 to model the antibody structure.
  
Molecular Docking:

Perform docking simulations using ClusPro.
  
Analyze binding affinity using PRODIGY.
  
Molecular Dynamics Simulations:

Prepare the system using CHARMM27 force field and TIP3P water model.
  
Run energy minimization, equilibration (NVT/NPT), and production MD simulations using GROMACS.
  

<h3>Results</h3>

<h5>Epitope Prediction</h5>
 
Linear epitope: Residues 1013-1054 (YNPEDGDPDNGVNPGTDFKDIPDDWVCPLCGVGKDQFEEVE)
    
Discontinuous epitope: Residues 230-1052
    
<h5>Antibody Modeling</h5>
 
Antibody model with low prediction errors (e.g., CDR-H3 region: 0.20)
    
Structural validation using PROSA, ERRAT2, and Verify3D
    
<h5>Molecular Docking</h5>
 
Binding affinity (ΔG): -8.0 kcal/mol
    
Dissociation constant (Kd): 1.4 µM
    
<h5>Molecular Dynamics Simulations</h5>
 
RMSD stabilizes at around 0.175 nm
    
RMSF indicates flexible regions (e.g., around residue 4000)
    
Hydrogen bonds remain stable throughout the simulation
    

<h3>Future Work</h3>

Experimental validation of the designed antibody through in vitro and in vivo studies.
 
Optimization of binding affinity and stability.
 
Application of this computational approach to design antibodies against other disease-related proteins.
 

<h3>Contributors</h3>

**Risha Reddy Mukkisa** - Initial project design and implementation

