# Temporal span of biodiversity monitoring mediates the effects of area and environment

Code and files for reproducible Random Forest analyses of temporal monitoring effects on Czech bird species richness

## Files

- `all_data_star.rds`: Combined datasets (Atlases, jpsp_points, jpsp_transects, SPARSE)
  - `richness`: Response variable - Observed bird species richness in a given geographic unit  (i.e.,point, polygon, cell, transect)
  - `time_span`: the time span of each survey (in years)
  - `start_year`: the first year of sampling (year)
  - `tas`(°C) : Mean temperature  
  - `tmin` (°C) :Min temperature
  - `tmax`(°C) :Max temperature
  - `pr` (mm): Precipitation
  - `AREA`(km²): the area of each geographic unit
  - `lat`, `lon` (°): latitude, longitude
  - `median_ndvi`: median of the Normalized Difference Vegetation Index. Unitless index, values range from -1 to 1.
  - CORINE Land Cover (km²): Area of each geographic unit covered by different land use covers (e.g.,forests, urban, agriculture, water)
  - `Protected_area` (km²): Area of each geographic unit covered by protected area. Nature Conservation Agency of the Czech Republic
  - `DataSet` (Category): The name of the dataset to which each data entry belongs.These are: Atlases, jpsp_points, jpsp_transects, SPARSE.
  
\n
  - `random_forest_star.qmd`: Main Quarto document containing the code to run all our analyses. 

- `prediction_data.rds`: The data set used to predict at different time spans. Contains the same predictors that "all_data_star.rds".
   
   