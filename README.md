# Climate Change Impacts on Streamflow and Hydrological Extremes

## South Phuthiatsana Catchment, Lesotho

**MSc Research Project | National University of Lesotho | 2025**

This study assessed the impacts of climate change on streamflow dynamics and hydrological extremes in the South Phuthiatsana Catchment, Lesotho, using a hybrid modelling framework combining **SWAT+ hydrological modelling** and **Extreme Gradient Boosting (XGBoost)** with **CMIP6 climate projections**.

The research evaluated historical hydro-climatic variability and projected future changes in precipitation, temperature, streamflow, and hydrological extremes under the **SSP2-4.5** and **SSP5-8.5** scenarios.

**Keywords:** Hydrological Modelling · Climate Change · XGBoost · SWAT+ · CMIP6 · Streamflow · Hydrological Extremes · Lesotho


---

## Research Context

The South Phuthiatsana Catchment is an important water-resource system in Lesotho, with the South Phuthiatsana River serving as a perennial tributary of the Mohokare (Caledon) River within the Orange-Senqu River Basin.

Climate variability and long-term climate change can alter precipitation, temperature, streamflow regimes, and the occurrence of hydrological extremes. Understanding these changes is important for supporting long-term water-resources planning and climate adaptation in the catchment.

This research therefore investigated historical hydro-climatic variability and assessed potential future changes in streamflow and hydrological extremes under different climate-change scenarios.

---

## Research Objectives

The study aimed to:

1. Assess historical trends and variability in precipitation, temperature, and streamflow in the South Phuthiatsana Catchment.

2. Evaluate the performance of the SWAT+ hydrological model in simulating historical streamflow.

3. Develop and evaluate an XGBoost machine-learning model for streamflow simulation.

4. Assess projected changes in precipitation and temperature under the SSP2-4.5 and SSP5-8.5 climate scenarios.

5. Simulate future streamflow using bias-corrected climate projections.

6. Assess potential changes in high-flow and low-flow characteristics and other hydrological extremes under future climate conditions.


---

## Study Area

### South Phuthiatsana Catchment, Lesotho

The study was conducted in the South Phuthiatsana Catchment in Lesotho. The
catchment was delineated to the **Masianokeng gauging station** and covers
approximately **651.7 km²**.

The catchment extends between approximately **29°12′50″ and 29°37′50″ S**
latitude and **27°25′5″ and 28°2′5″ E** longitude, with elevations ranging
from approximately **1,560 to 3,010 m above sea level**.

The South Phuthiatsana River is a perennial river originating in the
highlands of the Berea District. It flows through parts of Maseru before
joining the **Mohokare (Caledon) River**, which forms part of the
**Orange-Senqu River Basin**.

The catchment is characterised by a mixture of grassland, cropland and
tree-covered areas. The study area has an average annual precipitation of
approximately **690.7 mm** and average annual evapotranspiration of
approximately **402.3 mm**.

### Catchment Characteristics

| Characteristic | Description |
|---|---|
| Location | Lesotho |
| Catchment area | ~651.7 km² |
| Outlet | Masianokeng gauging station |
| Elevation range | ~1,560–3,010 m a.s.l. |
| River | South Phuthiatsana |
| Receiving river | Mohokare (Caledon) River |
| River basin | Orange-Senqu River Basin |
| Mean annual precipitation | ~690.7 mm |
| Mean annual evapotranspiration | ~402.3 mm |
| Dominant land cover | Grassland, cropland and trees |


<img width="753" height="396" alt="image" src="https://github.com/user-attachments/assets/a27cde55-a959-4808-b8cb-59e01732ad8a" />


---

## Data and Datasets

The study integrated topographic, land-cover, soil, meteorological, hydrological and climate-model datasets to develop and evaluate the hydrological modelling and climate-impact assessment framework.

### Summary of datasets

| Dataset | Variable / Purpose | Spatial / Temporal Resolution | Role in the Study |
|---|---|---|---|
| SRTM DEM | Elevation and terrain characteristics | 30 m | Catchment delineation and SWAT+ terrain preprocessing |
| Land-cover data | Land-use/land-cover classification | 10 m | SWAT+ land-cover parameterisation |
| Soil data | Soil properties | 250 m | SWAT+ soil parameterisation |
| Meteorological observations | Precipitation and temperature | Daily | Historical model forcing and analysis |
| Streamflow observations | River discharge | Daily | Model calibration, validation and evaluation |
| CMIP6 climate projections | Future climate variables | Model-dependent | Climate-change projections |
| MPI-ESM1-2-LR | Climate model | Model-dependent | Future climate forcing |
| SSP2-4.5 | Future emissions scenario | — | Intermediate climate-change scenario |
| SSP5-8.5 | Future emissions scenario | — | High-emissions climate-change scenario |

### Historical Hydro-Climatic Data

Historical precipitation and temperature data were used to characterise hydro-climatic variability and provide meteorological forcing for the hydrological modelling framework.

Observed daily streamflow data were used to evaluate the ability of the modelling approaches to reproduce historical streamflow dynamics.

### Climate Projection Data

Future climate conditions were assessed using CMIP6 climate projections under the **SSP2-4.5** and **SSP5-8.5** scenarios.

The climate projections were processed and bias-corrected before being used as inputs for future streamflow assessment.

The **MPI-ESM1-2-LR** climate model was used in the climate-impact assessment, providing future climate information for the selected scenarios.


---

## Methodology

The study adopted a hybrid modelling framework combining a process-based
hydrological model with a data-driven machine-learning approach to assess
climate-change impacts on streamflow and hydrological extremes.

The overall workflow consisted of:

1. Historical hydro-climatic data preparation and analysis.
2. Catchment delineation and hydrological model setup.
3. SWAT+ model calibration and evaluation.
4. XGBoost model development and evaluation.
5. Climate-model selection and bias correction.
6. Future climate projection under SSP2-4.5 and SSP5-8.5.
7. Future streamflow prediction.
8. Analysis of changes in hydrological extremes.

### Modelling Framework

```text
Historical Climate Data + Observed Streamflow
                    │
                    ▼
          Data Preparation & Analysis
                    │
                    ▼
             ┌───────────────┐
             │     SWAT+     │
             │ Process-based │
             │    model      │
             └───────┬───────┘
                     │
                     ▼
              Model Evaluation
                     │
             ┌───────┴───────┐
             │               │
             ▼               ▼
        SWAT+ Results    XGBoost Model
                             │
                             ▼
                    Model Evaluation
                             │
                             ▼
                  Best-performing approach
                             │
                             ▼
              Bias-corrected CMIP6 Climate Data
                             │
                  ┌──────────┴──────────┐
                  ▼                     ▼
              SSP2-4.5              SSP5-8.5
                  │                     │
                  └──────────┬──────────┘
                             ▼
                   Future Streamflow
                             │
                             ▼
                 Hydrological Extremes







