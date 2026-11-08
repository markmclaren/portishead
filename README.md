# Portishead Walks & Locations Map

An interactive, responsive web map centred on **17 Avon Way, Portishead, BS20 6JJ**, highlighting circular walks, points of interest, supermarkets, and local amenities.

Live demo: **[https://markmclaren.github.io/portishead/](https://markmclaren.github.io/portishead/)**

---

## Features

- **5 Curated Circular Walks** starting and ending at 17 Avon Way, with distance, estimated walking duration, directional path arrows, and route highlights.
- **Points of Interest & Landmarks:** Victorian Lake Grounds, Battery Point Lighthouse, Eastwood Local Nature Reserve, Portishead Quays Marina, Portishead Marina Lock, Portishead Pier, SeaRock Fish & Chips, Mokoko Coffee & Bakery, Fisherman's Steps, and Portbury Wharf Nature Reserve.
- **Local Amenities:** Supermarkets (Waitrose, Sainsbury's, Lidl, Aldi, Tesco Express, Co-op, etc.) and Medical facilities (GP, Pharmacies, Dentist, Vet, Clevedon Minor Injury Unit).
- **Interactive Controls:** Toggle walks and POI layers, interactive popups with full descriptions, home recentring, and GPS geolocation tracking (`trackUserLocation`).
- **Mobile Responsive:** Collapsible drawer menu, bottom walk info banner, touch-friendly UI.

---

## Walks Overview

| Walk | Distance | Duration | Key Highlights |
| :--- | :--- | :--- | :--- |
| **Walk 1: Lake Grounds to Marina (via Eastwood)** | 5.3 km | ~71 min | Lake Grounds boating lake & seawall promenade, Battery Point Lighthouse, Eastwood Nature Reserve along Broad Walk, The Royal Inn, Marina Lock, East Quay, Marina South, High Street. |
| **Walk 2: Portishead Marina Loop & Pier** | 4.4 km | ~58 min | West Quay promenade, coastal promenade out to the tip of Portishead Pier, Marina Lock bridge, Mokoko Coffee, SeaRock Fish & Chips, East Quay, Marina South, High Street. |
| **Walk 3: Kilkenny Bay & Fisherman's Steps** | 2.7 km | ~37 min | West Hill, drops down Beach Hill and Beach Road West to Mariners Path along Kilkenny Bay, Fisherman's Steps, traffic-free return across Kilkenny Fields footpaths and Stoney Steep (avoids walking along Nore Road). |
| **Walk 4: Portbury Wharf Nature Reserve** | 7.7 km | ~102 min | Marina promenade to Severn Estuary coastal path, Tower Hide, North Pool Hide, South Pool Hide, scenic return hugging Swan Lake, Phoenix Way, Quays Avenue, central walkway across Sainsbury's car park, and Old Mill Road. |
| **Walk 5: Marina Loop via The Rhyne & Waitrose** | 4.0 km | ~53 min | West Quay, Marina Lock bridge, Marina East, full length of The Rhyne footpath to Harbour Road, and Waitrose Piazza back to Cabstand. |

---

## Tech Stack

- **Map Engine:** [MapLibre GL JS](https://maplibre.org/) (`v5.2.0`)
- **Map Vector Tiles:** [OpenFreeMap](https://openfreemap.org/) (`liberty` style)
- **Data Format:** [GeoJSON](https://geojson.org/) for all routes and marker layers
- **Architecture:** Vanilla JavaScript, HTML5, and CSS3 — zero dependencies, build tools, or frameworks required.

---

## Running Locally

Clone the repository and launch a local web server (needed for GeoJSON fetches):

### Windows (Quick Launch)
Double-click `run.bat` or run in terminal:
```cmd
run.bat
```

### Python
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000/` in your browser.

---

## GitHub Pages Deployment

To host this map via GitHub Pages:
1. Navigate to **Settings > Pages** in your GitHub repository.
2. Under **Build and deployment > Source**, select **Deploy from a branch**.
3. Choose branch **`main`** and folder **`/ (root)`**, then click **Save**.
4. The site will be live at `https://<username>.github.io/portishead/`.
