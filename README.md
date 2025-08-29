# Ottawa Solar Resource Assessment

This project performs a **solar site suitability analysis** for the Ottawa region. It combines **land cover**, **slope**, and **distance to transmission lines** to generate a final suitability mask for solar installations.

## Requirements

Install dependencies from `requirements.txt`:

Main libraries used:
	•	rasterio – for raster operations
	•	geopandas – for vector data handling
	•	numpy – for numerical operations
	•	matplotlib – for plotting
	•	scipy – for distance transform

 1.	Place and analyze the input data in the data/ folder using DataCollection.ipynb and Data_Exploration_Visualization.ipynb:
	•	Land cover raster (.tif)
	•	DEM and slope rasters (.tif)
	•	Solar radiation data (.csv)
	•	Transmission grid lines (.shp)
2.	Run the notebook solar_resource_assessment.ipynb step by step to:
	•	Generate land cover suitability mask
	•	Generate slope suitability mask
	•	(Optional) Generate grid proximity mask
	•	Combine masks into a final suitability raster
  3. Forecast the Global Horizontal Irradiation (GI) in Ottawa region in GHI_Forecast.ipynb.
  4. Forecast PV yield estimation in Ottawa region using PV_Yield_Estination_PVGIS.ipynb.
