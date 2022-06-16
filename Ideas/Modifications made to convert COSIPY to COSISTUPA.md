202204070921

**Tags:** #model 

# [[Modifications made to convert COSIPY to COSISTUPA]]
## Inputs added
1. **DISCHARGE** (litres per minute): Fountain discharge rate
2. **BETA** (radians): Solar elevation angle from solarFParallel in radCor.py
3. **CLD**: Cloudiness index used to separate global solar radiation

## Parametrizations changed/introduced:
1. **make_icestupa**:
a. Precipitation divided into rain or snow using a new parameter called temperature_threshold_precipitation. Also snowfall and rain quantity is downscaled to correspond to settling on conical surface.
b. Discharge is converted from l/min to m w.e.
c. Solar radiation fraction impact on a cone is determined using the solar area fraction (f_cone) described in Balasubramanian22
d. Penetrating radiation and refreezing is assumed to be negligible
2. **remesh_method**: Adaptive profile used for small icestupas (swiss) and log profile used for big ones (indian). This is because log_profile does not converge to solutions for small icestupas and adaptive_profile takes too long to compute outputs for big icestupas.
3. **first_layer_height** increased to 0.05 m which corresponds to the calibrated value used in Balasubramanian22
4. **Ground heat flux** disabled by setting parameters zlt1, zlt2 to 0. This is because it is not clear how ground heat flux can be adjusted for icestupas.
5. **Roughness method** is set to constant. The calibrated value of 3 mm is used from Balasubramanian22
6. **Surface emissivity coefficient** is varied based on whether it is a snow or ice surface. The default value of 0.99 corresponds to snow emissivity coefficient and 0.97 is used if it is an ice surface. 
7. **Turbulent fluxes** increased as a function of the slope of the cone. 
8. **Fountain Rain heat flux** introduced. It is determined using the fountain water temperature provided during the initialisation step.


## New algorithms implemented
1. **Shape**: Algorithm of the conical shape evolution of icestupa was implemented from Balasubramanian22. This converts the surface mass balance output of the cosipy model into volume changes of icestupa. Mean density of all the layers is used to compute the volume instead of constant ice density used in the old model. The initial height of the cone was provided using the initial_snowheight_constant or the initial_glacier_height parameters during the initialisation step along with the spray radius of the fountain.
2.  **Freezing process**: Algorithm for the surface freezing process instigated by fountain discharge or rain was implemented from Balasubramanian22. Cold content of the surface layer drives this process.

## Advantages
1. **Albedo**: Due to separation of rain and snow, the corresponding albedo feedback is better resolved.
2. **Removal of surface layer thickness parameter**: DX was a very sensitive parameter of the model and the model generally performed poorly when it was not calibrated with field observations. This is no longer the case as spatial temperature variation is better resolved.  
3. **AIR density and surface characterisitics**: Since Cosistupa retains information about the density of each layer and implements a densification algorithm to evolve it temporally, better quantification of AIR density is possible. Moreover, this also enables better estimation of surface albedo. 
---
# References
1. [@balasubramanianInfluenceMeteorologicalConditions2022]