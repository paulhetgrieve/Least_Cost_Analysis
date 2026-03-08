# Grizzly Bear Movement Corridors – Least Cost Path Analysis

This project models potential grizzly bear movement corridors across the Rocky Mountain foothills of western Alberta using raster-based least cost path analysis. The objective was to identify routes that minimize cumulative movement cost between core habitat areas while accounting for terrain, land cover, and human disturbance.

The analysis began by defining an area of interest representing the Yellowhead Bear Management Area. Multiple raster datasets were processed and aligned to a common spatial reference system, resolution, and extent using GDAL utilities and QGIS. Digital elevation data were mosaicked and reprojected to generate a terrain surface used to derive slope, while a national land cover dataset was reclassified into movement resistance values based on expected grizzly bear habitat preferences.

Distance to roads was calculated as a proxy for human disturbance, with higher movement costs assigned to areas closer to roads. These layers were normalized to a common scale and combined using a weighted overlay to create a composite landscape resistance surface representing the energetic and ecological cost of movement.

Least cost path analysis was then performed to identify the optimal travel route between a core habitat area and a secondary habitat area. The resulting corridor illustrates how terrain, vegetation structure, and human infrastructure influence predicted wildlife movement patterns across the landscape.

## Key Outputs

- Landscape cost surface representing grizzly bear movement resistance  
- Derived slope raster from ASTER DEM data  
- Reclassified land cover cost layer  
- Distance-to-roads disturbance layer  
- Least cost movement corridor between habitat areas  

## Tools and Methods

- GDAL raster processing utilities  
- QGIS raster analysis and spatial preprocessing  
- ArcGIS Pro least cost path modelling  
- Weighted raster overlay and cost surface modelling  
- Wildlife connectivity and landscape resistance analysis  

## Final Corridor Map

![Grizzly Bear Least Cost Path](Layout.png)
