# 🌾 Crop Type & Land Cover Classification with LightGBM

> Pixel-level multiclass land cover classification using Sentinel-2 satellite imagery and LightGBM — bridging agricultural mapping with urban & regional planning.

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-Gradient%20Boosting-2F8A3A?style=for-the-badge&logo=leaflet&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML%20Toolkit-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Rasterio](https://img.shields.io/badge/Rasterio-Geospatial%20Raster-4B8BBE?style=for-the-badge&logo=qgis&logoColor=white)
![GeoPandas](https://img.shields.io/badge/GeoPandas-Vector%20Data-139C5A?style=for-the-badge&logo=pandas&logoColor=white)
![Sentinel-2](https://img.shields.io/badge/Sentinel--2-Satellite%20Imagery-1A73E8?style=for-the-badge&logo=satellite&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)
![Accuracy](https://img.shields.io/badge/Accuracy-89.35%25-brightgreen?style=for-the-badge)
![AUC](https://img.shields.io/badge/Macro--AUC-0.9043-blue?style=for-the-badge)

---

## 📌 Overview

This project classifies major crop types (Maize, Sugarcane, Sunflower, etc.) and broader land cover classes using **Sentinel-2 multispectral imagery** combined with **LightGBM**, a fast and efficient gradient boosting framework.

The workflow uses field-delineated training polygons, extracts spectral band values and indices at pixel level, and trains a multiclass classifier capable of producing spatially explicit land cover maps at scale.

---

## 🎯 Results

| Metric | Score |
|---|---|
| Overall Accuracy | **89.35%** |
| Macro-Averaged AUC | **0.9043** |

---

## 🛰️ Data

- **Imagery**: Sentinel-2 multispectral bands
- **Training Labels**: Field polygons digitized via QGIS / ArcGIS / JOSM
- **Feature Space**: Spectral bands + derived vegetation/spectral indices

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| `LightGBM` | Multiclass gradient boosting classifier |
| `rasterio` | Reading and writing raster data |
| `rasterstats` | Zonal statistics from raster + vector |
| `geopandas` | Vector data handling |
| `scikit-learn` | Train/test split, evaluation metrics |
| `Google Colab` | Training environment |

---

## 🚀 Why LightGBM for Remote Sensing?

- ✅ Very fast training even on large raster-derived datasets
- ✅ Strong performance on tabular satellite features (bands + indices)
- ✅ Native multiclass support — no complicated workarounds
- ✅ Built-in feature importance — interpretable band contributions
- ✅ Handles moderate class imbalance common in real land-cover data
- ✅ Scales well for classifying large geographic regions

---

## 🏙️ Planning Applications

Accurate crop and land cover maps serve as critical evidence for:

1. Identifying farmland to protect from urban expansion
2. Supporting land suitability analysis for new development
3. Mapping agricultural zones near cities for food-system planning
4. Monitoring conversion of farmland to built-up areas
5. Baseline data for infrastructure corridor alignment
6. Defining green belts and peri-urban buffers

---

## 📁 Repository Structure
```
crop-type-landcover-classification-lightgbm/
│
├── Code/LightGBM_for_Crop_Type_and_Land_Classification.ipynb
├── README.md
└── requirements.txt
```

---

## 🔧 Getting Started
```bash
# Clone the repository
git clone https://github.com/SHsabbir25/crop-type-landcover-classification-lightgbm.git
cd crop-type-landcover-classification-lightgbm

# Install dependencies
pip install rasterio rasterstats geopandas lightgbm scikit-learn matplotlib
```

Then open the notebook in **Google Colab** or **Jupyter** and follow the steps.

---

## 📬 Connect

If you work in urban planning, regional development, land-use policy, or geospatial analysis — I'd love to connect and discuss:
- How agricultural land classification fits into your planning workflows
- What data sources or methods you're using in 2025–2026

---

## 📄 License

MIT License
