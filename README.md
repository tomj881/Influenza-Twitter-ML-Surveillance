# Influenza-Twitter-ML-Surveillance
Final MSc research project that leverages machine learning and spatiotemporal analysis to detect influenza outbreaks using Twitter data. Combines NLP, classification models, and geolocation clustering to support real-time digital disease surveillance.

# 🦠 Twitter-Based Influenza Outbreak Prediction

---

## 📌 Project Overview

This research project explores the use of **machine learning and geospatial analysis** to detect influenza outbreaks using data sourced from Twitter. Traditional flu surveillance systems are slow and geographically limited. In contrast, Twitter provides real-time, location-rich data that can enhance public health monitoring through digital epidemiology.

This project demonstrates a pipeline that:
- **Classifies flu-related tweets**
- **Clusters geolocation data** to spot potential outbreak zones
- Compares the performance of five ML models
- Supports early warning systems for health agencies

---

## 🎯 Objectives

- 🧹 Preprocess Twitter text data (cleaning, tokenization, etc.)
- 🧠 Train and evaluate ML models for classification
- 🌍 Use geolocation clustering (DBSCAN/K-Means) to detect outbreak areas
- 📊 Visualize patterns and model performance
- ⚕️ Support real-time digital surveillance for influenza

---

## 🗃️ Dataset

**Title:** [Influenza Outbreak Event Prediction via Twitter – UCI ML Repository](https://archive.ics.uci.edu/dataset/861/influenza+outbreak+event+prediction+via+twitter)  
**Source:** University of California, Irvine  
**Format:** `.mat` (MATLAB)  
**Size:** 3,574 tweets  
**Features:**
- Tweet text
- Location (latitude/longitude)
- Keywords
- Severity levels
- Timestamps

**License:** For research and educational use only.

---

## 🧪 Models Used

The following supervised classification models were trained and evaluated:

- ✅ Random Forest (Best performer)
- XGBoost
- LightGBM
- CatBoost
- AdaBoost

**Evaluation Metrics:**
| Metric     | Random Forest |
|------------|----------------|
| Accuracy   | 0.804          |
| F1-Score   | 0.1967         |
| AUC-ROC    | 0.5738         |
| Recall     | ~0.12          |

*Note: All models exhibited low recall, highlighting challenges in detecting minority (flu-positive) cases.*

---

## 🌍 Spatiotemporal Analysis

To detect flu outbreak clusters:
- Tweets with latitude and longitude were extracted
- Clustering algorithms applied:
  - **DBSCAN** for density-based outbreak detection
  - **K-Means** for general spatial grouping
- Outputs included radar plots, keyword treemaps, word clouds, and cluster visualizations

This analysis identified **potential outbreak zones** based on high tweet density and flu severity.

---

## 📁 Project Structure

