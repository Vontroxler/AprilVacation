# CLAUDE.md — AprilVacation

This project is a single-file trip planner for a Panama City Beach group vacation (April 6–11, 2026) shared with the group via GitHub Pages.

## File

- `index.html` — the entire site: HTML, CSS, and JS all inline, no build tools or external dependencies

## Design

- Beach/vacation aesthetic with ocean color palette and warm body text
- CSS custom properties for light/dark mode (`prefers-color-scheme`)
- Mobile-first, responsive; sticky fixed nav bar
- Sections are collapsible; all start collapsed by default
- Clicking a nav link expands the target section and scrolls to it
- Interactive packing checklist with `localStorage` persistence
- Print-friendly `@media print` stylesheet (hides nav and link pills)

## Links

Two pill-style link types appear inline throughout the content:
- `.map-link` (teal) — Google Maps search URL: `https://www.google.com/maps/search/?api=1&query=PLACE+NAME`
- `.web-link` (blue) — official website link

Both use inline SVG icons (`fill="currentColor"`) so they theme correctly in dark mode. Special chars in Maps queries must be URL-encoded (`'` → `%27`, `&` → `%26`).

The Gulf Coast Salute website link was removed (domain was not resolving as of March 2026 — re-add when confirmed working).

## Content

Source markdown: `compass_artifact_wf-d6989072-a52f-42db-90e5-7c0f8d80285d_text_markdown.md`

Sections (with HTML `id`):
1. `#weather` — Weather tables and forecasts
2. `#drive` — Route, departure, gas stops (gas calc: 1 vehicle, 22 MPG, 1,200 mi round trip)
3. `#events` — Air Show and local events
4. `#food` — Restaurants and budget dining guide
5. `#activities` — Free and paid activities
6. `#packing` — Interactive packing checklist
7. `#costs` — Full cost breakdown (totals: $980–$1,725 excl. lodging; ~$22–38/person/day)
8. `#safety` — Beach flags, tides, groceries, medical
9. `#itinerary` — Day-by-day cards

## Deployment

Hosted on GitHub Pages from the `main` branch. To preview locally, open `index.html` directly in Firefox.
