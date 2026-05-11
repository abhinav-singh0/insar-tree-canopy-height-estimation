# 🌍 Measuring Tree Canopy Height using SAR Interferometry (InSAR)

> End-to-end forest canopy height estimation using Sentinel-1 SAR data, ESA SNAP, SNAPHU, and QGIS.

---

## 📌 Project Overview

This project implements a complete SAR Interferometry (InSAR) workflow for estimating forest canopy height from Sentinel-1 C-band Synthetic Aperture Radar (SAR) data.

The work was carried out as part of a seminar project at the Indian Institute of Technology (IIT) Dharwad under the guidance of Dr. Shashaank Aswatha Mattur.

Using ESA SNAP, SNAPHU, and QGIS, the project generates:
- Interferograms
- Unwrapped phase maps
- Digital Surface Models (DSM)
- Canopy Height Models (CHM)

for dense tropical vegetation regions around the IIT Dharwad campus.

---

## 🎯 Objectives

- Understand the fundamentals of SAR Interferometry (InSAR)
- Process Sentinel-1 SLC data for terrain and vegetation analysis
- Generate interferograms and perform phase unwrapping
- Create terrain-corrected DSM products
- Compute Canopy Height Models (CHM) using DSM–DEM subtraction
- Analyze coherence degradation and vegetation-induced phase errors

---

## 🛰️ Dataset and Study Area

### Study Area
- IIT Dharwad Forest Region
- Dense tropical vegetation zone

### Datasets Used
- Sentinel-1 Level-1 SLC Data
- OpenTopography DEM
- Global Canopy Height 2020 Dataset

---

## ⚙️ Processing Workflow

The following InSAR processing pipeline was implemented:

text Sentinel-1 SLC Data         ↓ Coregistration         ↓ Interferogram Formation         ↓ TOPS Debursting         ↓ Goldstein Phase Filtering         ↓ Phase Unwrapping (SNAPHU)         ↓ Phase-to-Height Conversion         ↓ Terrain Correction         ↓ DSM Generation         ↓ CHM = DSM − DEM (QGIS) 

---

## 🛠️ Tools and Technologies

- ESA SNAP
- SNAPHU
- QGIS
- Sentinel-1 SAR
- Remote Sensing
- SAR Interferometry (InSAR)
- Geospatial Analysis

---

## 📊 Results

The complete InSAR workflow was successfully implemented and terrain-corrected DSMs were generated from Sentinel-1 SAR imagery.

### Generated Outputs
- Interferograms
- Unwrapped phase maps
- Digital Surface Models (DSM)
- Canopy Height Models (CHM)

### Observed Canopy Height

| Region | Expected Height | Obtained Height |
|---|---|---|
| IIT Dharwad AOI | 16–20 m | 60–80 m |

---

## ⚠️ Challenges and Error Analysis

The obtained canopy heights showed systematic overestimation due to:

- Low coherence in dense vegetation regions
- Phase unwrapping errors
- DEM bias and raster misalignment
- C-band volume decorrelation
- Geometric distortions in SAR imagery

This project also highlights the practical challenges involved in vegetation height estimation using C-band SAR data.

---

## 🚀 Future Improvements

Potential improvements for achieving more accurate canopy height estimation:

- Multi-temporal InSAR stacking
- Integration with GEDI / ICESat-2 LiDAR data
- Sentinel-2 NDVI-based vegetation masking
- L-band SAR analysis (e.g., ALOS-2)
- Automated raster processing using Python and GDAL
- Ground truth validation using field measurements

---

## 📂 Repository Structure

text ├── images/ │   ├── workflow.png │   ├── chm_result.png │   ├── interferogram.png │   └── phase_unwrap.png │ ├── report.pdf ├── presentation.pdf ├── workflow_steps.md ├── future_work.md └── README.md 

---

## 📚 References

- ESA SNAP Documentation
- SNAPHU Documentation
- Sentinel-1 SAR Data (Copernicus Open Access Hub)
- OpenTopography DEM
- Global Canopy Height 2020 Dataset

---

## 👨‍💻 Author

Abhinav Singh  
M.Tech, Electrical Engineering  
Indian Institute of Technology Dharwad  

### Project Supervisor
**Dr. Shashaank Aswatha Mattur
