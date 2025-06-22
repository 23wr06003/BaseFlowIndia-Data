# BaseFlowIndia-Data: Supplementary Data for Baseflow Simulation in Central and South India (1979-2020)

## Baseflow Animation (1979-2020)
![Monthly Baseflow Simulation](https://raw.githubusercontent.com/23wr06003/BaseFlowIndia-Data/main/BaseflowIndia.gif)  
*Visualization of monthly baseflow patterns across Central and South India*

## 📄 Purpose
This repository contains supplementary data for the manuscript:
**"Estimating Gridded Monthly Baseflow across Central and Southern India"** submitted to the *Journal of Hydrology*. It includes:
- Final baseflow simulation outputs
- Source data references
- Methodology documentation

## 📂 Repository Contents
| File/Directory          | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `baseflow_1979-2020.tiff` | **Primary output**: Monthly baseflow (mm/month) at 0.25° resolution        |
| `BaseflowIndia.gif`       | Animated visualization of spatiotemporal patterns (1979-2020)               |
| `data_sources/`           | Directory containing metadata for all input datasets                        |
| `LICENSE`                 | Usage terms (CC BY 4.0)                                                   |

## 🌐 Data Sources
### Input Datasets Used for Simulation

| Variable Type         | Description                          | Units       | Source               | Resolution              |
|-----------------------|--------------------------------------|-------------|----------------------|-------------------------|
| **Dynamic Variables** |                                      |             |                      |                         |
| Total Precipitation   | Monthly accumulated rainfall         | mm/day      | ERA5                 | 0.25°, Monthly          |
| 2m Temperature        | Air temperature at 2 meters          | °C          | ERA5                 | 0.25°, Monthly          |
| 2m Dewpoint Temp      | Dewpoint temperature at 2 meters     | °C          | ERA5                 | 0.25°, Monthly          |
| 10m Wind Speed        | Wind speed at 10 meters              | m/s         | ERA5                 | 0.25°, Monthly          |
| Surface Net Radiation | Net radiation at surface             | W/m²        | ERA5                 | 0.25°, Monthly          |
| Potential Evapotranspiration | Penman-Monteith PET           | mm/day      | Calculated from ERA5 | 0.25°, Monthly          |
| Leaf Area Index       | Vegetation leaf area index           | unitless    | ERA5                 | 0.25°, Monthly          |
| **Static Variables**  |                                      |             |                      |                         |
| Mean Elevation        | Basin average elevation              | m           | MERIT DEM            | 90m                     |
| Mean Slope            | Basin average slope                  | degrees     | MERIT DEM            | 90m                     |
| Forest Fraction       | Forested area percentage            | %           | MODIS                | 500m                    |
| NDVI                  | Normalised difference vegetation index | unitless  | Landsat              | 30m                     |
| Clay Fraction         | Soil clay content                    | %           | SoilGrids            | 250m                    |
| Sand Fraction         | Soil sand content                    | %           | SoilGrids            | 250m                    |
| Bulk Density          | Soil bulk density                    | kg/m³       | SoilGrids            | 250m                    |
| Permeability          | Rock hydraulic permeability          | log(m²)     | GLHYMPS              | 1km                     |
| Aridity Index         | Long-term aridity measure            | unitless    | Calculated           | 0.25°                   |



### 🔍 Data Access Instructions for Reviewers
1. Download `baseflow_1979-2020.tiff` for spatial analysis
2. View `BaseflowIndia.gif` for temporal patterns
3. Consult `data_sources/` metadata for input references

## 🧪 Methodology
Baseflow estimation follows Xie et al. (2022) using LSTM-based modeling.  
Xie, J. et al. (2022). *Water Resources Research* 58(8). https://doi.org/10.1029/2022WR032833

## ⚖️ License
CC BY 4.0
