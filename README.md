# Robust-Phylogenetics

Simulated Datasets for "Robust Phylogenetics" Paper

This repository contains simulated datasets and analysis scripts used in the 'Robust Phylogenetics' study. The data and scripts are organised into specific folders, each corresponding to different simulation scenarios and analyses.

Data Folder Structure

The data folder contains the following:

        1. A PDF file titled "_SupplementaryMaterial_RobustPhylogenetics," which contains supplementary figures and tables referenced in the paper.

        2. Mislabelling Simulations: These simulations test the effectiveness of the trimmed log-likelihood method in detecting and removing mislabelled sites.

        3. Convergent Process Simulations: These simulations evaluate the method's performance when different evolutionary processes occur across various lineages.

        4. Saturation Simulations: These simulations investigate how the method performs when alignments contain mostly fast-evolving or saturated sites.


File Format and Organisation

The Saturation Simulations folder contains 100 DNA sequence alignments, saved in .fst format, which simulate sequences with a deep branching tree, where multiple substitutions at the same sites complicate phylogenetic inference.
The Mislabelling Simulations and Convergent Process Simulations folders each have subfolders representing different simulation conditions (e.g., varying branch lengths or evolutionary models), containing a total of 400 DNA sequence alignments in .fst format.

Empirical Datasets

For the empirical analyses, two datasets were used:

       1. Thermus Dataset: Available in the paper by Cummins & McInerney (2011).

       2. Arthropods Dataset: Available in the paper by Pisani (2004).


Scripts Folder Structure

The scripts folder includes:

       1. The 'robust_phylo_functions' R script: This script contains core functions required for analysing the simulation results, including calculating Robinson-Foulds distances between the generating (true) trees and inferred trees.

       2. Three Subfolders: 'Mislabelling Simulations',  'Convergent Process Simulations', and 'Saturation Simulations'. Each subfolder contains the necessary R and bash scripts to perform specific analyses for the corresponding         simulations. The scripts are named using the format step_number_xxx, where the number indicates the sequence in the analysis workflow (e.g., step_1_generate_alignments.R).

Workflow

To perform the analysis:

Begin with scripts labelled step_1 in the respective simulation folder.
Proceed through the steps sequentially (step_2, step_3, etc.) to ensure proper workflow execution for each set of simulations.
