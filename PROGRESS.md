# Existence — Website Project

## Last Updated: March 27, 2026

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
Hook → Problem → Time Block → Solution (Cycle) → Product → Proof → CTA

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
- All DTS assets compressed (photos ~100KB, videos ~500KB)
- Squares have Time Block overlays (Holbrook Pond, Group Jog, Beach Sunset, Farmers Market, Meditation, Project Review)

### Section 2: Problem (2 versions, tabbed)
| Version | Content |
|---------|---------|
| **s2v1** | "There's a gap..." headline + 3 numbered pain points (.01, .02, .03) + animated graph SVG (intention vs. actual diverging lines) |
| **s2v2** | Single philosophical headline about patterns |

- White background, inverted tab colors
- Graph SVG animates: rings fade in smallest→largest, lines trim from bottom, gap arc trims from center

### Section 3: Time Block Flip
- Scroll-triggered 3D card flip
- Auto-flips once on scroll into view
- **Cursor-driven**: continuously rotates as cursor moves across section (left = front, right = back)
- Front face: `Editing Time Block.svg` (The Real You)
- Back face: `NEW-Block.png` with `run-sharp.mp4` playing behind (The Ideal You)
- Video darkened with 50% black overlay
- Copy cross-fades: active side = full opacity, inactive = 10%
- "Every Time Block holds both." tagline after flip
- Labels in Season Mix italic

### Section 4: Solution — The Cycle
- Engineer (blue `#8ab4f8`) / Record (amber `#e8a87c`) / Reveal (teal `#82d9c5`)
- 3-column cards with hover accent bars
- "See How It Works →" links to `v5.html`

### Section 5: Product Showcase
- Calendar week view (large) + mobile + insights (stacked right)

### Section 6: Social Proof
- Founding principle quote + placeholder press logos

### Section 7: Closing CTA
- "Your days are already shaping you. It's time to shape them back."

### Footer
- Minimal: logo, links, copyright

---

## How It Works (`v5.html`)

16-frame scroll narrative in 4 parts:
1. **The Time Block** (Frames 1-5) — What it is, what's inside it
2. **The Cycle** (Frames 6-9) — Engineer → Record → Reveal
3. **The Compounding** (Frames 10-12) — System in motion, patterns emerge
4. **The Outcome** (Frames 13-16) — Time Alignment, transformation, CTA

---

## 3D Experiment (`homepage-3d.html`)

Stripped version with only:
- s1v3 (B&W video bg + content squares)
- s2v1 (gap headline + graph)
- Minimal footer linking back to main homepage

Purpose: playground for 3D/immersive hero experiments

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

### Colors
- Background: `#050505`
- Text: `#ffffff` (pure white for headlines/buttons/logo)
- Body text: `#888` (gray) / `#ccc` (light sections)
- Engineer: `#8ab4f8`
- Record: `#e8a87c`
- Reveal: `#82d9c5`
- Problem section: white background, black/dark text

### Design Language
- Dark mode primary, white sections for contrast
- Scroll-reveal animations with `cubic-bezier(0.16, 1, 0.3, 1)`
- Subtle parallax on content squares
- CSS drop shadows (not baked into SVGs — removed from SVG sources)
- Grid motif (fullgrid.svg) as structural background element
- DTS lifestyle photography + video for visual proof
- Phone mockup with cycling screen videos for product demos

---

## Key Files

| File | Purpose |
|------|---------|
| `homepage.html` | **Main homepage** (all versions) |
| `homepage-3d.html` | 3D experiment (s1v3 + s2v1 only) |
| `homepage-framework.html` | Framework/wireframe document |
| `v5.html` | How It Works page |
| `NEW-Block.png` | Time Block card PNG (transparent image area for video) |
| `Editing Time Block.svg` | Time Block "lived" face |
| `TIME_BLOCK_INFO.svg` | Time Block "intended" face (has embedded video foreignObject) |
| `Graph-New.svg` | Intention vs. actual diverging lines graph |
| `right-squares.svg` | Hero content square layout |
| `fullgrid.svg` | Background grid pattern |
| `logo-existence.svg` | Existence logo |
| `phone-frame.webp` | iPhone bezel frame |
| `phone-screen-1-4.mp4` | Phone screen videos |
| `phone-hero-video.mp4` | Phone hero video |
| `dts-1.jpg` — `dts-4.jpg` | DTS lifestyle photos (compressed) |
| `dts-v1.mp4` — `dts-v3.mp4` | DTS lifestyle videos (compressed) |
| `dts-bg-video.mp4` | B&W DTS background video |
| `run-sharp.mp4` | Running video for Time Block flip |
| `hero-bg.mp4` | Hero background video |
| `fonts/` | Season Mix + Roobert |

---

## Run Locally
```
cd /Users/matthewbuchwach/Documents/claude/existence-how-it-works
python3 -m http.server 8111
# Homepage: http://localhost:8111/homepage.html
# How It Works: http://localhost:8111/v5.html
# 3D Experiment: http://localhost:8111/homepage-3d.html
```
