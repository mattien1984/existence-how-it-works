# Existence — Website Project

## Last Updated: March 30, 2026

---

## Project Structure

### Two Main Pages
1. **Homepage** (`homepage.html`) — Landing page to hook users, articulate the problem, introduce the solution
2. **How It Works** (`v5.html`) — Deep dive into the Time Creation Cycle, Time Blocks, Engineer/Record/Reveal

### Experimental
3. **3D Experiment** (`homepage-3d.html`) — Stripped to s1v3 + s2v1 only, playground for 3D/immersive ideas

---

## Homepage (`homepage.html`)

### Narrative Structure
Hook → Phone Intro → Problem → Time Block → Solution (Cycle) → Product → CTA

### Section 1: Hero (5 versions, tabbed)
| Version | Background | Copy |
|---------|-----------|------|
| **s1v1** | Full-bleed `hero-bg.mp4` video | "Structure your time. Record how it's lived. Reveal who you're becoming." |
| **s1v2** | Grid + DTS content squares (6 squares with Time Block overlays, parallax on scroll) | "Record your days. Remember each moment. Reimagine your existence." |
| **s1v3** | B&W DTS video bg (`dts-bg-video.mp4`) + content squares | Same as v2 |
| **s1v4** | Grid SVG + animated spotlight + phone mockup (right side) | Same as v1 copy, text shifted right |
| **s1v5** | Blurred hero image (`existence-hero-grid.jpg`) + phone mockup | Same as v1 copy, text shifted right |

- Version tabs on left side, white stroke on active
- Site always loads on v1
- Phone mockup cycles through 5 screen videos with dot navigation
- DTS square assets: `dts-1.jpg` through `dts-4.jpg`, `dts-v1.mp4`, `dts-v2.mp4`, `dts-v3.mp4`

### Section 2: Phone Intro (4 versions, tabbed)
| Version | Content |
|---------|---------|
| **v1** | Single phone with video + headline + subhead + CTA |
| **v2** | Full phone with video + headline + subhead + CTA |
| **v3** | Two phones image + headline + subhead + CTA |
| **v4** | 3-column value props with thumbnail images (thumb01/02/03.png) |

- White background with `grid-try.png` grid pattern overlay
- Headline: "With Existence, time isn't only something you manage, it's something you create."
- Subhead: "A time intelligence system that captures every dimension of your life — then shows you what it all means."
- V4 columns: "Account for all of your time" / "See what no calendar can show you" / "A system that gets smarter with you"
- V4 subtext: Roobert Light, #222, line-height 1.35

### Section 3: Problem (3 versions, tabbed)
| Version | Content |
|---------|---------|
| **s2v1** | "There's a gap..." headline + 3 numbered pain points + animated graph SVG |
| **s2v2** | Single philosophical headline about patterns |
| **s2v3** | Stacked time blocks SVG composition |

- White background, inverted tab colors

### Section 4: Time Block Flip
- Scroll-triggered 3D card flip (cursor-driven continuous rotation)
- Front face: `Editing Time Block.svg` (The Real You)
- Back face: `NEW-Block.png` with `run-sharp.mp4` playing behind (The Ideal You)

### Section 5: Time Creation Cycle (scroll-pinned)
- Background: `runners.jpg` with dark overlay
- 400vh scroll-pin with sticky inner
- Left column: "The Time Creation Cycle" title + animated cycle SVG diagram
- Right column: 3 panels crossfade on scroll (Engineer → Record → Reveal)

#### Engineer Panel (01)
- Number/subtitle in **Roobert Semi Mono**, uppercase, #A4A7AE
- Custom SVG icons in fixed 24px containers:
  - `pillars.svg` → Set your pillar intentions (Work/Life/Health/Sleep split)
  - `timeblocksi.svg` → Create Time Blocks with tags (Activities, People, Places)
  - `favu.svg` → Favorites — place your most-used blocks in one touch
  - `stack.svg` → Recurring blocks = your Rhythm
- Animated pillar sliders below

#### Record Panel (02)
- Same Roobert Semi Mono number/subtitle styling
- Custom SVG icons at 16px height:
  - `Aassets/Energy1.svg` → Quality Score — rate intention vs. reality (0–10)
  - `reflection1.svg` → Reflections — capture meaning while it's fresh
  - `Media1.svg` → Photos & media — memorialize the moment
  - `Edit1.svg` → Update what actually happened — when, what, who, where
- `record-asset.png` below bullet points (80% width, nudged left/up)

#### Reveal Panel (03)
- Same Roobert Semi Mono number/subtitle styling
- Custom SVG icons in fixed 24px containers:
  - `insightys.svg` → Time Insights — weekly, monthly, yearly summaries
  - `time2.svg` → Time Alignment Score — intention vs. creation
  - `Aassets/Search + Assistant.svg` → E — your AI time companion
  - `explorer.svg` → Time Explorer — filter by activity, people, places
