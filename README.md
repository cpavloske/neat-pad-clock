# Neat Pad Clock

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

No setup needed — use this URL when creating the custom web app in Neat Pulse.

### Self-hosting

Host `index.html` on any static file server, then use that URL in Neat Pulse.

### Adding to Neat Pulse

In [Neat Pulse](https://pulse.neat.no), create a custom web app and point it to the hosted URL above. The app will then be deployable to your Neat Pad from Pulse.

## APIs Used

| Service | Purpose |
|---|---|
| [Open-Meteo](https://open-meteo.com/) | Weather & hourly forecast |
| [Open-Meteo Geocoding](https://open-meteo.com/en/docs/geocoding-api) | City search |
| [ipapi.co](https://ipapi.co/) | IP-based location detection (primary) |
| [ipwho.is](https://ipwho.is/) | IP-based location detection (fallback 1) |
| [freeipapi.com](https://freeipapi.com/) | IP-based location detection (fallback 2) |
