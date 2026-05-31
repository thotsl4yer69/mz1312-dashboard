# MZ1312 // ECOSYSTEM COMMAND CENTER

> **1312 — LOCAL PROCESSING — ZERO CLOUD — TOTAL SOVEREIGNTY**

The single pane of glass for the entire **MZ1312 UNCAGED TECHNOLOGY** stack. One enormous, self-contained mission-control dashboard — the one place to **see, access, and manage everything** across the ecosystem.

Design language: **NASA Mission Control × Bloomberg Terminal × Minority Report.**

🔗 **Live:** https://thotsl4yer69.github.io/mz1312-dashboard/

---

## What it is

A single `index.html` file. Zero build step. No dependencies to install. Open it and the whole ecosystem is in front of you — deep-space dark, glassmorphism cards, live gauges, an animated device-mesh canvas, and real GitHub data pulled straight from the public API.

## Sections

| # | Section | What it shows |
|---|---------|---------------|
| 01 | **Command Bar** | Logo, Melbourne clock, global search, pulsing device status lights |
| 02 | **Drifter Vehicle Intelligence** | Live telemetry gauges (RPM/speed/coolant/voltage), fuel trims, Vivi co-pilot status, 42-service mesh, live alert feed, CAN + Ghost Protocol status |
| 03 | **Device Mesh** | Animated node topology with live MQTT packet flow, per-device CPU/RAM/heartbeat, deploy buttons |
| 04 | **GitHub Repos** | Live cards for all 7 repos — stars, branch, open PRs, last commit (fetched from the GitHub API) |
| 05 | **Oracle Betting** | Bankroll, P&L, strike rate, today's top value bets, NRL/AFL model confidence, 30-day bankroll curve |
| 06 | **UNORTHODOXED** | 8-product catalogue, stock status, next-drop countdown, revenue tracker |
| 07 | **Ghost Protocol** | RF spectrum monitor, BLE tracker scan, ALPR awareness, CAN toolkit mode selector |
| 08 | **Vivi AI** | Personality stats, memory/usage, voice pipeline (Whisper→Claude/Ollama→Piper), live query box |
| 09 | **MYCILLIYUMS** | Foraging prediction heatmap, in-season species, weather conditions, sighting counts |
| 10 | **Documentation Hub** | Cards for API reference, Pi5 setup, troubleshooting, wiring, architecture, security audit + more |
| 11 | **Tools & Utilities** | Deploy buttons (Drifter / Cortana / Docker / Hermes) and quick actions (tests, NRL scan, health, briefing) |
| 12 | **Brands** | Brand guides, pitch deck, lookbook, ecosystem map |
| 13 | **Hardware** | Full bill of materials + Ghost Protocol product line + 3D-print / wiring links |
| 14 | **Analytics** | 52-week contribution heatmap, task tracker, codebase stats, language donut, uptime |
| 15 | **Footer** | The doctrine, session stats, links to every live site |

## Features

- **Single HTML file, zero build** — pure HTML/CSS/JS + [Chart.js](https://www.chartjs.org/) via CDN.
- **Live GitHub data** — fetches repo stars, branches, PRs and last-commit times from the public API (no auth).
- **Animated everything** — SVG gauges, a `<canvas>` device-mesh with travelling MQTT packets, count-up metrics, pulsing status lights.
- **Mission-control aesthetic** — deep space black `#080B14`, electric blue, amber (Drifter/alerts), purple (UNORTHODOXED), green (healthy), red (issues). Inter + JetBrains Mono. Glassmorphism with backdrop blur.
- **Responsive CSS grid** — collapses cleanly from ultrawide down to mobile.
- **Auto-refresh** — telemetry, services, alerts, RF spectrum and status lights update live on 2–9s intervals.
- **Keyboard-driven** — `1`–`9` jump to sections, `/` focuses search, `gg` top, `G` bottom, `p` print, `?` help.
- **Print CSS** — clean PDF export for briefings.
- **Dark mode only** — this is mission control, not a website.

## Keyboard shortcuts

| Key | Action |
|-----|--------|
| `1`–`9` | Jump to section |
| `/` | Focus global search |
| `g g` | Scroll to top |
| `G` | Scroll to bottom |
| `p` | Print / export PDF |
| `?` | Show shortcut help |
| `Esc` | Blur the focused input |

## The ecosystem

- **drifter** — 2002 Jaguar X-Type vehicle-intelligence OS (CAN, Vivi co-pilot, Ghost Protocol)
- **oracle** — NRL + AFL value-betting model and bankroll engine
- **unorthodoxed** — UNCAGED streetwear storefront
- **mz1312-orchestrator** — cross-project agent orchestrator
- **mz1312-dashboard** — this command center
- **sentient-core** — local-first memory/personality core for Vivi
- **mycelium-mapper** — foraging prediction engine

## Running locally

```bash
git clone https://github.com/thotsl4yer69/mz1312-dashboard.git
cd mz1312-dashboard
# just open it
start index.html        # Windows
# or serve for the GitHub API fetch to work cleanly:
python -m http.server 8080   # then visit http://localhost:8080
```

> Opening directly from `file://` works, but serving over `http://` avoids any browser fetch restrictions on the GitHub API calls.

## Wiring it to real data

Everything ships with believable demo data so the dashboard is alive out of the box. To make it real:

- **Telemetry / services / alerts** — point the `data-live` updaters at your Drifter MQTT bridge or REST endpoint.
- **Device mesh** — feed real heartbeat/CPU/RAM into the `NODES` array.
- **Oracle / Vivi / Ghost / Mycelium** — replace the placeholder arrays and the `data-demo` link targets with live URLs.
- **GitHub** — already live; just keep the repos public.

## Design tokens

```
--bg-void:#080B14  --blue:#3B82F6  --amber:#FF8C00
--purple:#8B5CF6   --green:#22C55E --red:#EF4444
fonts: Inter (UI) · JetBrains Mono (data)
```

---

© 2026 **MZ1312 UNCAGED TECHNOLOGY** · built with Claude Code · *the boulder never stops.*
