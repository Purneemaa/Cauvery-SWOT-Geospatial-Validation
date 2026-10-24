# Cauvery-SWOT-Geospatial-Validation
Reproducible SWOT WSE and multi-sensor river validation workflows for the Cauvery River Basin
1. Dataset Overview

This repository contains processed Surface Water and Ocean Topography (SWOT) satellite observations and associated validation results for selected reaches of the Cauvery River Basin, India, during 2024–2025.
The dataset supports the assessment of satellite-derived water surface elevation (WSE), river width, and hydrological variability using remote sensing and available ground-based observations.

2. Study Area

The study focuses on selected monitoring locations along the Cauvery River Basin, including:

- Biligundulu
- Urachikottai
- Kodumudi
- Musiri

Data availability and spatial coverage vary between monitoring locations.

3. Data Sources

SWOT satellite observations

- Mission: Surface Water and Ocean Topography (SWOT)
- Product: Level-2 High-Rate River Single-Pass (RiverSP)
- Product version: Version D
- Data provider: NASA PO.DAAC
- Study period: 2024–2025

Additional observations

Where applicable, Sentinel-1 SAR, Sentinel-2 optical imagery, and in-situ hydrological observations were used for comparison and validation.

4. Data Processing

SWOT RiverSP observations were extracted for selected monitoring locations and organised by acquisition date and spatial identifier.

Quality filtering was performed using the available product quality indicators:

- Water surface elevation: `wse_sm_q ≤ 1`
- River width: `node_q ≤ 1`

Station-specific extraction procedures were applied according to the spatial characteristics of each location. Urachikottai was analysed using a single SWOT node rather than a reach-averaged measurement.

5. Validation Methodology

Where reference observations were available, satellite-derived measurements were matched with corresponding in-situ observations.

Statistical performance was assessed using:

- Coefficient of determination (R²)
- Root mean square error (RMSE)
- Mean bias error

The validation procedures were implemented using Python.

6. Software and Processing Environment

The following tools were used during the research:

- Python for data processing, statistical analysis, and visualisation
- Anaconda for managing the Python computing environment
- Google Earth Engine for processing satellite imagery and extracting geospatial information

The associated scripts should be consulted for implementation details where provided.

7. Dataset Contents

The repository contains processed geospatial and hydrological observations, validation results, and associated documentation.

Users should consult the accompanying data dictionary for column definitions, measurement units, quality indicators, and missing-value conventions.

8. Data Limitations

SWOT observations are subject to satellite acquisition frequency, spatial coverage, retrieval uncertainty, and quality-control restrictions.

Temporal matching with in-situ observations may be affected by differences in observation times and data availability.

The dataset should therefore be interpreted with consideration of station-specific conditions and the limitations of satellite-based hydrological measurements.

9. Data Availability

The processed research dataset is deposited in Mendeley Data.

