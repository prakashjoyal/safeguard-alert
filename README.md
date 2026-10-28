# RoadGuard — Smart Accident Response Dashboard

A polished React + Vite frontend prototype for a vehicle crash-detection and emergency-alert concept.

## Run locally

Requirements: Node.js 18+ and npm.

```bash
npm install
npm run dev
```

Open the local URL shown by Vite. To verify a production build:

```bash
npm run build
npm run preview
```

## What's included

- Responsive dashboard UI for desktop, tablet and mobile
- Connected vehicle, critical alert, acknowledgement and dispatch metrics
- Illustrative incident location map and sensor health panel
- Adjustable impact sensitivity control
- Recent safety event table
- Built-in local sample video asset (`public/sample-highway-demo.mp4`) with SVG poster fallback
- Interactive “Simulate accident” flow that adds a demo event to the dashboard
- Local-only demo alert preview showing the proposed impact → GPS → alert workflow

## Important prototype limits

This project is a frontend simulation. It does **not** connect to real vehicle sensors, a live GPS device, SMS gateways, police stations, emergency services, or a backend. The displayed coordinates, vehicle IDs, metrics and events are sample data. The “Run simulation” action never sends a real message.

For a real deployment, add a backend/API, authenticated emergency-contact directory, verified local emergency-service integration, secure GPS/device telemetry, delivery receipts, audit logs, false-positive handling and a reliable fallback path. Do not automatically contact emergency services based only on an unvalidated sensor threshold. Validate the crash algorithm and coordinate with the relevant local authorities before operational use.

## Suggested future hardware integration

- Accelerometer / gyroscope (IMU) to detect sudden deceleration and impact patterns
- GPS module to capture coordinates
- Cellular module or a paired phone for connectivity
- Optional airbag / vehicle CAN signal where legally and safely accessible
- Backend to evaluate event confidence and route alerts to verified contacts

## Sample video

The included MP4 is generated demo footage illustrating a stylized highway scene. It is not actual crash footage and is not evidence of real sensor operation.
