# Neat Pad Pro Clock

A minimal clock + weather display designed for the Neat Pad (1280×800).

## Features

- Live clock with seconds, AM/PM, day and date
- Current weather via [Open-Meteo](https://open-meteo.com/) — temperature, feels like, humidity, wind, rain chance
- Auto-detects location on load via IP geolocation (no browser permissions needed)
- Interactive hourly rain chance chart
- Manual location picker — choose from presets or search any city

## Usage

Open `index.html` in a browser. No build step or dependencies required.

For local development with live reload:

```bash
npx http-server . -p 3001 -c-1
```

Then open `http://localhost:3001`.

## Deployment

### GitHub Pages (quickest)

Already hosted at: **https://cpavloske.github.io/neat-pad-clock/**

Point the Neat Pad browser to that URL — no setup needed.

### Self-hosting

Host `index.html` on any static file server and point the Neat Pad browser to that URL.

## APIs Used

| Service | Purpose |
|---|---|
| [Open-Meteo](https://open-meteo.com/) | Weather & hourly forecast |
| [Open-Meteo Geocoding](https://open-meteo.com/en/docs/geocoding-api) | City search |
| [ipapi.co](https://ipapi.co/) | IP-based location detection |
