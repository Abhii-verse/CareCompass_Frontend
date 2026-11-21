# CareCompass — BedFinder Blitz (Frontend-only)

A responsive vanilla HTML/CSS/JavaScript hackathon prototype. No Node.js, Express, database, API server, or paid key is required.

## Run it
1. Extract the ZIP.
2. Open `index.html` in a modern browser. For best results, use VS Code **Live Server** so browser geolocation works on localhost.
3. Internet is needed for Leaflet map tiles and the Leaflet CDN. Hospital directory and demo filters work locally.

## Features
- 15 sample Hyderabad hospitals with simulated General, ICU, Ventilator and Oxygen counts.
- Search by hospital/area; specialty and facility/bed filters.
- Haversine straight-line distance sorting; use browser geolocation or default Hyderabad demo coordinates.
- Hospital emergency status badges: Normal, Busy, ER Full - Divert.
- Data age indicator; flags sample data older than four hours.
- Call links (`tel:`), ambulance quick dial (`108` and `112`) and Google Maps driving directions.
- Leaflet map with hospital markers and popups.
- Demo admin console (PIN `2468`) to edit beds and status.
- Local browser persistence with `localStorage`.

## Important limitations (say this during judging)
This is a **frontend-only simulation**. Bed counts and hospital contact details are illustrative placeholders, not verified hospital information or live inventory. Admin PIN is client-side and is not real security. Updates are stored only in the current browser and do not sync to other users/devices. Distance is straight-line, not road distance. The app must not be used to make real emergency-care decisions.

## Suggested live demo
1. Search `City Care` and show its simulated ICU beds.
2. Choose the ICU filter and sort by nearest.
3. Open Admin console → PIN `2468` → choose City Care Hospital.
4. Change ICU beds from `4` to `0`, set status to `ER Full - Divert`, and save.
5. Show the updated card and red status badge. Reload to show localStorage persistence.
