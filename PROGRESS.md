# Existence — How It Works Page

## Last Updated: March 24, 2026

---

## Project Location
`/Users/matthewbuchwach/Documents/claude/existence-how-it-works/`

## Run
```bash
cd /Users/matthewbuchwach/Documents/claude/existence-how-it-works
python3 -m http.server 8111
```
Then open:
- **V1**: http://localhost:8111/v1.html (or index.html — same file)
- **V2**: http://localhost:8111/v2.html

---

## What This Is

A scroll-driven "How It Works" page for **Existence** (existence.io), a Time Intelligence System. Inspired by Oura Ring's "How It Works" page but in the Existence design language (dark, cinematic, black & white, Season Mix + Roobert fonts).

The page explains the **Time Creation Cycle**: Engineer → Record → Reveal — the core loop of the product.

---

## Two Versions

### V1 (`v1.html` / `index.html`)
- **Central cycle** stays sticky in the viewport center, shrinking as you scroll
- Content panels branch off left and right from the cycle
- Cycle arcs glow when their corresponding step is active
- Sections: What It Is → Time Blocks → Engineer → Record → Reveal → DNA/Compounding → Outcomes → CTA

### V2 (`v2.html`) — Colleague's Vision (Active Development)
- **Oura-style cinematic scroll** with left rail progress indicator
- **Hero**: Full-bleed looping video with "existence" logo + opening statement
- **Scroll-driven mask transition**: Dark mask slides from left, hero video fades, square video + content fades in
- **Left rail**: Sticky ENGINEER → RECORD → REVEAL progress nav (like Oura's time-of-day rail)
- Frame-by-frame scroll journey:
  1. Hero video + "Most people never see..."
  2. Mask wipe → "Existence shows you how it's created" + Time Intelligence System features + square video with Time Block overlay
  3. Cycle animation (draws itself)
  4. Engineer step (Time Blocks cascade in)
  5. Expanded Time Block micro-moment
  6. Record step (Intended vs Actual split view + Quality Score)
  7. Reveal step (Data Explorer, AI Summaries, "E")
  8. Loop closes — "system in motion"
  9. Multiplication — stacking loops
  10. Patterns emerge — heat grid
  11. Identity — DNA helix
  12. Gap closing — intention vs actual bars
  13. Time Alignment — balanced pillars
  14. CTA — "Start Creating Time"

---

## Design Language

### Fonts
- **Headlines**: Season Mix Regular (no bold)
- **Body/UI**: Roobert Regular, Light, Medium
- Font files in `fonts/` directory

### Colors
- Pure black & white — no color accents
- `--black: #050505`
- `--white: #f5f2ed`
- `--gray: #666`
- Subtle rgba white variations for borders, backgrounds, dim states

### Vibe
- Matches existence.io — dark, cinematic, minimal
- Scroll-driven animations (IntersectionObserver + scroll position tracking)
- Elements fade up with staggered delays (`data-fade-order`)
- No libraries — pure vanilla HTML/CSS/JS

---

## Key Files

| File | Purpose |
|------|---------|
| `v1.html` | Version 1 — central sticky cycle approach |
| `v2.html` | Version 2 — Oura-style left rail + cinematic scroll (active) |
| `index.html` | Copy of v1 |
| `hero-bg.mp4` | Compressed hero video (from DTS_IRL_ESCAPISM_ID135.mov) |
| `system-bg.mp4` | Square 1:1 video (from DTS_IRL_ESCAPISM_ID138.mov) |
| `hash-frame.svg` | Corner bracket frame overlay for square video |
| `fonts/` | Season Mix + Roobert font files |
| `PROGRESS.md` | This file |

---

## Video Sources (on T7 drive)
- Hero: `/Volumes/T7/Ex Videos/DTS_IRL_ESCAPISM_Joey_Bania_Clips_ID135.mov`
- Square: `/Volumes/T7/Ex Videos/DTS_IRL_ESCAPISM_Joey_Bania_Clips_ID138.mov`
- Hash frame: `/Volumes/T7/Ex Videos/Hash_2.svg`

---

## Reference
- **Existence site**: https://www.existence.io/
- **Time Creationism site**: https://time-creationism.webflow.io/ (password: 24022026)
- **Oura inspiration**: https://ouraring.com/how-it-works
- **Product content source**: Full "How It Works" copy provided by user in conversation

---

## What's Next / TODO
- [ ] Refine scroll timing on V2 hero transition
- [ ] Left rail behavior after cycle sections (currently hides)
- [ ] More video clips for different sections
- [ ] Engineer section — animate calendar → Time Block transformation
- [ ] Record section — make the split view feel more tactile
- [ ] Mobile responsive pass
- [ ] Potential deployment (user declined Vercel for now)
