# Delhi NO₂ Pollution Mapping

This project visualizes NO₂ column density over Delhi using satellite data and GeoTIFF processing. It extracts NO₂ values for specified locations and plots a heatmap of NO₂ concentration.

---

## Features

- Loads NO₂ data from Sentinel-5P (TROPOMI) GeoTIFF files
- Extracts NO₂ values for given latitude and longitude points (e.g., Delhi monitoring stations)
- Generates a heatmap of NO₂ concentrations
- Saves results to CSV for further analysis

---

##  Project Structure

PollutionController/
├── delhi_no2_2019.tif # Input GeoTIFF file (NO₂ data)
├── stations.csv # CSV file with station names and coordinates
├── extract_no2.py # Python script to extract NO₂ values
├── plot_no2.py # Python script to plot heatmap
├── README.md # Project description
└── screenshot.png # Sample heatmap screenshot

yaml
Copy
Edit

---

##  Screenshot

![NO₂ Heatmap](screenshot.png)

---

##  How to Run

1. **Install Dependencies**  
   ```bash
   pip install rasterio geopandas pandas matplotlib
Run Extraction Script

bash
Copy
Edit
python extract_no2.py
Run Plot Script

bash
Copy
Edit
python plot_no2.py
Check Output

no2_values.csv: NO₂ values at station locations

no2_heatmap.png: Heatmap of NO₂ concentration

 Data Sources
Sentinel-5P TROPOMI NO₂

 Dependencies
Python 3.8+

rasterio

geopandas

pandas

matplotlib

 Author
Sagnik Patra
