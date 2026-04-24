# Design Sprint -- Day 3 Notes
## House2Home | Storyboard & Solution Sketch

## Context

Day 2 produced the lightning demo research (10 competitors), committed A/B Kit Comparison as the primary critical screen, and completed two rounds of Crazy 8s. Day 3 takes the selected interaction model — binary forced-choice kit comparison — and builds it out into a storyboard: a full sequence of screens covering the user arc from landing to order confirmation. The goal is light wireframes sufficient to prototype from, not finished designs.

## Key Decision: Prototype Scope Lock

**Decision:** Solo Mover desktop flow (Screens 1–10) is the prototype spine for Day 4.

**Rationale:** A solo sprint cannot validate three separate flows in a single session. Solo Mover is the critical path because it tests the core A/B kit comparison mechanic that all personas share. Validating this mechanic first is the highest-leverage test available.

**What's deferred:** Couple branch (STRY-04) and AR branch (STRY-05) are deferred — designed but not built in this sprint. The case study will reference them as validated through the design process (storyboarded, not prototyped).

**What's out of scope:** Professional/Architect flow is not storyboarded or prototyped — documented in sprint notes only as a reference for the case study.

## Solution Sketch Selection

From the Crazy 8s Round 1, the selected interaction model was **"1 or 2 — Pick Your Starter Pack"**: a binary forced-choice screen showing two style-matched kits with no third option, no back-out, no open browsing. Three rounds of this comparison narrow 6 kits to 1.

Three screen variations were iterated before settling on the final solution:
- **Iteration 1:** Style confirmed → full kit preview below label — too much information at once
- **Iteration 2:** "1 or 2" binary side-by-side — clean forced choice, right level of information
- **Iteration 3:** Cost/item count breakdown with thumbnails — surfaced the right detail (price, item count) without requiring a full kit read

**Settled on Iteration 3 logic applied to Iteration 2's comparison frame:** Show "1 or 2" as the primary action, with cost (~$860), item count (5 items), and small thumbnails as the only context provided. No descriptions, no style labels in the comparison — the visual kit does the explaining.

**Selection rationale:** Simplifies information, prioritizes the single action the user needs to take (pick one), and creates a predictable repeating flow across all 3 rounds.

## Storyboard — Solo Mover Flow (Desktop)

*Physical artifact: paper sketch, photographed in Design Sprint-notes day 3 new.pdf*

### Screen 1: Style Finder Entry
House2Home landing. User sees style discovery prompt — "Find Your Style and decorate your home." Single primary CTA. Kit previews shown below to anchor expectation.

### Screen 2: Style Selector
Multi-select word/emoji grid — "words that describe your style, select 5–8." Low cognitive load, implicit style signaling. Selection seeds the style profile without asking users to self-report a style name.

### Screen 3: Style Confirmed
"Your Style: Modern" — style label displayed with 2–3 kit thumbnails as proof. User sees what their style produces before entering comparison. CTA advances to kit comparison rounds.

### Screen 4: A/B Kit Comparison (Round 1 of 3)
**Primary critical screen.** "1 or 2 — Pick Your Starter Pack." Two kits shown side by side. Each kit shows: cost (~$860), item count (5), small item thumbnails. No descriptions. User picks one; the other is eliminated. Progress indicator shows round position (Round 1 of 3).

### Screen 5: A/B Kit Comparison (Round 2 of 3)
Same pattern. Winning kit from Round 1 faces a new kit. Same information structure. Rounds feel identical by design — predictable, low friction.

### Screen 6: A/B Kit Comparison (Round 3 of 3)
Final round. One winner emerges.

### Screen 7: Chosen Kit Detail
"Modern... Pack" — full kit display. Item list with individual thumbnails, total cost (~$853), add-ons section. Two CTAs: "Add to Cart" (primary) and "Add Items" (secondary — for individual swaps). Customization is available but not required.

### Screen 8: Add-Ons
Optional upsell screen. Additional items shown with thumbnails, names, prices, checkboxes. User can add or skip.

### Screen 9: Order Summary
Order detail screen. Shows: delivery estimate, payment info entry, shipping info entry. CTA: proceed to payment.

