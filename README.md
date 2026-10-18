# NISAR GCOV X-TRACTOR

> **A RAM-Optimized Desktop Extraction & Calibration Tool for NASA-ISRO SAR (NISAR) Level-2 GCOV Products.**

[![License: Non-Commercial](https://img.shields.io/badge/License-Non--Commercial-red.svg)](LICENSE)
[![Platform: Windows 64-bit](https://img.shields.io/badge/Platform-Windows_64--bit-blue.svg)](https://github.com/YOUR_USERNAME/NISAR_GCOV_X-TRACTOR/releases/latest)
[![Release: Free Download](https://img.shields.io/badge/Download-Standalone_.exe-brightgreen.svg)](https://github.com/YOUR_USERNAME/NISAR_GCOV_X-TRACTOR/releases/latest)

---

## Download Standalone Tool (Free)

No installation, Python, or Conda required! Download the pre-compiled executable and run it immediately on any Windows PC:

👉 **[Download NISAR_X_TRACTOR.exe (Latest Version)](https://github.com/pdbarma/NISAR-GCOV-XTRACTOR/releases/latest)**

*Free for personal, academic, and scientific research use.*

---

> [!NOTE]
> **Work-in-Progress**: This application is under active development. Community suggestions, bug reports, and feature requests are warmly welcomed to help improve performance, usability, and radar workflows!

---

## How It Works (Visual Workflow)

![Flowchart](assets/mermaid-diagram.svg)

---

## Step-by-Step Visual Guide

### Step 1: Select Input File & Output Directory
Select your downloaded NISAR `.h5` file and destination folder. The software dynamically inspects the file, identifying the instrument (L-Band or S-Band), frequency grids, and UTM projection.

```text
[ Input H5 File ]    ──► Browse and select NISAR_L2_PR_GCOV_...h5
[ Output Folder ]    ──► Select where to save output files
[ Target ROI Name ]  ──► Enter a region name (e.g., Dehradun_Study)
```

> *Tip: Look at the status banner at the top to confirm your detected radar instrument and available polarizations.*

---

### Step 2: Draw Your Region on the Interactive Map
Click **"Open Interactive Web Map & Draw ROI"** to view the scene footprint overlaid on satellite imagery.

```text

Interactive Swath Map

[Red Boundary]  ──► Full Satellite Scene Footprint
1st Click       ──► Top-Left Corner of your study area
2nd Click       ──► Bottom-Right Corner
[Blue Box]      ──► Selected Sub-Region (Auto-saved to UI)

```

---

### Step 3: Choose Your Processing Pipeline

| Pipeline | Output Format | Ideal For |
| :--- | :--- | :--- |
| **GeoTIFF Rasters** | `.tif` (Linear & dB) | GIS mapping in QGIS, ArcGIS, ENVI, and statistical classification |
| **HDF5 (GCOV Subset)** | Lightweight `.h5` | Scientific SAR processing, InSAR, and **ESA SNAP** workflows |
| **Pauli Decomposition** | 3-band RGB `.tif` | Polarimetric scattering analysis (Double bounce, Volume, Surface) |

---

### Step 4: Click Start & Relax!
Click **`🚀 START NISAR EXTRACTION PROCESS`**.  
The engine slices only the target pixels directly from disk using low RAM (~15 MB). Within seconds, your analysis-ready files are generated!

---

## Why Use NISAR GCOV X-TRACTOR?

- **Potato-PC Friendly:** Smoothly extracts subsets from massive 10–15 GB scenes without running out of RAM or freezing your computer.
- **Full Scientific Metadata:** Keeps all satellite orbit vectors, attitude quaternions, and calibration matrices intact in HDF5 subsets.
- **ESA SNAP Compatible:** Corrects internal dimension scales so ESA SNAP opens the subsetted `.h5` without `EOFException` crashes.
- **Zero Installation:** Runs as a standalone `.exe` without needing Python, Conda, or GIS driver installations.

---

## ☕ Support the Project & Future Development

> NISAR GCOV X-TRACTOR is developed independently and shared freely for researchers, students, and SAR enthusiasts.
> If this tool saved you processing time or aided your research, consider supporting continued updates and new radar algorithms!

<div align="center">

#### For Donations/Contributions UPI/VPA: 314rsaofficial@okicici or, Kindly Contact me via mail pdbarma01@gmail.com

*Every contribution helps keep this tool updated, optimized, and freely accessible!*

</div>

---

## Terms of Use & License

- **Version Scope:** Governs all past releases, the current build, and all future updates and binaries.
- **Non-Commercial Use:** Free solely for personal, educational, academic, and non-commercial scientific research.
- **Commercial Restriction:** Any commercial use, redistribution, or incorporation into for-profit products/pipelines is strictly prohibited without written consent.
- **Reverse Engineering & AI Protection:** Reverse engineering, binary decompilation, and ingesting/training AI, ML, or automated code synthesis models on this software or its binaries to reproduce its logic or create derivatives is strictly prohibited.
- See the full [LICENSE](LICENSE) for legally binding details.

---

## Feedback & Contact

Have feedback, feature requests, or encountered an issue with a specific NISAR product?
- Open an issue on this repository or reach out directly!

<div align="center">  
  
**Copyright © Pirsa '314rsa' Debbarma 2026. All rights reserved.**  

</div>
