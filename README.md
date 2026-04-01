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
- `stochastic_simulation_plotting.ipynb`: Visualization of simulation results by various patterns.
- `/data`: Empirical data from Satake et al. (2024).
- `/results`: Simulation outputs and intermediate results.

## Requirements
- Python 3.10.13
- numpy==2.0.1
- pyabc==0.12.15
- scipy==1.15.3
- pandas==2.2.3
- seaborn==0.13.2
- dendropy==5.0.8
- matplotlib==3.10.0

## Contact
**Sou Tomimoto** Email: sou.tomimoto[at]gmail.com  
Author Contributions: Data collection, model development, and lead coding.
