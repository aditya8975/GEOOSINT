# GEOINT PRO

**A browser-based, open-source intelligence (OSINT) dashboard that aggregates live public data onto an interactive map — satellite imagery, military installations, air traffic, geopolitical events, seismic activity, weather, and country-level data — with zero backend.**

![status](https://img.shields.io/badge/status-active-brightgreen)
![license](https://img.shields.io/badge/license-MIT-blue)
![type](https://img.shields.io/badge/stack-vanilla%20JS-yellow)

> All data comes from verified, public, open-source APIs (OpenStreetMap, NASA GIBS, OpenSky, GDELT, USGS, Open-Meteo, REST Countries, World Bank). No private, classified, or proprietary data is used or required.

---


---
![Project Home](images/g1.PNG)
---
---
![Project Home](images/g2.PNG)
---
---
![Project Home](images/g3.PNG)
---
---
![Project Home](images/g4.PNG)
---
---
![Project Home](images/g5.PNG)
---
---
![Project Home](images/g6.PNG)
---
---
![Project Home](images/g7.PNG)
---
---
![Project Home](images/g8.PNG)
---
---
![Project Home](images/g9.PNG)
---
---
![Project Home](images/g11.PNG)
---
---
![Project Home](images/g12.PNG)
---
---
![Project Home](images/g13.PNG)
---
---
![Project Home](images/g14.PNG)
---

## What it does

GEOINT PRO lets you drop a pin (or search a location) and pull together a live intelligence picture of that area, entirely client-side:

| Module | Source | What you get |
|---|---|---|
| Satellite imagery | NASA GIBS | True color, false color (burn/vegetation), NDVI, thermal, night lights — 8 selectable layers |
| Military installations | OpenStreetMap Overpass | Bases, airfields, checkpoints, ranges, bunkers, etc. |
| Airports & airfields | OpenStreetMap Overpass | Civil/military airfield classification |
| Live air traffic | OpenSky Network | Real-time ADS-B aircraft positions + heuristic "suspicious" flagging |
| Geopolitical events | GDELT Project v2 | Recent events + tone/sentiment in a radius around your point of interest |
| News | The Guardian API | Related news coverage |
| Seismic activity | USGS | Recent M4.5+ earthquakes |
| Environment | Open-Meteo | 30-day temperature, precipitation, wind history |
| Country intelligence | REST Countries + World Bank | Population, GDP, military spend, borders |
| Cyber lookups | ipinfo.io | Quick IP/domain lookups |
| OSINT toolkit | — | Curated links to Bellingcat, SunCalc, WHOIS, Wayback Machine, OpenCorporates, etc. for manual investigation |
| AI intelligence brief | Groq (Llama 3.3 70B) | Generates a written summary from all loaded data, using your own free API key |

Everything renders on a [Leaflet](https://leafletjs.com/) map with draw/measure tools, a searchable command bar, and an exportable plain-text intelligence report.

## Screenshots

> _Add screenshots or a short GIF here (`docs/screenshot-1.png`) once you have them — GitHub renders images inline and this is usually the first thing a reviewer looks at._

## Tech stack

- **Vanilla HTML/CSS/JS** — no framework, no build step, no bundler
- [Leaflet.js](https://leafletjs.com/) + [Leaflet.draw](https://github.com/Leaflet/Leaflet.draw) for the map
- [Chart.js](https://www.chartjs.org/) for data visualization
- All data fetched client-side directly from public REST APIs

 simply open `index.html` directly in a browser.

### API keys (optional, all free-tier)

Some modules work out of the box with no key (OSM, OpenSky, USGS, Open-Meteo, REST Countries, World Bank, GDELT). A few optional modules need a free key, added in-app via the **⚙ API Keys** panel — keys are stored only in your browser's `localStorage` and are never sent anywhere except the relevant provider's API:

| Module | Provider | Get a free key |
|---|---|---|
| AI Intelligence Brief | Groq | https://console.groq.com |
| Fire/thermal hotspots | NASA FIRMS | https://firms.modaps.eosdis.nasa.gov/api/ |
| News module | The Guardian | https://open-platform.theguardian.com/access/ |
| Conflict events | ACLED | https://acleddata.com/register/ |
| IP/domain reputation | AbuseIPDB | https://www.abuseipdb.com/register |
| File/hash reputation | VirusTotal | https://www.virustotal.com/gui/join-us |


## Disclaimer

This tool is intended for **open-source research, journalism, and educational purposes**. It aggregates only publicly available data. It is not affiliated with any government or defense agency, and the "UNCLASSIFIED" labeling in the UI reflects that all displayed data is public-source, not any official classification marking.

## License

MIT — see [LICENSE](LICENSE).

## Author

Built by **Aditya** ((https://github.com/aditya8975)) 
