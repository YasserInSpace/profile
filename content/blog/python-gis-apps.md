---
title: "Building GIS Web Apps with Python"
date: 2026-04-06
summary: "A practical walkthrough on deploying geospatial analytics dashboards using Python, Streamlit, and Leaflet."
tags: ["Python", "Web GIS", "Streamlit"]
---

Creating powerful spatial analysis scripts in Jupyter Notebooks is great, but sharing those insights with non-technical stakeholders requires an intuitive interface. Python makes it incredibly easy to bridge this gap.

### The Tech Stack
- **Backend/Logic:** `Geopandas` for vector operations, `Rasterio` for image processing.
- **Frontend/UI:** `Streamlit` allows us to build interactive web apps with pure Python.
- **Mapping:** `Folium` (built on Leaflet.js) integrates seamlessly with Streamlit to display interactive maps.

### A Simple Workflow
Instead of building a complex React/Django application, a Streamlit app can be stood up in hours. You define your map UI, add interactive sliders (e.g., for filtering earthquake magnitudes or adjusting flood probability thresholds), and deploy it instantly. 

This approach was instrumental in developing the multi-hazard risk mapping platform for Côte d'Ivoire, allowing decision-makers to interact dynamically with the data without needing desktop GIS software.
