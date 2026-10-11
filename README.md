# TerraMetrics Property Risk Intelligence — v3.0

A static Leaflet GIS and illustrative climate-insurance research dashboard inspired by the uploaded dark property-intelligence interface.

## Folder structure

```
TerraMetrics_Risk_Studio/
  index.html
  package.json
  README.md
  css/ (main.css, map.css, sidebar.css, popup.css, legend.css)
  js/ (app.js, basemaps.js, config.js)
  data/zaf_data/ (uploaded South African geospatial JavaScript and GeoJSON datasets)
```

## Run locally

1. Extract the ZIP.
2. Open a terminal inside `TerraMetrics_Risk_Studio`.
3. Run `python -m http.server 8000`.
4. Visit `http://localhost:8000`.

Internet is required for Leaflet, Chart.js, Turf.js, basemap tiles and address geocoding (OpenStreetMap Nominatim). Local GIS data load from `data/zaf_data`.

## Features

- Address search using public Nominatim (network access and fair usage limits apply)
- Selected-location aerial imagery and geocoding result table
- Interactive street/satellite map and optional geographic overlays
- Visible GIS attribute table, downloadable CSV
- Geometric proximity buffer, **not** a hazard prediction
- User-adjustable annual event probability, damage ratio, insured exposure, expected annual loss
- Sensitivity chart and JSON scenario export

## Important limitations

No hurricane Ian model, FEMA damage classification, calibrated flood depths, observed wind speeds, property-specific claims or proprietary insurance scores are supplied. The reference screenshot is used only as a **layout/style reference**, not as evidence for those metrics. Financial outputs are **hypothetical** and not suitable for actual underwriting or insurance quotes. Geocoding confidence is not assessed.

This project retains the user-supplied GIS layers and is designed for further integration with validated climate and insurance datasets.
