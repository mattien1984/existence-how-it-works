# Existence — How It Works Page

## Last Updated: March 26, 2026

---

## Versions

| Version | File | Description |
|---------|------|-------------|
| V1 | `v1.html` | Central sticky cycle with branching content panels, cycle shrinks on scroll |
| V2 | `v2.html` | Oura-style left rail + cinematic hero video transition |
| V3 | `v3.html` | Hero video mask wipe → headline → cycle rotate-in → pinned left circle with right panels |
| V4 | `v4.html` | **CURRENT** — Time Block hero with inline SVG highlighting, scroll-driven feature reveal |

## Live URL
**https://mattien1984.github.io/existence-how-it-works/**
Password: `existence2026`

V1 also live: **https://mattien1984.github.io/existence-how-it-works/v1-encrypted.html**

To update live site:
```
cd /Users/matthewbuchwach/Documents/claude/existence-how-it-works
npx staticrypt v4.html -p existence2026 --short
cp encrypted/v4.html index.html && rm -rf encrypted/
git add index.html v4.html && git commit -m "Update" && git push
```

---

## V4 — Current State

### What's Built

**Hero Section (scroll-driven, 500vh)**
- Blurred calendar screenshot background with dark overlay
- "existence" logo at top center, fades with hero text
- Hero text: "Everything you will ever do happens inside a unit of time."
- Scroll indicator chevron (bounces, fades on scroll)
- On scroll: hero text fades → Time Block SVG pulls in from right → left text appears

**Time Block Feature Panels (inside hero sticky frame)**
- Left side panels swap in-place with fade-up animation:
  - Panel 0: "A Time Block captures both what you intended to do and how it was actually lived."
  - Panel 1: When — clock icon (Time.svg)
  - Panel 2: What — document icon (what.svg)
  - Panel 3: Where — pin icon (Where.svg)
  - Panel 4: Who — people icon (whowith.svg)
- Right side: TIME-BLOCK.svg (Figma export, inlined) stays pinned
- SVG region highlighting: active group at opacity 1 + glow, everything else dims to 0.12

**Inline SVG Groups (targetable by JS)**
- `#tb-hero` — photo/header area
- `#tb-what` — title/activity text
- `#tb-when` — time/date row
- `#tb-pillar` — Work/Life/Health/Sleep buttons
- `#tb-who` — people row
- `#tb-where` — place row
- `#tb-quality` — right sidebar quality score

**Cycle Section**
- "At the center is a continuous cycle" bridge
- Sticky cycle (cycle.svg) with Engineer/Record/Reveal
- Active step highlights blue, inactive dims
- Right-side panels swap with content for each step

**Post-Cycle**
- Loop closes, multiplication, patterns, alignment, Time Alignment, CTA

**Left Rail Nav**
- Sticky vertical progress bar with ENGINEER / RECORD / REVEAL
- White dot fills as you scroll

---

### Still TODO

**Part 1 — Time Block**
- [ ] Duality section: "ideal you / real you" (Quality Score, Reflection, Media)
- [ ] Scale up: one block → many → day timeline
- [ ] Pillar highlighting

**Part 2 — Cycle**
- [ ] Real app screenshots for Engineer/Record/Reveal panels

**Part 3 — Outcomes**
- [ ] Time Alignment visualization
- [ ] Gap closing animation

**General**
- [ ] Mobile responsive
- [ ] Replace mock UI with Figma exports
- [ ] Final copy review
- [ ] Push encrypted v4 to GitHub Pages

---

## Key Files

| File | Purpose |
|------|---------|
| `v4.html` | Current working version |
| `TIME-BLOCK.svg` | Figma Time Block card (inlined in v4) |
| `Time.svg` / `what.svg` / `Where.svg` / `whowith.svg` | Feature icons |
| `cycle.svg` | Engineer→Record→Reveal circle |
| `calendar-bg-blur.jpg` | Blurred app screenshot for hero bg |
| `fonts/` | Season Mix + Roobert |

## Fonts
- Headlines: Season Mix Regular (serif)
- Body: Roobert Regular (sans)

## Colors
- Background: `#050505`
- Text: `#ffffff` / `#f5f2eb`
- Engineer: `#8ab4f8`
- Record: `#e8a87c`
- Reveal: `#82d9c5`

## Run Locally
```
cd /Users/matthewbuchwach/Documents/claude/existence-how-it-works
python3 -m http.server 8111
# Open http://localhost:8111/v4.html
```
