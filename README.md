# 🌊 Hai Phong Flood Risk Assessment
### Spatial Risk Intelligence Deliverable | Northern Vietnam | IntelliWhere

![Risk Level](https://img.shields.io/badge/Flood%20Risk-District%20Level%20Analysis-blue)
![Data](https://img.shields.io/badge/Data-Open%20Source%20%7C%20Free-green)
![Stack](https://img.shields.io/badge/Stack-Python%20%7C%20GeoPandas%20%7C%20Folium%20%7C%20ReportLab-orange)
![Status](https://img.shields.io/badge/Status-Sample%20Deliverable-teal)

---

## What This Project Is

A **professional GIS risk consulting deliverable** demonstrating how spatial data analysis can be used to assess flood risk for lenders, insurers, investors, and local government with asset exposure in Hai Phong, Vietnam.

Hai Phong is Vietnam's largest northern seaport, sitting at the mouth of the Red River Delta — 1 to 4 metres above sea level. That geography creates compounded flood exposure from typhoons, river overflow, and coastal storm surge converging simultaneously across all 15 administrative districts.

This project is part of the **IntelliWhere** GIS risk intelligence portfolio — building AI-assisted spatial analysis tools for financial and infrastructure decision-making.

---

## How to Run
Link in GitHub Pages brings you to the interactive risk analysis map.

```bash
git clone https://github.com/intelliwhere/hai-phong-flood-risk
cd hai-phong-flood-risk
pip install -r requirements.txt
jupyter notebook hai_phong_flood_risk.ipynb
```

The HTML map and PDF are pre-rendered — open them directly with no code required.

**requirements.txt:**
```
geopandas
folium
pandas
numpy
shapely
reportlab
jupyter
```

---

## Deliverables

| File | Description |
|---|---|
| `hai_phong_flood_risk.ipynb` | Jupyter notebook — full methodology, district scoring, risk classification, and plain-language findings written to be readable by non-technical clients |
| `hai_phong_flood_risk.html` | Interactive map — polygon-based district overlays, 7 toggleable spatial data layers, sliding city info panel, district score slideshow, and three advisory overlays |
| `hai_phong_final.pdf` | 11-page professional risk brief with executive summary, methodology, flood risk factor analysis, district evidence table, and key findings for lenders and insurers |
| `README.md` | This file |

---

## Interactive Map Features

`hai_phong_flood_risk.html` is fully self-contained — open in any browser, no server required.

**Core map:**
- 14 district polygons colour-coded by flood risk (red = Very High → green = Low)
- Click any district for verified incident data and score reasoning
- Fixed-size labels readable at all zoom levels

**7 Spatial Layers (toggle on/off):**
- 🌡️ **Elevation Heatmap** — NASA SRTM colour-coded by ground height with legend
- 🌊 **River Network** — Thai Binh, Van Uc, Lach Tray, and Cam rivers
- 📏 **500m River Buffer** — flood overflow proximity zones
- 🔵 **Sea Level Rise +1m** — UNDP 2050 coastal inundation scenario
- 🌀 **Typhoon Track Corridor** — 4 historical NOAA IBTrACS tracks + Gulf of Tonkin corridor
- 🟡 **Urban Drainage Risk** — Hong Bang and Le Chan legacy network failure zones
- 🔴 **Storm Surge Zone** — coastal district exposure with surge approach direction

**4 Advisory Panels (bottom button bar):**
- **District Score Evidence** — 8-slide carousel with score reasoning and verified incidents
- **Interpretation** — how to read the map, suitable vs. unsuitable zones, mitigation areas
- **Implications** — risk implications by client type (lenders, insurers, developers, government)
- **Recommendations** — concrete action steps per client type

---

## Risk Methodology

Scores (1–5) derived from four weighted factors:

| Factor | Source | Weight |
|---|---|---|
| Elevation above sea level | NASA SRTM (30m) | High |
| Proximity to coastline / river systems | OpenStreetMap hydrography | High |
| Historical typhoon track density | NOAA IBTrACS (1990–2024) | Medium |
| District land use & infrastructure | OpenStreetMap + Vietnam MARD | Medium |

All scores anchored to verified historical incidents — no district receives High or Very High without documented evidence from ReliefWeb, VnExpress, MARD audits, or FAO records.

---

## Data Sources (All Free & Publicly Available)

| Dataset | Source |
|---|---|
| District boundaries, roads | OpenStreetMap |
| Elevation terrain (30m) | NASA SRTM |
| Historical typhoon tracks | NOAA IBTrACS (1990–2024) |
| Flood hazard / dike ratings | Vietnam MARD (Audit 2020–21) |
| Disaster situation reports | ReliefWeb / UN OCHA |
| Climate projections | UNDP Vietnam 2019 |
| Agricultural loss records | FAO Vietnam 2017 |
| News archive | VnExpress, Tuoi Tre (2005–2024) |

---

## Key Findings

- **60%** of Hai Phong's districts carry High or Very High flood risk
- **5 districts** face compound simultaneous exposure — not covered by standard single-peril insurance
- **Hai An port** was overtopped during Typhoon Son Tinh (2018): 12,000 homes flooded, 48hr suspension
- **Tien Lang** projected to lose 15–20% of land area under 30cm sea level rise (UNDP 2019)
- **Cat Hai island** isolated 72+ hours during Typhoon Bebinca (2024) — no road evacuation corridor

---

## Disclaimer

This analysis is based on compiled spatial data from publicly available sources for informational risk assessment purposes only. It does not constitute a legal survey, boundary determination, or professional engineering opinion. Site-specific conditions may vary materially.

---

## About IntelliWhere

**IntelliWhere** — Geospatial risk intelligence combining open spatial data and Python-based GIS analysis to produce decision-ready deliverables for financial and infrastructure clients.

**Ryan Nguyen** | B.Eng Geomatics Engineering, York University (EIT)

- 📧 intelliwhere@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/ryan-nguyen-1504bb182/)
- 🐙 [GitHub](https://github.com/intelliwhere)

---

> *Next in this series: Traffic Congestion Analysis (Hanoi) · Air Pollution Risk Mapping (Northern Vietnam)*
