---
title: "How Flood Detection Works Using SAR Data"
date: 2026-04-13
summary: "Exploring Synthetic Aperture Radar (SAR) to monitor flood events globally, bypassing cloud cover constraints."
tags: ["SAR", "Flood Detection", "Sentinel-1"]
---

When a disaster like a flood strikes, the skies are often obscured by thick clouds. This renders traditional optical satellites virtually useless. Enter **Synthetic Aperture Radar (SAR)**.

### Why SAR?
SAR sensors, like those on Sentinel-1, transmit microwave signals that penetrate clouds and operate day or night. When these waves hit calm water, they bounce away from the sensor (specular reflection), making flooded areas appear dark in the resulting imagery.

### The Methodology
1. **Acquisition:** Download Sentinel-1 GRD imagery before and during the flood event.
2. **Preprocessing:** Apply precise orbit files, remove thermal noise, and perform radiometric calibration and terrain correction.
3. **Thresholding & Change Detection:** By comparing the backscatter values of the 'before' and 'after' images, we can isolate pixels that changed from bright (rough land) to dark (smooth water).

This methodology is at the core of the Flood Management System we implemented in Senegal, providing near-real-time actionable insights to first responders.
