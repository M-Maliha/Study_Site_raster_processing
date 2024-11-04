**Site-Specific Raster Processing Notebook**

*Overview* 

This notebook is designed to process cold site rasters by resampling and reprojecting them to match an RGB raster's specifications. The notebook also includes steps to modify the data type of the original RGB raster to match that of the reprojected rasters for consistency.

*Features*

Resampling: Adjusts the resolution of the cold site rasters to match that of the target RGB raster.
Reprojection: Reprojects the cold site rasters to the coordinate reference system (CRS) of the RGB raster, ensuring spatial alignment.
Data Type Adjustment: Modifies the data type of the original RGB raster to match the data type of the reprojected rasters, facilitating consistent data handling across different raster layers.

*Prerequisites*
This notebook requires the following Python libraries:

rasterio: For reading and writing raster data.
numpy: For handling raster data arrays.
geopandas (optional): For spatial vector data processing.


Load Cold Site Rasters: The notebook loads cold site raster files, which will be resampled and reprojected to match the RGB raster specifications.
Resample and Reproject: Using the target RGB raster as a reference, each cold site raster is resampled and reprojected to match its resolution and CRS.
Adjust Data Type: The data type of the original RGB raster is adjusted to match the data type of the reprojected cold site rasters for consistency in further analyses.

*Output*
Reprojected Cold Site Rasters: All processed rasters will have the same resolution and CRS as the target RGB raster.
Updated RGB Raster: The original RGB raster will be modified to have the same data type as the reprojected rasters.
