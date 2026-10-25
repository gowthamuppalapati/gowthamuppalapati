# Gowtham Uppalapati 👋
📍 Göttingen, Germany | 🎓 Master's Student (Sustainable International Agriculture)  
✉️ gowthamuppalapati21@gmail.com · [LinkedIn](https://www.linkedin.com/in/gowtham-uppalapati/) · [Portfolio](https://gowthamuppalapati.github.io/Gowtham-agritech-portfolio/)

## About me
**Digital agriculture · remote sensing · crop monitoring** – I build end to end, from satellite data to a running web app.
- M.Sc. Sustainable International Agriculture (Göttingen & Kassel) · B.Sc. Agriculture · former test-automation engineer.
- Currently a Student Assistant at the University of Kassel, contributing to agricultural research projects.


## Now building: Field Intelligence

A crop-monitoring platform that follows every field from tillage to harvest, using free satellite and weather data.
Code is private while it is being built; results and screenshots are on LinkedIn.

- **Data engine** – Sentinel-2, Sentinel-1 (radar) and Landsat from two catalogues (Planetary Computer, Copernicus
  Data Space), DWD weather, soil moisture and evapotranspiration; one 10 m grid per field; runs every day on 28
  reference fields in Germany.
- **Own models, each with testing on regions and years it never saw**
  - crop type (LightGBM, 4,500+ parcels, three federal states): 78–91 % right, says "unsure" instead of guessing
  - crop growth (LAI): error 1.04 on measured wheat vs 1.05 for ESA's method
  - cloud gap filler: radar + weather fill cloudy days, with calibrated uncertainty bands
  - soil map from bare-soil images + terrain (EU LUCAS samples): clay R² 0.47 on unseen 50 km blocks
- **Web app** – React, TypeScript, MapLibre, FastAPI, PostGIS; German and English; Linux server with Docker, HTTPS,
    backups and uptime checks; 100+ automated tests.


## Previous Projects

### 🛰️ Satellite-Based Drought Stress & Irrigation Priority Mapping
🔗 [github.com/gowthamuppalapati/agri-drought-monitor](https://github.com/gowthamuppalapati/agri-drought-monitor)
- Built an automated Sentinel-2 pipeline via the Microsoft Planetary Computer STAC API — cloud-filtered search, AOI clipping, band extraction
- Combined NDVI and a SWIR-based NDWI into a single drought stress index
- Classified the index into three irrigation-priority tiers (High/Medium/Low) using percentile-based thresholds
- *Prototype – known issues listed in the repo.*

### 🌱 weedscout – where to scout for weeds first
🔗 [github.com/field-intelligence-platform/weedscout](https://github.com/field-intelligence-platform/weedscout) · open source (Apache-2.0) · v1.6.0
- A free tool that shows a farmer, agronomist or drone pilot where to walk first when scouting a field for weeds.
- Give it the field boundary file you already have and a year; it uses free Sentinel-2 satellite images to find the zones that grew weaker than the rest of their own crop on most clear days, and returns a map, zones for farm software and a plain-language summary in 1–2 minutes.
- It is a scouting map, not a weed detector: a weak zone can also be waterlogging, compaction or nutrient stress, and every zone shows its evidence ("weaker on 8 of 10 dates").
- Tested on 28 fields across Germany it was never tuned on, it found 79–81 % of planted weak patches and flags almost nothing by chance. 

### 🐐 Virtual Fencing — GPS-Based Livestock Containment
🔗 [github.com/gowthamuppalapati/Virtual_Fence_Proj](https://github.com/gowthamuppalapati/Virtual_Fence_Proj)
- Simulated the GPS-collar containment tech used by Nofence/Halter/eShepherd — audio-then-stimulus cues instead of physical fencing
- Shapely-based boundary-crossing prediction — warns animals based on projected heading, not just current position
- Built a Q-learning contextual bandit personalizing warning lead-time per animal — resolved 91.5% of approaches by audio alone vs. an 88.6% fixed-threshold baseline, cutting stimulus events from 263 to 223
- Shipped a live FastAPI dashboard with a rule-based natural-language herd assistant


## Experience
**Student Assistant (HiWi) — University of Kassel, Witzenhausen, Germany**
*Apr 2026 – Present*
- Contributing to the university's agricultural research projects (field data, sensors, software).

**Software Tester — Pinnacle Group, Inc. (Hyderabad)**
*Dec 2023 – May 2025*
- Automated end-to-end tests for web & mobile applications (Java, Selenium, TestNG, Jenkins CI)
- Built and maintained regression suites and clear test documentation
- Tracked defects and collaborated with dev/QA teams to validate fixes
- DevOps work on AWS; focused on **data accuracy, consistency, and structured processes**

## Education
- **MSc Sustainable International Agriculture (SIA)** — University of Göttingen & University of Kassel (Oct 2025 – Present)  
  Relevant: soil fertility, organic farming systems, agri-environmental policy, agricultural data analysis, precision farming
- **B.Sc. Agriculture** — PDKV Akola
  
## Skills
- **Agriculture:** agronomy, crop production, crop monitoring, soil science, weed & pest management, precision farming
- **Agri data:** remote sensing (Sentinel-1/2, Landsat), vegetation indices, GIS / QGIS, PostGIS, machine learning (LightGBM), data analysis
- **Development:** Python, FastAPI, React, TypeScript, SQL, Java, Git
- **Testing:** test automation, Selenium, TestNG, pytest, regression testing
- **Deployment:** Linux servers, Docker, CI/CD (GitHub Actions, Jenkins), Oracle Cloud, AWS (EC2, S3, IAM, VPC)

## Contact
- Email: **gowthamuppalapati21@gmail.com**
- Location: **Göttingen, Germany**
