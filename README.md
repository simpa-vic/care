# CarePoint Hospital Management — Demo Website

A responsive multi-page hospital-record prototype built with HTML, CSS and vanilla JavaScript.

## Pages
- `index.html` — dashboard KPIs, outcome chart, most treated illnesses and recent visits
- `patients.html` / `patient-form.html` — patient register and patient registration
- `visits.html` / `visit-form.html` — longitudinal treatment history and encounter entry
- `doctors.html` — doctors and specialties; add clinician profiles
- `analytics.html` — illness frequency, gender and age breakdown, outcomes, recorded death outcomes and treatment costs
- `reports.html` — CSV exports for patients, visits and summary metrics
- `settings.html` — restore fictional demo data or clear local records

## Run locally
1. Extract the ZIP file.
2. Open the `medicare_hospital` folder in VS Code.
3. Use the Live Server extension and open `index.html`. Alternatively, open `index.html` directly in a modern browser.
4. Internet access is needed for Chart.js (loaded from jsDelivr CDN) and optional Google Fonts. Forms and local data storage work without a backend, but charts need Chart.js to load.

## Important limitations
This is a front-end prototype, **not a production electronic medical record system**. Records are stored in the browser's `localStorage`, with no server, multi-user synchronization, authentication, authorization, audit trail, backups, or encryption controls. Use only fictional/sample data. Do not enter real patient information.

For a real hospital, build a backend API and database (for example PHP + MySQL/PostgreSQL), enforce role-based access, log access and changes, secure backups, validate clinical data, and review applicable Nigerian data-protection and health-record obligations with qualified professionals. Death figures currently count visits whose outcome is marked `Deceased`; this is not automatically a validated hospital mortality rate.
