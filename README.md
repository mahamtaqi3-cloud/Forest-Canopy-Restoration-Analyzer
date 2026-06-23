# Forest Canopy Restoration Analysis

An end-to-end remote sensing project designed to monitor forest canopy health and identify priority zones for ecological restoration using satellite imagery.

## 🚀 Project Overview

This project leverages satellite data to calculate the **Normalized Difference Vegetation Index (NDVI)**, a standard ecological metric for assessing plant health. By analyzing Near-Infrared (NIR) and Red spectral bands, the project creates visual health maps that distinguish between dense forest canopy and degraded or open land.

## 📊 Key Features

* **Satellite Data Integration**: Connects directly to the Microsoft Planetary Computer to fetch real-time Sentinel-2 imagery.
* **NDVI Analysis**: Implements the standard formula $NDVI = \frac{(NIR - Red)}{(NIR + Red)}$ to quantify vegetation density.
* **Restoration Mapping**: Generates spatial visualizations that highlight "Low Health" zones (NDVI < 0.3) as potential targets for reforestation efforts.
* **Health Profiling**: Includes statistical histograms to visualize the health distribution of specific forest patches.

## 🛠 Tech Stack

* **Platform**: [Google Colab](https://colab.research.google.com/)
* **Language**: Python 3
* **Libraries**:
* `pystac-client` & `odc-stac`: For cloud-native satellite data access.
* `planetary-computer`: For authenticating and signing data requests.
* `matplotlib` & `numpy`: For scientific visualization and matrix manipulation.



## 📈 Visual Analysis

*(Once you have saved your map as `restoration_map.png`, upload it to your GitHub repository and uncomment the line below)*

## 💡 How to Use

1. Open the `.ipynb` file in **Google Colab**.
2. Ensure you have your own Microsoft Planetary Computer API key if required (or use the default environment settings).
3. Adjust the `bbox` (bounding box) coordinates in the second cell to analyze your area of interest.
4. Run the cells sequentially to fetch data, compute the NDVI, and generate the health maps.

## 🤝 Contributions

This project is open-source and intended to support environmental monitoring. Feel free to fork this repository, submit issues, or suggest improvements for time-series analysis or automated cloud masking!

---

