# 4DX Cinema Experience | WebXR & PS VR2 Portal

A futuristic web-based 4DX cinema simulator with haptic feedback simulation, seat selection, movie browsing, and experimental WebXR / Three.js VR theater mode (aimed at PS VR2 / WebXR headsets).

## Features

- **4DX Seat Simulator** – Interactive motion platform with preset effects (Top Gun jet dive, Avatar mist, Oppenheimer blast, Mad Max heat wave)
- **Environmental effects** – Particle systems for water spray & wind, device vibration (haptics) where supported
- **Movie showcase** – Filterable grid of 4DX-enhanced films with effect tags
- **Seat reservation** – Interactive theater map with Standard vs 4DX Prime seats and live price calculation
- **WebXR / VR Mode** – Three.js powered virtual cinema screen (enter via “Launch PS VR2 Mode”)

## Tech Stack

- Vanilla HTML / CSS / JS
- Tailwind CSS (CDN)
- Three.js (r128) for WebXR scene
- Font Awesome icons
- Device Vibration API for haptics

## Quick Start

Just open `index.html` in a modern browser (Chrome / Edge recommended for WebXR & vibration).

For local development:

```bash
# any static server
npx serve .
# or
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Notes

- Full WebXR session requires a compatible headset / browser and secure context (HTTPS or localhost).
- Haptic vibration works on mobile devices that support the Vibration API.
- This is a front-end demo / prototype — no backend booking system is included.

## License

MIT
