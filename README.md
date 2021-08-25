# KMC-simulations-for-electrocatalysis-with-Zacros
This repository includes 5 Jupyter notebooks and corresponding folders containing sample input and output files for KMC simulations for the electrocatalysis with Zacros. The folder *zacros_wrapper* is from the authors of software Zacros. *Units.py* contains frequently used units.

Specifically, 

*01-parameter-CO-stripping+Goodpaster.ipynb* is for parameters conversion to the form for Zacros using the samples from the CO stripping model and Goodpaster model.

*02-CO-stripping-MKM.ipynb* exhibits running microkinetic models for Cyclic Voltammetry（CV) and potential steps (PS). Results can be compared with KMC results.

*03-PS-Multi.ipynb* runs potential steps for CO stripping with multiple trajectories and provides plots for adsorbate coverage and current density. Folder *03-PS-Multi-SF* contains sample simulation files and outputs.

*04-CV-Multi.ipynb* runs CV for CO stripping with multiple trajectories and provides plots for adsorbate coverage and current density. Note that CV requires reading the last snapshot of forward sweeping and coding that as the initial state for backward sweeping, and in the notebook includes the methods dealing with bidentate situations. Folder *04-CV-Multi-SF* contains sample simulation files and outputs.

*05-Isotope-Multi.ipynb* runs the two-site model for CO$_2$ reduction for multiple trajectories and saves data in .csv files that can be further analyzed. Folder *05-Isotope-Multi* contains sample simulation files and outputs. Note that the *lattice_input.dat* and *state_input.dat* should be changed for different region sizes.
