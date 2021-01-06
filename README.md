# R-Digital-Hillslope-Position
### Automated digital hillslope position classification algorithm - Miller and Schaetzl (2015)
#### Consult the Wiki for the tutorial - An Rmarkdown file is also available

Classification of hillslope position has a long history in soil geomorphology. However, its roots in tacit field knowledge has prevented its use in GIS. The model provided here has been calibrated and validated on soil scientists’ observations in the field. The resulting maps of hillslope position represent base maps that can be used to (1) improve research on toposequences by providing explicit definitions of each hillslope element’s location, (2) facilitate the disaggregation of soils currently mapped as complexes, and (3) identify map unit inclusions that exist due to subtle topographic variation. The base maps developed by the model can also help identify areas of possible mismapping, especially where soil boundaries cross topographic breaks. This information can enable the mapper to redefine many existing soil map unit boundaries, placing them more correctly at locations where defendable landscape breaks exist.

![alt text](https://github.com/MollicMeyer/R-Digital-Hillslope-Position/blob/main/DHPwidescreen.jpg?raw=true)

## Summary

Ruhe and Walker (1968) defined and identified five hillslope profile positions for geomorphically describing landscapes, which have been incorporated into methods utilized by the USDA-NRCS (Wysocki et al., 2000; Schoeneberger et al., 2012). This ArcGIS tool takes the terrain parameters of slope gradient, profile curvature, and relative elevation to make determinations of hillslope position. Please note that hillslope position is highly sensitive to the analysis scale used for the respective parameters. Based on calibration to soil scientists' use of hillslope position in the field, the following parameter analysis scales are recommended:

Slope gradient = 9m  
Profile curvature = 63m  
Relative elevation = 135m  

The hillslope position grid produced by this classification tool uses the following codes:

1 = summit  
2 = shoulder  
3 = backslope  
4 = footslope  
5 = toeslope  

Landscape analysis of hillslope position will not result in a full sequence of positions for all slopes. Instead, each grid cell is classified by its contextual shape meeting specified definitions. In this way, this hillslope position classification is identifying zones of surficial processes as influenced by morphology.

This fully automated tool uses the classification breaks established by calibration to soil scientists' use of hillslope position in the field. If the user wishes to make the classification by different breaks, (*refer to .RMD line 130) for manual specification of breaks. Slope gradient is divided by two breaks to create low(-1; <1.4<sup>o</sup>), medium(0; 1.4<sup>o</sup> to 2.9<sup>o</sup>), and high(1; > 2.9<sup>o</sup>) classes. Profile curvature and relative elevation are divided by one break to create low(-1; <0) and high(1; >0) classes. Ths.


## References

Ruhe, R.V. and P.H. Walker. 1968. Hillslope models and soil formation: I. Open systems. Transactions of the 9thInternational Congress of Soil Science. 4:551-560. Adelaide, Australia.  
Schoeneberger, P.J., D.A. Wysocki, E.C. Benham, and Soil Survey Staff. 2012. Field Book for Describing and Sampling Soils, Version 3.0. U.S. Department of Agriculture, Natural Resource Conservation Service. Lincoln, Nebraska.  
Wysocki, D.A., P.J. Schoeneberger, H.E. LaGarry. 2000. Geomorphology of Soil Landscapes. InM.E. Sumner (ed.). Handbook of Soil Science. CRC Press. Boca Raton, Florida.

## Cite the tool
Development of the hillslope position classification tool is documented in the following publications and dissertation, and should be used for citation as appropriate:

Miller, B.A. and R.J. Schaetzl, 2015. Digital classification of hillslope position. Soil Science Society of America Journal 79(1):132-145. doi:10.2136/sssaj2014.07.0287.  
Miller, B.A., 2014. Semantic calibration of digital terrain analysis. Cartography and Geographic Information Science Journal 41:166-176. doi:10.1080/15230406.2014.883488.  
Miller, B.A. 2013. Incorporating tacit knowledge of soil-landscape relationships for digital soil and landscape mapping applications. Dissertation, Department of Geography, Michigan State University, USA.  

![alt text](https://github.com/MollicMeyer/R-Digital-Hillslope-Position/blob/main/burroak3.gif?raw=true)