### Screen 10: Order Confirmation
Confirmation screen. Order summary (items, total), delivery date, visual of chosen kit items. Secondary CTA: share / save.

### Screen 11: Email Confirmation
Email view — "Summary: Starter Pack" — order recap with item list. Entry point back into app if user wants to track or reorder.

## Storyboard Panel Summary

| Panel | Screen Name | Decision Moment / Emotional Beat | Annotation | Prototype-Required |
|-------|-------------|----------------------------------|------------|-------------------|
| 1 | Style Finder Entry | Entry commitment — user decides to engage | Single CTA anchors expectation; kit previews below reduce uncertainty | Yes |
| 2 | Style Selector | Self-expression — user externalizes taste | Word/emoji multi-select seeds style profile without requiring design vocabulary | Yes |
| 3 | Style Confirmed | Validation — user sees their style named | Style label + kit thumbnails prove the system understood them; builds trust before comparison | Yes |
| 4 | A/B Kit Comparison R1 | **HIGHEST-RISK MOMENT** — forced binary choice with no escape | Abandonment risk: user forced to pick 1-of-2 with no back-out, no browse, no third option. Mitigation: cost/item count/thumbnails provide just enough info for a gut decision without analysis paralysis | Yes |
| 5 | A/B Kit Comparison R2 | Momentum — repeat pattern reduces friction | Same structure as R1; predictability lowers cognitive load by round 2 | Yes |
| 6 | A/B Kit Comparison R3 | Resolution — one winner emerges | Final elimination round; user sees the pattern complete | Yes |
| 7 | Chosen Kit Detail | Ownership — user examines what they chose | Full kit display with item list, total cost; customization available but not required | Yes |
| 8 | Add-Ons | Optional expansion — user can enhance without pressure | Upsell positioned as optional; checkboxes keep it low-commitment | Yes |
| 9 | Order Summary | Commitment — financial decision point | Standard checkout flow; delivery estimate and payment entry | Yes |
| 10 | Order Confirmation | Completion — purchase confidence achieved | Order recap with delivery date; share/save CTA extends the moment | Yes |
| 11 | Email Confirmation | Post-purchase reassurance | Order recap via email; re-entry point to app | No (low priority) |

Screens 1–10 map 1:1 to Figma prototype frames for Day 4. Screen 11 (Email Confirmation) is documented but not required for the tested prototype.

## Storyboard — Professional Flow (Desktop)

*Physical artifact: paper sketch, page 3 of Design Sprint-notes day 3 new.pdf*

### Screen 1: Pro Dashboard
Logged-in state. Shows active projects as a grid (3–4 project cards with client name, project status, budget). Status indicators per project. New Project CTA prominent.

### Screen 2: New Project Form
Modal or dedicated screen. Fields: Client name, Budget, Level (brief/detail), Budget confirmation. Primary CTA: "New Style Brief."

### Screen 3: Dashboard Updated
Returns to dashboard. New project card appears. Project shows status: style finder not yet sent.

### Screen 4: Smith Project — Style & Kits
Project detail view. Client: Smith. Style: Modern → "Find Kits" CTA triggers kit curation for this style. Pro sees the same kit pool the client will compare from.

### Screen 5: Kit Selection by Pro
Pro-curated kit selection screen. Multiple kit thumbnails displayed in a row with checkmark/checkboxes. Pro selects the 2–3 kits to send to client for comparison. Checkmark confirms selection.

### Screen 6: Smith Project — Ready to Send
Project detail updated. Shows: Style: Modern, selected kits displayed as thumbnails. Primary CTA: "Send to Client." Pro can review selection before sending.

## Next Step

Prototype the Solo Mover flow first. Screens 1–10 above define the prototype scope for Phase 1 of prototyping.

**Prototype scope (Solo Mover, Phase 1):**
- Style Finder → Style Selector → Style Confirmed → A/B Kit Comparison × 3 → Chosen Kit Detail → Add-Ons → Order Summary → Order Confirmation

**Deferred to later phases:**
- Couple/Roommates flow (shared style finder + anonymous vote reveal)
- Professional flow (dashboard, project management, client kit sending)
- Mobile AR flow ("Test in Your Space" entry point + AR kit visualization)
