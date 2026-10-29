# 4DX Cinema Experience | WebXR & PS VR2 Portal

A futuristic web-based 4DX cinema simulator with haptic feedback simulation, seat selection, movie browsing, and a proper **WebXR immersive theater** designed for PS VR2 / WebXR-compatible headsets.

## Features

- **4DX Seat Simulator** – Interactive motion platform with preset effects (Top Gun jet dive, Avatar mist, Oppenheimer blast, Mad Max heat wave)
- **Environmental effects** – Particle systems for water spray & wind, device vibration (haptics) where supported
- **Movie showcase** – Filterable grid of 4DX-enhanced films with effect tags
- **Seat reservation** – Interactive theater map with Standard vs 4DX Prime seats and live price calculation
- **PS VR2 / WebXR Immersive Mode**
  - Full `immersive-vr` session request
  - Cinema environment (screen, floor, walls, seat rows)
  - Dual controller support with visual rays + grips
  - Haptic feedback via controller actuators / gamepad vibration (Sense controllers)
  - `local-floor` reference space (ideal for seated experiences)
  - Graceful fallback UI when WebXR is unavailable

## Tech Stack

- Vanilla HTML / CSS / JS
- Tailwind CSS (CDN)
- Three.js (r128) + WebXR
- Font Awesome icons
- Device Vibration API + WebXR haptic actuators

## Quick Start

Open `index.html` in a modern browser (Chrome or Edge recommended).

For local development (required for WebXR on most browsers):

```bash
npx serve .
# or
python -m http.server 8000
```

Visit `http://localhost:8000` and click **Launch PS VR2 Mode**.

## PS VR2 Notes

- Official PlayStation browser WebXR support for PS VR2 is limited / evolving. This experience uses the standard WebXR API so it works on any compatible headset or PC browser with a VR runtime.
- When running on a system that exposes PS VR2 Sense controllers via WebXR (or streaming solutions), trigger / squeeze inputs fire haptic pulses.
- Best results: Chrome/Edge + WebXR-capable runtime, or a headset that supports immersive-vr sessions.

## License

MIT
