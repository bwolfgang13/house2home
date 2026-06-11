# House2Home — Design Sprint Prototype

## What this project is

**Springboard UX/UI bootcamp assignment** — a modified solo GV 5-day design sprint.

**Product:** House2Home — a platform that helps people who feel overwhelmed by decorating confidently style their space. Core value: a curated "starter kit" of 3 items (a print, a light, an accessory) matched to the user's style and budget ($10–$50 each).

**Core insight:** The problem isn't just finding items — it's lack of confidence. The product must provide direction, not just options.

---

## Current state

### What's been built
- `Day 5/House2home Hi-Fi.html` — the original 16-screen design canvas (pannable/zoomable, like Figma). Direction A only; Direction B lives in `Day 5/House2home Hi-Fi B.html`.
- `index.html` — **clickable prototype** at the repo root. Single self-contained React/Babel file. This is the live deliverable.

### Live URL
`https://bwolfgang13.github.io/house2home/`

### GitHub repo
`https://github.com/bwolfgang13/house2home`

### How to push changes
```
cd "/Users/benjaminwolfgang/Documents/Springboard/Design Sprint"
git add index.html
git commit -m "your message"
git push origin main
```
Username: `bwolfgang13` — use a personal access token as the password (github.com → Settings → Developer settings → Tokens (classic) → repo scope).

---

## Prototype — screen flow (in order)

1. **Landing** → "Find my style →" → Q1
2. **Q1 — Feeling** (6 vibe cards, multi-select) → Next → Q2
3. **Q2 — Color Palette** (4 palettes, single-select) → Next → Q3
4. **Q3 — Textures** (3 horizontal bands, multi-select) → Next → Q4
5. **Q4 — Mood** (2 split options, single-select) → Next → Q5
6. **Q5 — Words** (18 word pills, multi-select) → Next → Q6
7. **Q6 — Priority** (4 cards, single-select) → "See my style →" → Style Result
8. **Style Result** — "Modern Warm" → "Pick my starter pack →" → Pack R1
9. **Pack Round 1** (A vs B) → Pack R2
10. **Pack Round 2** (winner vs C) → Pack R3
11. **Pack Round 3** (winner vs D) → Pack Reveal
12. **Pack Reveal** — "Add to Cart →" → Cart | "Try in My Room" → AR screen
13. **AR / Try in Room** — "Continue to cart →" → Cart
14. **Cart + Add-ons** — "Proceed to checkout →" → Checkout
15. **Checkout** — "Place order →" → Order Confirmation
16. **Order Confirmation** — end state

### Interactivity
- **Quiz screens:** Selections are clickable and visually highlight. Multi-select: Q1, Q3, Q5. Single-select: Q2, Q4, Q6.
- **Quiz pre-seeded** with coherent Modern Warm answers for demo storytelling (user can override).
- **Pack tournament:** Live — choosing a pack actually advances it.
- **Demo path:** Style always resolves to "Modern Warm." Pack always reveals "The Soft Studio" (Pack D).
- **Cart/Checkout:** Static pre-filled fields.

---

## Design system

### Colors (current — as implemented in index.html)
```
bg:          #FAFAF8   (off-white, page background)
paper:       #FFFFFF   (card/surface background)
ink:         #1C1C1A   (primary text)
inkMid:      #888884   (secondary text)
inkLight:    #767672   (labels, captions — WCAG AA compliant)
accent:      #5A7A5A   (sage — CTAs, selected states, brand — WCAG AA ~4.8:1)
accentLight: #D4E4D4   (accent tint — decorative corners)
accentBg:    #EFF5EF   (accent wash — selected card bg, tag bg)
border:      #E4E0DA   (standard border)
borderLight: #F0EDE8   (subtle dividers)
```

### Typography
- **Serif:** Playfair Display, weight 300 (light) — headlines, pack names, brand mark
- **Sans:** Lato, weights 300/400/500 — all body text, labels, buttons
- Load via: `https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,300;0,400;0,500;1,300;1,400;1,500&family=Lato:wght@300;400;500&display=swap`