- `reveal-callouts.png` below

### Section 6: Product Showcase
- Headline: "Every dimension of your time captured in one place." (Season Mix, clamp 29px–50px)
- Subhead: "What you did, when, where, with whom, and how it felt. Intention on one side, reality on the other." (Roobert Light 16px, #aaa)
- 3 staggered product images with white glow drop-shadows:
  - `feat-1.png` — large dashboard (80% width, left)
  - `feat-3.png` — square card (30% width, top right)
  - `feat-2.png` — wide card (30% width, bottom right)
- Staggered reveal animations on each image

### Section 7: Closing CTA
- "Your days are already shaping you. It's time to shape them back."
- "Apply to Join" button

### Footer
- Minimal: logo, links (How It Works, About, Privacy, Terms), copyright

---

## How It Works (`v5.html`)

16-frame scroll narrative in 4 parts:
1. **The Time Block** (Frames 1-5) — What it is, what's inside it
2. **The Cycle** (Frames 6-9) — Engineer → Record → Reveal
3. **The Compounding** (Frames 10-12) — System in motion, patterns emerge
4. **The Outcome** (Frames 13-16) — Time Alignment, transformation, CTA

---

## Live URLs
- **Homepage**: https://mattien1984.github.io/existence-how-it-works/homepage.html
- **How It Works**: https://mattien1984.github.io/existence-how-it-works/v5.html
- **3D Experiment**: https://mattien1984.github.io/existence-how-it-works/homepage-3d.html

---

## Brand & Design

### Fonts
- Headlines: **Season Mix** Regular/Italic (serif)
- Body/UI: **Roobert** Light/Regular/Medium (sans)
- Labels/Tags: **Roobert Semi Mono** Regular (mono) — used for section numbers, subtitles in S5

### Colors
- Background: `#050505`
- Text: `#ffffff` (pure white for headlines/buttons/logo)
- Body text: `#888` (gray) / `#ccc` (light sections)
- Section labels: `#A4A7AE` (Roobert Semi Mono elements)
- Engineer: `#8ab4f8`
- Record: `#e8a87c`
- Reveal: `#82d9c5`
- Problem section: white background, black/dark text
- S2 V4 subtext: `#222`

### Design Language
- Dark mode primary, white sections for contrast
- Scroll-reveal animations with `cubic-bezier(0.16, 1, 0.3, 1)`
- Subtle parallax on content squares
- White glow drop-shadows on product images (`drop-shadow(0 0 40px rgba(255,255,255,0.14))`)
- Grid motif (`grid-try.png`) as Section 2 background
- DTS lifestyle photography + video for visual proof
- Phone mockup with cycling screen videos for product demos

---

## Key Files

| File | Purpose |
|------|---------|
| `homepage.html` | **Main homepage** (all versions) |
| `homepage-3d.html` | 3D experiment (s1v3 + s2v1 only) |
| `v5.html` | How It Works page |
| `feat-1.png` | Product showcase: large dashboard |
| `feat-2.png` | Product showcase: wide insights card |
| `feat-3.png` | Product showcase: square time block card |
| `thumb01.png` | S2 V4: "Account for all of your time" |
| `thumb02.png` | S2 V4: "See what no calendar can show you" |
| `thumb03.png` | S2 V4: "A system that gets smarter with you" |
| `grid-try.png` | Section 2 grid background (3840×2160) |
| `record-asset.png` | Record panel visual |
| `pillars.svg` | Icon: pillar intentions |
| `timeblocksi.svg` | Icon: time blocks |
| `favu.svg` | Icon: favorites |
| `stack.svg` | Icon: recurring blocks |
| `insightys.svg` | Icon: time insights |
| `time2.svg` | Icon: time alignment |
| `explorer.svg` | Icon: time explorer |
| `Edit1.svg` | Icon: edit/update |
| `reflection1.svg` | Icon: reflections |
| `Media1.svg` | Icon: photos & media |
| `Aassets/Energy1.svg` | Icon: quality score |
| `Aassets/Search + Assistant.svg` | Icon: E AI companion |
| `Aassets/TB.svg` | Icon: time blocks (alt) |
| `fonts/RoobertSemiMonoTRIAL-Regular.otf` | Roobert Semi Mono font |
| `fonts/` | Season Mix + Roobert + Roobert Semi Mono |

---

## Run Locally
```
cd /Users/matthewbuchwach/Documents/claude/existence-how-it-works
python3 -m http.server 8111
# Homepage: http://localhost:8111/homepage.html
# How It Works: http://localhost:8111/v5.html
# 3D Experiment: http://localhost:8111/homepage-3d.html
```
