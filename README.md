# Measuring Tree Canopy Height using SAR Interferometry (InSAR)

## Overview

This project presents an end-to-end SAR Interferometry (InSAR) workflow for estimating forest canopy height using Sentinel-1 C-band Synthetic Aperture Radar (SAR) data.

The work was carried out as part of a seminar project at the Indian Institute of Technology (IIT) Dharwad under the guidance of Dr. Shashaank Aswatha Mattur.

The project uses ESA SNAP, SNAPHU, and QGIS to generate Digital Surface Models (DSM) and Canopy Height Models (CHM) for dense forest regions around the IIT Dharwad campus.

---

## Objectives

- Understand the principles of SAR Interferometry (InSAR)
- Generate interferograms from Sentinel-1 SLC data
- Perform phase filtering and phase unwrapping
- Generate terrain-corrected Digital Surface Models (DSM)
- Compute Canopy Height Models (CHM) using DSM–DEM subtraction
- Analyze major sources of error in vegetation height estimation

---

## Workflow

The complete processing pipeline implemented in this project:

1. Sentinel-1 SLC Data Collection  
2. Co-registration  
3. Interferogram Formation  
4. TOPS Debursting  
5. Goldstein Phase Filtering  
6. Phase Unwrapping using SNAPHU  
7. Phase-to-Height Conversion  
8. Terrain Correction  
9. DSM Export  
10. CHM Generation in QGIS using DSM − DEM  

---

## Tools and Technologies

- ESA SNAP
- SNAPHU
- QGIS
- Sentinel-1 SAR Data
- OpenTopography DEM
- Remote Sensing
- SAR Interferometry (InSAR)

---

## Study Area

- IIT Dharwad Forest Region
- Dense tropical vegetation area used for canopy height estimation experiments

---

## Results

The complete InSAR processing workflow was successfully implemented and terrain-corrected DSMs were generated from Sentinel-1 SLC data.

Generated outputs include:
- Interferograms
- Unwrapped phase maps
- Digital Surface Models (DSM)
- Canopy Height Models (CHM)

The obtained canopy heights showed systematic overestimation:
- Expected canopy height: 16–20 m
- Obtained canopy height: 60–80 m

### Major Causes of Error
- Low coherence in dense vegetation regions
- Phase unwrapping errors
- DEM bias and raster misalignment
- C-band volume decorrelation effects

---

## Repository Structure

text ├── images/ │   ├── workflow.png │   ├── chm_result.png │   ├── interferogram.png │   └── phase_unwrap.png │ ├── report.pdf ├── presentation.pdf ├── workflow_steps.md ├── future_work.md └── README.md 

---

## Future Improvements

Potential improvements for achieving more accurate canopy height estimation:

- Multi-temporal InSAR stacking
- Integration with GEDI / ICESat-2 LiDAR data
- Sentinel-2 NDVI-based forest masking
- L-band SAR analysis (e.g., ALOS-2)
- Automated raster processing using Python, GDAL, and Rasterio
- Validation using ground truth measurements

---

## References

- ESA SNAP Documentation  
- SNAPHU Documentation  
- Sentinel-1 SAR Data (Copernicus Open Access Hub)  
- OpenTopography DEM  
- Global Canopy Height 2020 Dataset  

---

## Author

Abhinav Singh  
M.Tech, Electrical Engineering  
Indian Institute of Technology Dharwad
