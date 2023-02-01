# PlantMap3D-BioMassEstimator

Biomass Estimation Module:
ROS wrapper will collect the output of the segmentation module for 8 segmentation arrays, 8 height above ground arrays from a height estimation module

Inputs:
- list of 8 segmentation label numpy 2D arrays 
- list of 8 height above ground 2D arrays (not used in version 1)

Process:
1. count pixels for each species from segmentation label input
2. apply a linear y = mx+b correlation between species pixel count and biomass (by species if necessary)

Outputs:
- list of 8 1D numpy arrays Biomass estimates for each possible species (floats)

Roadmap:
1. Version 1 release date: 2/10/2023
2. Version 2: change biomass estimation to include height information to calculate volume per species. Then the biomass estimate would be a correlation between species volume and biomass. No release date yet.
3. Version 3: change biomass correlation method to be either more statistically sophisticated, or introduce a neural network for biomass estimation.
