# Inferring_somatic_mutation_dynamics
Codes for the following article:  
Tomimoto, S. and Satake, A. 2026. Inferring somatic mutation dynamics from genomic variation across branches within long-lived tropical trees.

In that paper, 
-	We built mathematical models to predict the genetic differences between branch tips by somatic mutations.
-	The model considers the varying dynamics of stem cells in shoot meristem during shoot elongation and branching.
-	We compared the model prediction with empirical data from tropical trees, Dipterocarpaceae, and estimated the dynamics of stem cells and mutation rate.
-	Somatic mutation dynamics were shaped by somatic genetic drift arising from stem cell lineage replacement during shoot elongation and branching.
-	Accounting for stem cell dynamics led to slightly smaller estimates of mutation rates compared with previous estimates that ignored the dynamics.
-	Our models offer insights into how genetic variability is shaped in the tropical trees and the stem cell dynamics underlying their long-term growth.

S.T. is responsible for collecting data, and writing code (Contact details: sou.tomimoto[at]gmail.com). 
Link to the manuscript would be available in the near future.

All codes were performed in Python (version 3.10.13). There are 4 code files (for mathematical calculations, model fitting, stochastic simulation, and corresponding visualization) and 2 folders (for data from Satake et al 2024 and simulation results).

markov_chain_ABCSMC.ipynb:   calculating the inter-branch SNVs by the Markov chain model and model fitting by ABC-SMC.
markov_chain_plotting.ipynb: plotting model prediction based on MAP parameters
markov_chain_para_dep.ipynb: plotting model prediction under varying parameters to evaluate parameter dependency of the model.
stochastic_simulation.ipynb: simulating various patterns of somatic mutation accumulation by the simulation model (Tomimoto & Satake 2023 JTB) 

Following is the package information used in the code:
numpy==2.0.1
pyabc==0.12.15
scipy==1.15.3 
pandas==2.2.3  
seaborn==0.13.2  
matplotlib==3.10.0  


# Inferring Somatic Mutation Dynamics

This repository contains the Python implementation for the following article:  
**Tomimoto, S. and Satake, A. (2026). Inferring somatic mutation dynamics from genomic variation across branches within long-lived tropical trees.**

## Overview
-	We built mathematical models to predict the genetic differences between branch tips by somatic mutations.
-	The model considers the varying dynamics of stem cells in shoot apical meristems during apical growth and branching.
-	We compared the model prediction with empirical data from tropical trees, Dipterocarpaceae, and estimated the dynamics of stem cells and mutation rate.
-	Somatic mutation dynamics were shaped by somatic genetic drift arising from stem cell lineage replacement during shoot elongation and branching.
-	Accounting for stem cell dynamics led to slightly smaller estimates of mutation rates compared with previous estimates that ignored the dynamics.
-	Our models offer insights into how genetic variability is shaped in the tropical trees and the stem cell dynamics underlying their long-term growth.

## Repository Structure
- `markov_chain_ABCSMC.ipynb`: Inter-branch SNV calculation and model fitting via ABC-SMC.
- `markov_chain_plotting.ipynb`: Visualization of model predictions based on MAP (Maximum A Posteriori) parameters.
- `markov_chain_para_dep.ipynb`: Parameter dependency analysis and sensitivity testing.
- `stochastic_simulation.ipynb`: Stochastic simulations of somatic mutation accumulation (based on Tomimoto & Satake 2023, JTB).
- `/data`: Empirical data from Satake et al. (2024).
- `/results`: Simulation outputs and intermediate results.

## Requirements
- Python 3.10.13
- numpy==2.0.1
- pyabc==0.12.15
- scipy==1.15.3
- pandas==2.2.3
- seaborn==0.13.2
- matplotlib==3.10.0

## Contact
**Sou Tomimoto** Email: sou.tomimoto[at]gmail.com  
Author Contributions: Data collection, model development, and lead coding.
