# ClimaGuard
## Overview
<img width="1906" height="908" alt="image" src="https://github.com/user-attachments/assets/cbda8028-2c27-4823-a361-e865654f1178" />
ClimaGuard is a web application. It utilizes satellite data and machine learning to monitor, predict, and analyze environmental pollution — especially industrial air pollution — in real-time. The platform is designed to provide transparency, promote sustainable practices, and enable data-driven policy interventions.

## Project Goals
The primary goals of ClimaGuard are:

- Industrial Pollution Monitoring: Enable scalable, real-time tracking of industrial emissions across India using remote sensing and ML.
- Predictive Analytics: Use time-series forecasting models like LSTM to predict pollution levels, aiding early interventions.
- Actionable Insights for Stakeholders: Offer interpretable dashboards for governments, industries, and the public to track pollution patterns and risk zones.
- Environmental Impact Assessment: Use NDVI (Normalized Difference Vegetation Index) to assess pollution's effect on surrounding ecosystems.

## Key Features
ClimaGuard incorporates the following core features:
<img width="1918" height="909" alt="image" src="https://github.com/user-attachments/assets/af026f75-9937-4a5c-9e4e-829102074f6a" />
<img width="1919" height="914" alt="image" src="https://github.com/user-attachments/assets/4f20d5f3-90e1-477d-b2b1-1f0be097ba2e" />
<img width="1919" height="917" alt="image" src="https://github.com/user-attachments/assets/950c6448-1452-4eb5-ac87-78ef6eb286d3" />
<img width="1919" height="907" alt="image" src="https://github.com/user-attachments/assets/67e7ea8f-8108-46d0-b3a1-55f4f36591ae" />

- Multi-Pollutant Monitoring: Tracks 8 critical pollutants — CO, NO, NO₂, SO₂, O₃, PM2.5, PM10, and NH₃ — using satellite and sensor fusion.
- Time-Series Forecasting: LSTM models predict pollutant levels up to 4 days in advance with an 85% accuracy rate.
- Anomaly Detection: Random Forest and Isolation Forest models flag unusual pollution spikes.
- Hotspot Clustering: K-Means identifies high-risk pollution zones; clustering insights guide mitigation efforts.
- Real-Time Dashboard: Interactive heatmaps, trend graphs, and AQI tables updated every minute.
- User-Centric Mapping: Leaflet-based maps enable location-aware queries and overlay toggles for AQI, wind, temperature, and vegetation layers.

## System Architecture
The platform is built on a layered architecture:

1. Data Acquisition Layer: Satellite imagery and APIs for weather and pollution data (NO₂, PM2.5, SO₂, O₃, etc.).
2. Processing & Analytics Layer:
  - LSTM for pollutant forecasting
  - Random Forest for anomaly detection
  - K-Means Clustering for identifying pollution clusters
  - NDVI for environmental degradation analysis
3. Visualization Layer: Real-time dashboards with interactive maps and visual summaries for stakeholder decisions.

## Machine Learning Models
- LSTM: Achieved 87.7% classification accuracy across multiple pollutants (PM10, NO₂, SO₂, etc.)
- Random Forest & Isolation Forest: Used for anomaly detection across pollutants
- K-Means: Clustered 60 industries of 4 types (Cement, Tannery, Steel and Power Plant) into distinct zones based on pollution severity

## Technology Stack
- Frontend: HTML, CSS, JavaScript (Leaflet.js, Chart.js, ApexCharts)
- Backend: Python (Django)
- ML/AI: TensorFlow/Keras for LSTM, Scikit-learn for clustering and classification
- Visualization: Real-time dashboards with geospatial overlays

## Open Source APIs Used
This project makes extensive use of the following open-source APIs and datasets:

- OpenWeatherMap API – Real-time weather and temperature data.
- WAQI (World Air Quality Index) API – Real-time AQI and pollutant concentration data.
- Sentinel (ESA Copernicus) – Satellite imagery for pollutant and NO₂ tracking.
- Geoapify API – Geocoding, map tiles, and place search functionality.
- Google Gemini API – AI-based response generation for summarizing and interpreting results.

## Comparative Advantage
- Broader Pollutant Range: Covers 8+ pollutants and vegetation metrics
- Real-Time + Historical Insights: Merges current data with 20-year trends
- Low Latency: < 1 minute for most updates
- Public Transparency: Data accessible via a user-friendly, responsive interface
- Scalability: Adaptable for national-scale deployments and various industries

## Future Enhancements
Potential future developments for SatIndustry include:

- Advanced Analytics: Implementing more sophisticated AI/ML models for predictive environmental analysis and anomaly detection.
- Expanded Data Layers: Integrating additional environmental datasets, such as water quality indices, deforestation rates, and biodiversity metrics.
- User Accounts and Personalization: Adding user accounts to enable personalized dashboards, saved locations, and custom data alerts.
- Algorithm Optimization to reduce computational costs
