# CarePoint — Appointment Booking Demo

CarePoint is a responsive, single-page healthcare appointment booking website built as a frontend portfolio demonstration. It includes doctor discovery, specialty filters, fictional provider profiles, an appointment booking flow, demo account screens, a patient dashboard, and an admin overview.

> **Demo only:** This project is not connected to a clinic or a backend. The doctor profiles, ratings, availability, testimonials, and contact details are fictional. Demo account and booking data are stored in the browser's local storage/session storage. Do not enter real patient or health information.

## Run locally

No build step or package installation is required.

1. Download or clone this folder.
2. Open `index.html` directly in a modern browser.
3. For a local web server, run `python -m http.server 8000` from this folder and visit `http://localhost:8000`.

The website uses hash-based routes, so direct file opening works without server-side routing configuration.

## Features

- Responsive homepage and mobile navigation
- Specialty links and doctor directory search, fee, availability, and sort filters
- Dynamic fictional doctor profile pages
- Appointment date/time selection, review, confirmation reference, and duplicate-slot checks within this browser
- Local demo registration and sign-in screens
- Patient appointment history and cancellation confirmation
- Admin overview page
- FAQ accordion, privacy and terms pages

## Project files

- `index.html` — application entry point
- `styles.css` — responsive styling and visual design
- `app.js` — sample data, hash router, and browser-local interactions

## Assets and dependencies

The app has no npm dependencies or build tools. Doctor and hero photography is loaded from Unsplash, and the DM Sans / Manrope fonts are loaded from Google Fonts. Those remote assets require an internet connection; system font fallbacks and the rest of the site work without them.

## Demo navigation

- Home: `#/`
- Doctor directory: `#/doctors`
- Login/register: `#/login`, `#/register`
- Patient dashboard: `#/dashboard`
- Admin overview: `#/admin`

Register with any demo name/email/password, then sign in using the same email. This is a visual interaction demo, not secure authentication. The admin overview is also a public demo route and has no authorization enforcement.

## Validation

The JavaScript syntax was checked with `node --check app.js`. This static site has no automated test suite or production API/database.
