202202201618

**Status:** #review 

**Tags:** #model, #tech

# [[Diffuse solar radiation]]
Model updated with pvlib module [1] to include estimated cloudiness value and diffuse solar radiation just from latitude, longitude and altitude. The cloudiness determination assumes $cld = 1- clr$ where clr is clearness value estimated from Erbs [3]. The Diffuse radiation is estimated from Iniechen [2]. The uncertainty of this approach is discussed in  [4].


---
# References
1. [@holmgrenPvlibPythonPython2018]
2. [@ineichenBroadbandSimplifiedVersion2008]
3. [@erbsEstimationDiffuseRadiation1982] 
4. [@ineichenValidationModelsThat2016]