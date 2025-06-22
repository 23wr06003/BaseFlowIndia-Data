# BaseFlowIndia-Data: Supplementary Data for Baseflow Simulation in Central and South India (1979-2020)

## 🎥 Baseflow Animation (1979-2020)
![Monthly Baseflow Simulation](https://raw.githubusercontent.com/23wr06003/BaseFlowIndia-Data/main/BaseflowIndia.gif)  
*Visualization of monthly baseflow patterns across Central and South India*

## 📄 Purpose
This repository contains supplementary data for the manuscript:
**"Estimating Gridded Monthly Baseflow across Central and Southern India"**  
submitted to the *Journal of Hydrology*. It includes:
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
| Dataset                  | Source                                             | Resolution | Period      |
|--------------------------|---------------------------------------------------|------------|-------------|
| Precipitation            | IMD Gridded Rainfall Data                         | 0.25°      | 1979-2020   |
| Temperature              | IMD Gridded Temperature Data                      | 1.0°       | 1979-2020   |
| GRACE Terrestrial Water | NASA JPL Mascons                                  | 0.5°       | 2002-2020   |
| Soil Moisture            | GLDAS NOAH Model                                  | 0.25°      | 1979-2020   |
| *[Add others]*           |                                                   |            |             |

## 🧪 Methodology
### Baseflow Estimation Workflow
1. **Hydrological Modeling**:  
   LSTM-based architecture adapted from Xie et al. (2022)
2. **Parameterization**:  
   Region-specific calibration using observed streamflow data
3. **Baseflow Separation**:  
   Digital filter applied to total runoff simulations
4. **Validation**:  
   Comparison against ground-truth baseflow estimates

**Reference**:  
Xie, J., Liu, X., Bai, P., & Liu, C. (2022). Estimating Gridded Monthly Baseflow Using GRACE/GRACE-FO and Machine Learning. *Water Resources Research*, 58(8). https://doi.org/10.1029/2022WR032833

## ⚖️ License
This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).  
When using this data, please cite:  
*[Your Full Paper Title]. Journal of Hydrology (Under Review).*

---

### 🔍 Data Access Instructions for Reviewers
1. Download `baseflow_1979-2020.tiff` for spatial analysis
2. View `BaseflowIndia.gif` for temporal patterns
3. Consult `data_sources/` metadata for input references

## 🧪 Methodology
Baseflow estimation follows Xie et al. (2022) using LSTM-based modeling.  
**Reference**:  
Xie, J. et al. (2022). *Water Resources Research* 58(8). https://doi.org/10.1029/2022WR032833

## ⚖️ License
CC BY 4.0
