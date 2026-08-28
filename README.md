# Gowtham Uppalapati 👋
📍 Göttingen, Germany | 🎓 Master's Student (Sustainable International Agriculture)  
✉️ gowthamuppalapati21@gmail.com

## About me
- Master's student in **Sustainable International Agriculture** (University of Göttingen & University of Kassel)
- Former **Software Tester** (Pinnacle Group, Inc.) with experience in end-to-end testing, defect tracking, and data accuracy
- Currently a Student Assistant at the University of Kassel, building the computer-vision training dataset behind **BeetleBot**, an autonomous robot that detects crop pests — multi-light field imaging and life-stage-aware image annotation in LabelMe
- Interested in **digital agriculture, remote sensing, precision farming, and data-driven decision support**
- Comfortable with **Python, Java, GIS workflows, computer vision dataset annotation**, and cloud/dev tools

## What I'm focusing on
- Remote sensing & geospatial analytics for agriculture (Sentinel-2, NDVI/NDWI)
- Computer vision dataset engineering — multi-light imaging, multi-class annotation for ML models
- Building clean, reproducible data workflows (Python + GIS)

## Tech stack
**Programming:** Python, Java  
**Geospatial/RS:** QGIS, NDVI/NDWI, Sentinel-2 (Planetary Computer STAC API), Raster processing (Rasterio, Rioxarray)  
**Computer Vision & ML:** LabelMe, multi-class image annotation, Q-learning / contextual bandits  
**Tools:** Git/GitHub, VS Code, Testing docs & workflows  
**OS:** Windows, Linux

## Featured projects

### 🐞 BeetleBot — Autonomous Pest Detection *(Current)*
- Student Assistant role on an autonomous, row-straddling robot that scans field crops for the Colorado Potato Beetle while distinguishing it from beneficial insects like ladybirds
- Annotated 800+ field images in LabelMe across an 8-class, life-stage-aware taxonomy — egg, larva, pupa, and adult stages of the pest and its natural predator, plus aphids
- Captured imagery under a controlled multi-light setup (white/red/blue/green LED) for a dataset robust to real-world lighting variation
- Coordinated multi-camera capture rigs mounted under the chassis for synchronized multi-angle imagery

### 🐄 Trittschall — SoundHooves Lameness Detection *(Completed)*
- Built the hoof-sound controller for a preclinical dairy cow lameness detection system at the University of Kassel — a core Python daemon managing FDX-B RFID identification, RS-232 serial communication, and inter-process coordination via trigger files
- Decoded the proprietary FDX-B RFID frame byte-by-byte, including the `0x5309B1` handshake and 15-digit animal IDs
- Built automatic RS-232 crash recovery — the system self-reconnects on port loss with no manual intervention

### 🛰️ Satellite-Based Drought Stress & Irrigation Priority Mapping
- Built an automated Sentinel-2 pipeline via the Microsoft Planetary Computer STAC API — cloud-filtered search, AOI clipping, band extraction
- Combined NDVI and a SWIR-based NDWI into a single drought stress index
- Classified the index into three irrigation-priority tiers (High/Medium/Low) using percentile-based thresholds

### 🌱 Precision Weed Detection and Targeted Spraying
- Geospatial workflow flagging weed-suspicion zones from Sentinel-2 NDVI (< 0.4 = weak vegetation) via the Planetary Computer STAC API
- Cleaned raw classification with connected-component noise filtering, then converted to vector management zones with a three-tier spray priority (High/Medium/Low)
- Scoped explicitly as a weed-*suspicion* signal, not confirmed detection — low NDVI can also mean nutrient deficiency, water stress, or pest damage

### 🐐 Virtual Fencing — GPS-Based Livestock Containment (Simulation)
- Simulated the GPS-collar containment tech used by Nofence/Halter/eShepherd — audio-then-stimulus cues instead of physical fencing
- Shapely-based boundary-crossing prediction — warns animals based on projected heading, not just current position
- Built a Q-learning contextual bandit personalizing warning lead-time per animal — resolved 91.5% of approaches by audio alone vs. an 88.6% fixed-threshold baseline, cutting stimulus events from 263 to 223
- Shipped a live FastAPI dashboard with a rule-based natural-language herd assistant

## Experience
**Student Assistant (HiWi) — University of Kassel, Witzenhausen, Germany**
*Apr 2026 – Present*
- Built the SoundHooves hoof-sound controller (RFID, serial comms, crash recovery) — *completed*
- Currently building the training dataset for BeetleBot — multi-light field imagery and LabelMe annotation across an 8-class, life-stage-aware taxonomy

**Software Tester — Pinnacle Group, Inc. (Hyderabad)**
*Dec 2023 – May 2025*
- Tested web & mobile applications end-to-end for reliability and functional correctness
- Designed and executed manual test cases; maintained clear test documentation
- Tracked defects and collaborated with dev/QA teams to validate fixes
- Focused on **data accuracy, consistency, and structured processes**

## Education
- **MSc Sustainable International Agriculture (SIA)** — University of Göttingen & University of Kassel (Oct 2025 – Present)  
  Relevant: soil fertility, organic farming systems, agri-environmental policy, agricultural data analysis, precision farming

## Contact
- Email: **gowthamuppalapati21@gmail.com**
- Location: **Göttingen, Germany**
