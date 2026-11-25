# Afghanistan Clinics Dashboard

An interactive web GIS dashboard for exploring health clinics across Afghanistan: where they are, what type they are, and which districts they serve.

**Live demo:** https://clinics-gilt.vercel.app

## Features

- **Clinic map** with marker clustering; facility labels appear from zoom level 8
- **District boundaries** (ADM2) as a toggleable overlay layer
- **Search and filters** by district and facility type; the map flies to the selected clinic
- **Summary cards**: total clinics, hospitals, donor-supported clinics, clinics with clean water
- **Charts** built with Chart.js
- **Clinic detail page** for every facility (`/clinic/:id`) with its own location map

## Tech stack

| Area | Tools |
|---|---|
| UI | React 19, React Router, React-Bootstrap / Bootstrap 5 |
| Mapping | Leaflet, React-Leaflet, react-leaflet-cluster |
| Charts | Chart.js, react-chartjs-2 |
| Data | PapaParse (CSV), GeoJSON, react-window (virtualised lists) |

## Data

- Clinic list: CSV from [clinics-map-streamlit](https://github.com/rahimiabdulrahmanab/clinics-map-streamlit)
- District boundaries: [`public/afg_admin2.geojson`](public/afg_admin2.geojson), Afghanistan's 401 districts (ADM2), included in this repository

## Run locally

```bash
npm install
npm start
```

Then open http://localhost:3000.

---

Built by **Abdul Rahman Rahimi**, Software Developer & Geospatial Analyst, [Rahimi Tech Solution](https://github.com/rahimiabdulrahmanab).
