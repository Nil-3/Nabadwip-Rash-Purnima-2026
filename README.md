# Nabadwip Rash Purnima 2026 — Heritage Festival Guide

**Live Web App:** [https://nil-3.github.io/Nabadwip-Rash-Purnima-2026/](https://nil-3.github.io/Nabadwip-Rash-Purnima-2026/)

A mobile-first, zero-backend festival companion built for visitors navigating the historic Shakta Rash festival in Nabadwip, West Bengal. Designed as a lightweight single-file web app (`index.html`) ready for instant browser use or Android packaging via Capacitor.

---

## Problem & Product Thinking

During Rash Purnima, Nabadwip transforms into a dense "No Vehicle Zone" where thousands of visitors navigate narrow *para* (alleyway) networks between midnight and 4 AM under heavy mobile network congestion. This app solves four core pain points:

1. **Disorientation in Narrow Lanes:** Combines a curated directory of **31 Shakta Rash pujas** with GPS proximity sorting and hybrid walking navigation.
2. **Network Congestion & Battery Drain:** Uses a lightweight single-file architecture with instant-access SOS helplines, festival rules, and local food directories—no heavy backend or login walls.
3. **Late-Night Readability:** Includes a dedicated **Night Mode** (low-glare obsidian-and-gold palette + dimmed map tiles) tailored for overnight darshan.
4. **Remote Testing for Reviewers:** Automatically falls back to **Nabadwip Dham Railway Station** as a demo starting point if GPS is denied or the user is more than 50 km away, allowing anyone to test **Nearest** sorting and route previews from anywhere.

---

## Key Features

* **31 Shakta Rash Puja Directory:** Instant search by pandal name or neighborhood, GPS-based **Nearest** sorting with live distance badges, and a persistent visited checklist (`0 / 31` saved via `localStorage`).
* **Multi-Layer Interactive Map:** Powered by Leaflet.js with color-coded markers for **31 Pujas**, **10 renowned *Lal Doi* & local food spots** (toggleable layer), and **3 transit hubs** (Nabadwip Dham Station, Baral Ferry Ghat, Bus Stand).
* **Hybrid Walking Navigation:** Tap any pin to preview the walking route and estimated time inside the app (with an automatic timeout fallback if OSRM is slow) or launch one-tap **Google Maps** turn-by-turn voice navigation.
* **Bilingual (English / বাংলা):** One-tap toggle switches headings, navigation, SOS contacts, festival rules, and food descriptions between English and Bengali.
* **Instant-Access SOS & Local Guide:** Direct `tel:` dial links for 112, Nabadwip Police Station, Nadia Police Control Room, Municipality, Women's Helpline, and Tourist Helpline, paired with crowd-safety guidelines and a 10-spot food guide.

---

## Tech Stack & UX Standards

* **Frontend:** HTML5, Tailwind CSS (CDN), Vanilla JavaScript
* **Mapping & Routing:** Leaflet.js, Leaflet Routing Machine (OSRM), Google Maps Deep Linking
* **Persistence:** Browser `localStorage` (visited checklist, language, and Night Mode preferences)
* **Accessibility & Mobile UX:** Minimum `44×44px` touch targets on interactive controls, `≥12px` outdoor-legible typography, high-contrast Dark Mode buttons/badges, and `prefers-reduced-motion` support.

---

## Running Locally

No build step or dependencies required:

1. Clone or download this repository.
2. Open `index.html` in any modern browser (or use the **Live Server** extension in VS Code).
