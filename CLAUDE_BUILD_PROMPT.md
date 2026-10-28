# Claude build prompt — RoadGuard Smart Accident Response

Build a premium, responsive React + Vite web application named **RoadGuard** for a smart highway accident detection and emergency response concept.

## Concept
A vehicle-mounted IMU/accelerometer detects a potential severe collision. The device captures GPS coordinates, vehicle ID and event time, then creates an emergency incident record and prepares a message for a verified control room / police contact. The interface should make the workflow visible: **impact detected → severity checked → GPS captured → alert prepared → dispatch status tracked**.

## UI direction
- Build a refined, production-style emergency operations dashboard, not a generic template.
- Visual style: dark navy left sidebar, bright neutral workspace, blue primary actions, green operational state, red critical-event state, generous whitespace, subtle borders and shadows.
- Use a clean sans-serif font, responsive desktop/tablet/mobile layouts, accessible contrast and keyboard-friendly controls.
- Include dashboard cards, live/demo status, sensor-health panel, incident location visual, recent events table, a local incident video player, and a detailed accident simulation modal.
- Make all buttons and interactions work in the frontend. Do not leave dead controls.
- Include clear demo labels on sample values and simulated GPS.
- Include local sample video under `public/` and reference it with a relative path so the app works offline after dependencies are installed.
- Use React functional components and hooks, Vite, and lucide-react icons. Keep code organized and provide a README.

## Functional demo
- “Simulate accident” opens a modal with vehicle ID, severity, GPS coordinates and destination label.
- Confirming creates a local event, updates the recent events list, and shows the steps that would be performed.
- Add adjustable impact sensitivity and mock sensor states.
- Include a “copy coordinates” action and toast feedback.
- Video player must use the included local demo clip.
- The frontend must not claim to have actually sent an SMS, called police, or connected to hardware.

## Safety and real-world integration notes
This is a prototype, not a life-safety product. Use mock data only. Do not send real emergency messages or call real police numbers from the demo. For production, implement a secure backend, validated crash-classification logic, authenticated/verified emergency contacts, delivery acknowledgements, audit logs, privacy controls, false-positive cancellation and a fallback mechanism. Show a confirmation / demo notice before simulated dispatch. Avoid hardcoding an unverified police station number.

## Deliverables
- Complete runnable React + Vite source
- `npm install`, `npm run dev`, `npm run build` support
- Local demo video in `public/`
- README with setup and limitations
- A ZIP archive of the complete project
