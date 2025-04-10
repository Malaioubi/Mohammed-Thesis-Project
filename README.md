# Mohammed Thesis Project

# Predicting Molecular Structures from Mass Spectrometry Data Using Machine Learning

This repository contains a computational pipeline designed to simulate, fragment, and optimise mass spectra of chemical compounds using RDKit and a genetic algorithm. The workflow processes compound data, simulates ionisation and fragmentation reactions, matches simulated spectra with experimental data, and uses optimisation techniques to enhance the simulation. Finally, both qualitative and quantitative comparisons are performed between the simulated and experimental spectra.

> **Note:**  
> Due to its large size, the GNPS database file (`GNPS-LIBRARY.json`) that this model relies on could not be uploaded to this repository. Please download the GNPS database file from the GNPS website (https://ccms-ucsd.github.io/GNPSDocumentation/gnpslibraries/) and place it in the repository root (or update the file path in the code) to run the pipeline.


## Overview

This project aims to:

- **Pre-process Compound Data:**  
  Read and validate SMILES/InChI data from a JSON file.
  
- **Simulate Ionisation and Fragmentation:**  
  Use RDKit to convert compounds into their ionised forms and simulate fragmentation reactions.
  
- **Match Experimental Data:**  
  Use a KDTree-based nearest-neighbour search to match simulated m/z peaks with experimental mass spectrum data.
  
- **Optimise Transition Probabilities:**  
  Use a genetic algorithm to optimise the transition probabilities governing the fragmentation process.
  
- **Visualise Results:**  
  Generate visual comparisons between the experimental and simulated spectra, including a visualisation of the fragmentation tree.
  
- **Quantitative Analysis:**  
  Calculate similarity metrics (cosine similarity) between the simulated and experimental spectra.



### Requirements

- **Python 3.7 or Higher:** Ensure you have a compatible version of Python installed.
- **Dependencies:**  
  The pipeline uses several Python libraries including:
  - RDKit  
  - NumPy  
  - Pandas  
  - Matplotlib  
  - NetworkX  
  - scikit-learn  
  - SciPy
