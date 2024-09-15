
# Analysis of Avalanche Hazard in South Tyrol

This repository contains the Python code, Jupyter notebooks, and related data for the analysis and evaluation of the existing avalanche cadastre in South Tyrol through hazard mapping and simulations. The project was developed as part of a bachelor’s thesis at the University of Graz, Faculty of Environmental, Regional, and Educational Sciences, Department of Geography and Regional Research.

## Project Overview

In this project, potential avalanche release areas (PRAs) are identified and evaluated based on geomorphological parameters such as slope, terrain roughness, wind shelter, and forest cover. Historical avalanche data is used to validate the results of the hazard mapping, and simulations were performed using RAMMS (Rapid Mass Movements Simulation) to compare with historical events.

## Structure of the Repository

The repository contains the following directories and files:

- `/notebooks`: Jupyter notebooks used for data processing, PRA identification, and simulation preparation.
- `/data`: Geographical data files such as DEM (Digital Elevation Model) and PRA shapefiles.
- `/scripts`: Python scripts for preprocessing, terrain analysis, and visualization of avalanche hazard zones.
- `/outputs`: Results of simulations and visualizations of hazard mapping.
  
## Main Files

- `PRA_Berechnung_Franzelin.ipynb`: This notebook contains the core calculations and method implementation for PRA analysis.
- `PRA_Vergleich.ipynb`: This notebook compares the PRA analysis with different Values to find the best.
- `Franzelin_Bachelor_Signed.pdf`: The final thesis document, which provides detailed information about the project’s background, methodology, and results.

## Methodology

1. **Data Collection**: The initial step involves collecting historical avalanche data and geographical features like slope, roughness, wind shelter, and forest cover.
2. **PRA Identification**: Using threshold values for the various geomorphological parameters, potential avalanche release areas (PRAs) are identified.
3. **Simulation**: RAMMS is used to simulate potential avalanche paths, comparing the results to historical avalanche data for validation.
4. **Evaluation**: The accuracy of the PRA model is evaluated against recorded avalanche events, and discrepancies are analyzed to improve the model.

## Requirements

- Python 3.9
- Jupyter Notebook
- GeoPandas
- NumPy
- GDAL
- RAMMS (for simulation)

## Digital Terrain Model (DTM) Usage

This project requires a Digital Terrain Model (DTM) dataset for analysis. You can download the DTM from the **South Tyrol Geoportal**. Please follow the steps below to acquire and use the dataset in this project:

### Downloading the DEM:

1. **Access the Geoportal**:
   - Visit the official South Tyrol Geoportal at [geoportal.buergernetz.bz.it](http://geokatalog.buergernetz.bz.it/geokatalog/#!).

2. **Locate the DEM Dataset**:
   - Use the search bar or navigate through the available layers to find the **Digital Elevation Model (DEM)** data.
   - Choose the appropriate resolution and format (such as GeoTIFF or another format compatible with this project).

3. **Download the Dataset**:
   - Click on the download button provided by the geoportal and save the DTM file to your local system.

## Installation

To get started, clone the repository and set up a virtual environment:

```bash
git clone https://github.com/username/avalanche_hazard_south_tyrol.git
cd avalanche_hazard_south_tyrol
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
pip install -r requirements.txt
```

## Usage

1. Start Jupyter Notebook and open the relevant notebooks in the `/notebooks` directory.
2. Ensure that you have the required data files in the `/data` directory.
3. Run the PRA analysis and hazard simulations.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Jean Patrick Franzelin  
Bachelor of Science in Geography  
University of Graz  
2024

