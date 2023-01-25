# PlantMap3D-BioMassEstimator

Biomass Estimation Module:
ROS wrapper will collect the output of the segmentation module for 8 segmentation arrays, 8 height above ground arrays from a height estimation module

Inputs:
- list of 8 segmentation label numpy 2D arrays 
- list of 8 height above ground 2D arrays

Outputs:
- list of 8 1D numpy arrays Biomass estimates for each possible species (floats)