### Design rules
- No border-radius on cards or buttons (squared corners only)
- 0.5px borders throughout
- Selected state: `1.5px solid #5A7A5A` border + `0 4px 16px rgba(122,154,122,0.14)` shadow
- Multi-select affordance: square checkbox indicator (always visible — outlined when unselected, filled when selected)
- Single-select affordance: circular indicator (appears only when selected)
- No icons or emoji in UI
- Font floor: 11px minimum
- All flow screens: 800px tall, 1280px wide. Landing: 820px tall, 1440px wide.
- Brand mark: `house` + `<span accent>2</span>` + `home` in Playfair Display 300

### Naming model
- **Style** = "Modern Warm" (quiz result, always pre-wired)
- **Pack** = "The Soft Studio" (tournament winner, always pre-wired)
- These are distinct concepts — keep them clearly separate in copy

---

## Pack data

```
Pack A — The Calm Edit      ($79)   minimal · neutral · airy
  Print:     Abstract Minimal No. 3   $24
  Light:     Woven Pendant Shade      $38
  Accessory: Ceramic Bud Vase         $17

Pack B — The Bold Layer     ($94)   textured · contrast · statement
  Print:     Geometric Statement Print  $28
  Light:     Arc Floor Lamp             $44
  Accessory: Woven Storage Basket       $22

Pack C — The Earthy Mix     ($78)   natural · organic · grounded
  Print:     Botanical Study I        $22
  Light:     Terracotta Table Lamp    $38
  Accessory: Rattan Tray              $18

Pack D — The Soft Studio    ($85)   soft · refined · structured  ← demo winner
  Print:     Line Art Figure Study    $24
  Light:     Slim Column Table Lamp   $44
  Accessory: Boucle Throw Pillow      $17
```

---

## Unsplash photo IDs
URL pattern: `https://images.unsplash.com/photo-{ID}?auto=format&fit=crop&w={W}&h={H}&q=70`

```
hero / airy:     1616594039964-ae9021a400a0
modernWarm:      1493663284031-b7e3aefcae8e
calm (Pack A):   1616486338812-3dadae4b4ace
bold (Pack B):   1532323544230-7191fd51bc1b
earthy (Pack C): 1586023492125-27b2c045efd7
studio (Pack D): 1583845112203-29329902332e
packAll:         1631679706909-1844bbd07221
textureRaw:      1505693416388-ac5ce068fe85
textureSoft:     1611117775350-ac3950990985
textureSmooth:   1505691723518-36a5ac3be353
cozy:            1522708323590-d24dbb6b0267
minimal:         1502005229762-cf1b2da7c5d6
eclectic:        1564540583246-934409427776
natural:         1505873242700-f289a29e1e0f
modern:          1565538810643-b5bdb714032a
vintage:         1560448204-e02f11c3d0e2
enveloping:      1522708323590-d24dbb6b0267
tableRunner:     1604147706283-d7119b5b822c
blackFrame:      1513519245088-0e12902e5a38
candles:         1603006905003-be475563bc59
placemats:       1556910103-1c02745aae4d
print:           1513519245088-0e12902e5a38
light:           1513506003901-1e6a229e2d15
accessory:       1565193566173-7a0ee3dbe261
```

---

## Pending work

### index.html — implemented
- Price range on landing hero ("Starter kits from $79")
- Q4: third option "Both, depending on the room" added as full-width text card below photo pair
- Style Result: "Share my style" clipboard button with "Copied!" feedback
- Pack tournament: "Browse all packs instead →" escape hatch on round 1, routes to BrowseAllPacks screen (screen 17)
- Pack tournament: label language — "Challenger" → "Also great for you", "Your pick" → "Your current favorite", "here's your next challenge" → "here's your next option"
- "How it works" modal: accessible from every screen via persistent NavBar link; covers quiz logic, pack concept, tournament mechanic, AR upload, and returns
- Landing "How it works" nav link now opens the modal instead of a placeholder page

### index.html — pending (AR / Try in My Room section)
- Skip option / framing for messy/empty apartment context
- Photo guidance before upload (angle, lighting, framing — with ideal vs. poor examples)
- Improve AR composite fidelity
- Designer's placement note for each item's spatial position
- Error state for failed/poor-quality AR composite with retake guidance
- Fallback: curated similar-room stock photo if upload doesn't work
- Shareable AR composite/room composition

### Canvas cleanup (not index.html)
- Strip Direction B content from `Day 5/House2home Hi-Fi.html` — "Concierge / Room-as-Canvas" section still embedded. Direction B backed up in `Day 5/House2home Hi-Fi B.html`.
