# MZ1312 // ECOSYSTEM COMMAND CENTER

> **1312 — LOCAL PROCESSING — ZERO CLOUD — TOTAL SOVEREIGNTY**

The single pane of glass for the entire **MZ1312 UNCAGED TECHNOLOGY** stack — and a self-contained **application**, not a page of links. Every tool, dashboard and feature is built *into* the file: the full Oracle betting engine, Ghost Protocol hardware line, a live 3D Vivi avatar, a working Claude chat, the 36-design Canva gallery, the investor pitch deck and business plan — all embedded, nothing linked away.

Design language: **NASA Mission Control × Bloomberg Terminal × Minority Report.**

🔗 **Live:** https://thotsl4yer69.github.io/mz1312-dashboard/

---

## What it is

A single `index.html`. Zero build step. Open it and the whole ecosystem is in front of you — 21 sections, real GitHub + weather data, a `<canvas>` device mesh, an interactive 3D avatar, and a dozen genuinely-functional tools. The only external dependencies are two CDN libraries: **Chart.js** and **Three.js**.

## Sections (21)

| # | Section | Built-in tooling |
|---|---------|------------------|
| 01 | **Overview** | Ecosystem KPIs, system health bars, jump-to-tool launcher, today snapshot |
| 02 | **Drifter** | Live animated telemetry gauges, fuel trims, Vivi status, 42-service mesh, live alerts |
| 03 | **Device Mesh** | Animated node topology with live MQTT packet flow + per-device cards |
| 04 | **Repos** | Live GitHub API — stars, branch, open PRs, last commit **+ commit-activity sparklines** |
| 05 | **Oracle** | **Full engine** — value bets, ELO ladders, **Poisson score matrix**, **SGM builder**, **Kelly calculator**, CLV tracker, bet log, fixtures with kickoff countdowns |
| 06 | **UNORTHODOXED** | 8-product store with a **working cart**, drop countdown, revenue |
| 07 | **Ghost Protocol** | RF spectrum monitor, BLE scan, ALPR, CAN mode selector, **inline SVG hardware renders** |
| 08 | **Vivi AI** | **Live 3D avatar (Three.js + GLTFLoader)**, OrbitControls, breathing + blink, **working Claude chat**, voice pipeline |
| 09 | **MYCILLIYUMS** | Foraging prediction heatmap, in-season species, conditions |
| 10 | **Diagnostics** | **Searchable X-Type DTC database** + AJ-V6 PID reference + Jaguar quirks |
| 11 | **Wiring** | **Interactive SVG harness** — click any node for its pinout/gauge/routing |
| 12 | **Troubleshooting** | Tabbed decision-tree **flowcharts** (won't start / Vivi silent / no CAN / overheating) |
| 13 | **Deploy** | Copy-ready SSH command deck + **simulated console** |
| 14 | **Briefing** | Vivi's morning brief (live weather), agenda, conditions |
| 15 | **Finance** | Hardware spend table, revenue projection chart, betting P&L + discreet legal tracker |
| 16 | **Docs** | Every spec, guide and diagram |
| 17 | **Brands** | Guides, decks, lookbooks |
| 18 | **Design Gallery** | **36 embedded Canva designs**, 9 sets, A/B/C/D options, category filters, **★ favourites** |
| 19 | **Pitch & Plan** | **Embedded investor pitch deck** (slides) + **business plan** |
| 20 | **Hardware** | BOM + Ghost Protocol product line + 3D/wiring links |
| 21 | **Analytics** | 52-week contribution heatmap, codebase stats, language donut |

## Headline features

- **Live 3D Vivi avatar** — Three.js + GLTFLoader loads `vivi_avatar.glb`, OrbitControls (drag/zoom), amber-tinted lighting, procedural breathing + eye-blink. Falls back to a procedural crystalline avatar, then to text, if WebGL or the model is unavailable.
- **Working Vivi chat** — set an Anthropic API key in **⚙️ Settings** (stored in `localStorage`) and Vivi answers via the Claude API with her own system prompt; otherwise a built-in local demo responds. Uses `anthropic-dangerous-direct-browser-access`.
- **Real Oracle engine** — Poisson score-probability matrix, ELO ladders, correlation-aware SGM builder, fractional Kelly calculator, CLV chart — all compute live in-browser.
- **36-design Canva gallery** — every generated design embedded as a lazy-loaded preview, grouped by Ghost Protocol Hardware / UNORTHODOXED Clothing / Brand Lookbook, with A/B/C/D labels and a **favourites** system.
- **Live data** — GitHub repo stats + commit sparklines, and **Melbourne weather** via the free Open-Meteo API (no key).
- **Konami code** (↑↑↓↓←→←→BA) — Vivi pops a speech bubble and her eyes glow.
- **Productivity** — autosaving **notepad** (`N`), persistent **deploy checklist** (`D`), **session timer**, particle background, global search.
- **Keyboard-driven** — `1`–`9` jump, `/` search, `N` notepad, `D` deploy, `gg`/`G` top/bottom, `p` print, `?` help.
- **Print CSS** for clean PDF export · **dark mode only** — this is mission control.

## Keyboard shortcuts

| Key | Action | Key | Action |
|-----|--------|-----|--------|
| `1`–`9` | Jump to section | `N` | Notepad |
| `/` | Global search | `D` | Deploy checklist |
| `g g` | Top | `G` | Bottom |
| `p` | Print / PDF | `?` | Help |
| `↑↑↓↓←→←→BA` | 😏 | `Esc` | Blur input |

## Running locally

```bash
git clone https://github.com/thotsl4yer69/mz1312-dashboard.git
cd mz1312-dashboard
python -m http.server 8080   # serve so GLB + API fetches work cleanly
# visit http://localhost:8080
```

> Serve over `http://` rather than `file://` so the 3D model and GitHub/weather fetches load without browser restrictions.

## Configuring the Claude chat

1. Click the **⚙️** gear in the command bar.
2. Paste your Anthropic API key and pick a model (default Sonnet 4.6).
3. The key lives only in this browser's `localStorage` and is sent **directly** to Anthropic. Use only on a device you trust.

## The ecosystem

`drifter` · `oracle` · `unorthodoxed` · `mz1312-orchestrator` · `mz1312-dashboard` · `sentient-core` · `mycelium-mapper`

## Design tokens

```
--bg-void:#080B14  --blue:#3B82F6  --amber:#FF8C00
--purple:#8B5CF6   --green:#22C55E --red:#EF4444  --cyan:#22D3EE
fonts: Inter (UI) · JetBrains Mono (data)
```

---

© 2026 **MZ1312 UNCAGED TECHNOLOGY** · built with Claude Code · *the boulder never stops.*
