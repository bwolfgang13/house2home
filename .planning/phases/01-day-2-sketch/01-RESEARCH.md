# Phase 1: Day 2 — Sketch - Research

**Researched:** 2026-04-01
**Domain:** GV Design Sprint methodology — Lightning Demos, Crazy 8s, Solution Sketch
**Confidence:** HIGH

---

<user_constraints>
## User Constraints (from CONTEXT.md)

### Locked Decisions

- **D-01:** A/B kit comparison is the PRIMARY critical screen — first Crazy 8s round targets this screen
- **D-02:** The Crazy 8s question to answer for A/B comparison: "How do we reduce choice paralysis?" — explore the decision mechanic itself, not just the visual layout
- **D-03:** Style selector is the SECONDARY critical screen — second Crazy 8s round
- **D-04:** HMW notes from Day 1 are the prompts for Crazy 8s — do not start from blank paper; use them to ensure panels are distinct interaction models, not layout variations
- **D-05:** 10 products total across 4 categories
- **D-06:** Consumer tools (Houzz, Homestyler, Planner 5D, Pinterest) — 3-field notes: what it does well, what's missing, what mechanism to borrow
- **D-07:** Collaborative tool (Miro/FigJam) — mechanism focus: how individual contributions merge into a shared output — directly analogous to the Couple flow's style profile merge
- **D-08:** Pro tools (Houzz Pro, Modsy, Havenly) — use the specific question sets from the research guide
- **D-09:** AR tools (IKEA Place, Wayfair AR) — use the specific question sets from the research guide
- **D-10:** The 3-panel solution sketch captures the A/B kit comparison moment — Before (style profile, 6 options, no direction) / During (comparison mechanic that reduces paralysis) / After (emotional confidence, "I chose this")
- **D-11:** Annotations explain design decisions, not just label UI — reader must understand the UX bet without verbal explanation
- **D-12:** Crazy 8s done on physical paper — photographed and embedded
- **D-13:** Sprint doc is a Markdown file (Day 2/ directory), consistent with Day 1 structure
- **D-14:** Doc must include: screenshots/photos of Crazy 8s, lightning demo notes per product, solution sketch photo, written reflection on key choices made

### Claude's Discretion

- Per-category mechanism lens for consumer tools: identify what each product does to reduce style/decision uncertainty and where the flow breaks down
- Order of lightning demos within a session: consumer tools first (context), then collaborative (mechanism analogy), then pro tools (client flow), then AR (placement UX)
- Specific format/structure of the Day 2 markdown doc sections

### Deferred Ideas (OUT OF SCOPE)

None — discussion stayed within phase scope.

</user_constraints>

---

<phase_requirements>
## Phase Requirements

| ID | Description | Research Support |
|----|-------------|------------------|
| SKTCH-01 | Lightning demos completed for 4+ competitor/analogous products (must include at least one collaborative tool) | Lightning demo structure section; 10-product set defined with 4 categories |
| SKTCH-02 | Lightning demo notes document each product's mechanism (what they do, what's missing, what's worth borrowing) | 3-field note format per product; category-specific lens questions documented |
| SKTCH-03 | Most critical screen identified and documented with rationale | Locked as A/B kit comparison (D-01); rationale documented in CONTEXT.md |
| SKTCH-04 | Crazy 8s completed for critical screen — 8 distinct interaction models, not layout variations | Crazy 8s methodology section; HMW prompts as scaffolding; 8 distinct interaction model archetypes for A/B mechanic |
| SKTCH-05 | Second Crazy 8s round for at least one additional critical screen | Second round targets style selector (D-03); methodology same as first round |
| SKTCH-06 | Solution sketch — 3-panel before/during/after with annotation explaining design decisions | Solution sketch format section; annotation rules; UX bet framing |
| SKTCH-07 | Day 2 work documented in sprint doc (screenshots, written reflection) | Sprint doc structure section; Day 1 template as model |

</phase_requirements>

---

## Summary

Day 2 of the GV design sprint has three sequential activities: Lightning Demos (inspiration capture), Crazy 8s (rapid divergent ideation), and Solution Sketch (convergent commitment). Each feeds the next. Lightning demos generate mechanisms worth borrowing. Crazy 8s use those mechanisms as raw material to produce 8 distinct interaction models per critical screen. The solution sketch commits to one 3-panel story built from the best Crazy 8s idea.

The central design challenge for this phase is answering a specific question: **How do we reduce choice paralysis during A/B kit comparison?** The Crazy 8s must explore the mechanics of that decision moment — not the visual styling of it. This distinction is the highest-risk gap in the phase (panels becoming layout variations rather than interaction model variations). Using Day 1 HMW notes as scaffolding, not blank paper, is the primary mitigation.

The solution sketch must land on an emotional outcome, not a UI state. "The user feels confident they chose this" is different from "the user is presented with a selection." The annotation layer is where that bet gets made explicit — panels alone are insufficient.

**Primary recommendation:** Run lightning demos in the prescribed order (consumer → collaborative → pro → AR), capture per-product mechanism notes using the 3-field format, then use HMW notes explicitly as Crazy 8s prompts to generate interaction model variety before selecting the best idea for the solution sketch.

---

## Standard Stack

This is a design/UX sprint with no code. "Stack" in this context means the tools and physical materials required.

### Core Materials

| Tool/Material | Purpose | Why Standard |
|---------------|---------|--------------|
| Physical paper (A4 or larger) | Crazy 8s substrate — folded into 8 panels | GV canonical method; physical keeps sketching fast and uncommitted |
| Black pen (medium tip) | Sketching | Forces commitment, no erasing, keeps pace |
| Camera/phone | Photograph paper artifacts | Embeds sketches into digital sprint doc |
| Markdown file (Day 2/ directory) | Sprint doc — mirrors Day 1 structure | Consistency with Day 1 format per D-13 |

### Reference Inputs (must be loaded before starting)

| Asset | Location | Used For |
|-------|----------|---------|
| Day 1 HMW notes | `Day 1/Design Sprint Notes Day 1 - Expanded.md` | Crazy 8s prompts — prevents blank-paper echo chamber |
| Solo Mover user flow map | Same file | "Before" state for solution sketch panel 1 |
| Prior competitor notes | Same file | Starting point for consumer tool lightning demo notes — do not re-research from scratch |
| A/B comparison × 3 mechanism description | `Day 1/Design Sprint Notes Day 1 - Expanded.md` (Key Design Decisions table) | The mechanism the solution sketch must depict |

---

## Architecture Patterns

### Lightning Demo Structure

**The GV canonical format per demo:**

1. Present product (screenshot or live demo)
2. Capture one headline: what is the interesting element
3. Capture one borrowable mechanism: what specifically could be stolen/adapted
4. Duration: 3 minutes per product maximum

**The 3-field note format for this sprint (D-06):**

```
Product: [Name]
Category: [Consumer / Collaborative / Pro / AR]
What it does well: [one mechanism or pattern that works]
What's missing: [where the flow breaks down or the gap exists]
Mechanism to borrow: [the specific thing worth adapting for House2Home]
```

**Lightning demo order (Claude's discretion):**

1. Consumer tools first — establish baseline (Houzz, Homestyler, Planner 5D, Pinterest)
2. Collaborative tool second — mechanism analogy for Couple flow (Miro or FigJam)
3. Pro tools third — client curation and approval flow (Houzz Pro, Modsy, Havenly)
4. AR tools last — placement and confirmation UX (IKEA Place, Wayfair AR)

**Rationale for this order:** Consumer tools contextualize what exists. The collaborative tool reveals a mechanism analogy directly relevant to the Couple flow's merge moment. Pro tools show client-facing curation. AR tools inform visualization UX — least relevant to the primary critical screen.

### Lightning Demo Research Guide (per-category lens)

**Consumer Tools (Houzz, Homestyler, Planner 5D, Pinterest):**
- What does this product do to reduce style/decision uncertainty?
- Where does the flow break down — where does the user get lost or drop off?
- Is there a comparison mechanism? How does it work?
- Prior notes exist in Day 1 — build on them, do not re-research from scratch

**Collaborative Tool (Miro or FigJam — pick one):**
- How do individual contributions merge into a shared output?
- Is there a voting or preference-capture mechanism?
- What does it feel like when individual choices converge to a team decision?
- How is the "winner" surfaced — is it calculated, voted, or negotiated?
- **Why this matters:** Directly analogous to Couple flow's style profile merge. The mechanism Miro/FigJam uses to make individuals feel heard while producing a shared outcome is the pattern to borrow.

**Professional Tools (Houzz Pro, Modsy, Havenly):**
- Houzz Pro: How does client sharing/approval work? Can pros curate selections for clients? What does the project dashboard look like?
- Modsy: How are room visualizations presented to clients? What's the purchase flow — does the pro buy or the client?
- Havenly: How does the designer present selections? How does client review and approval work? What's the communication model?
- **Pattern to watch:** Thumbs up/down product rating (Havenly) is a discrete preference signal — relevant to style selector mechanic

**AR Tools (IKEA Place, Wayfair AR):**
- How does AR onboarding work — what does scanning feel like?
- How do you place, move, and swap items?
- What's the path from AR placement to purchase?
- Can you view multiple items together or just one at a time? (Wayfair: yes, multiple items now supported)
- How accurate is style filtering before AR placement?
- **IKEA Kreativ note (2024):** IKEA moved from simple AR placement to Scene Scanner — creates editable 3D room replica. More complex onboarding but higher spatial accuracy.

### Crazy 8s Structure

**The exercise:**
- Fold one sheet of A4 paper into 8 equal panels
- Set an 8-minute timer
- Sketch one idea per panel — one minute maximum each
- Goal: 8 distinct ideas, not 8 versions of one idea

**The critical distinction for this sprint:**

Distinct interaction models means:
- Panel 1: Head-to-head bracket (show Kit A vs Kit B — pick one, move on)
- Panel 2: Trait comparison (show kits by attribute — "cozy" "modern" "bold")
- Panel 3: Guided question (ask user a question about their life, filter kit to 2 based on answer)
- Panel 4: Elimination with reasons (user marks "not this" with a tag, system learns and narrows)
- Panel 5: Scroll-to-commit (kit options scroll horizontally; commit by reaching end)
- Panel 6: Undo-friendly choice (pick one, but system immediately asks "sure?" with both still visible)
- Panel 7: "What matters most" slider (rate warmth/boldness/budget weighting, kit sorts)
- Panel 8: Expert pick prompt ("if a stylist chose for you, they'd pick X — agree or override?")

Layout variations means:
- Panel 1: Kit A left, Kit B right — white background
- Panel 2: Kit A left, Kit B right — colored background
- Panel 3: Kits stacked vertically — same mechanic
(This is the failure mode to avoid.)

**Using HMW notes as prompts (D-04):**
Before starting the timer, write one HMW note from Day 1 at the top of each panel. This pre-frames each panel with a distinct question, preventing the mind from defaulting to layout variations.

**Two Crazy 8s rounds:**
- Round 1 (primary): A/B kit comparison — "How do we reduce choice paralysis?"
- Round 2 (secondary): Style selector — "How might we help users discover their style without making them feel tested?"

**Between rounds:** Brief review of Round 1 panels. Circle the interaction model(s) with highest potential. Do not skip Round 2 — SKTCH-05 requires it and the secondary screen feeds Day 3 storyboarding.

### Solution Sketch Structure

**The 3-panel format:**

| Panel | Name | What It Contains |
|-------|------|-----------------|
| 1 — Before | Setup | User's state entering the decision moment: style profile exists, 6 kit options shown, no clear direction — the paralysis condition |
| 2 — During | The Bet | The specific interaction model that plays out — the mechanic that reduces paralysis. This is the primary design decision. It should show the HOW, not just the WHAT. |
| 3 — After | Emotional Resolution | User's state after completing the mechanic — emotional outcome ("I chose this"), not a UI state ("selection confirmed"). Confidence, not completion. |

**Annotation rules (SKTCH-06, D-11):**

Each panel needs:
1. A title label
2. A written description of what is happening
3. At least one annotation explaining WHY — the design decision behind the depicted mechanic

A reader must be able to understand the UX bet without verbal explanation from the creator. This is the test: if you removed yourself and showed the sketch to someone, would they understand what design choice is being made and why?

**The key UX bet to communicate in Panel 2:**
The comparison mechanic must make the user feel they CHOSE their kit, not that they were guided to one. "I chose this" vs. "I was shown this" is the emotional delta. The annotation must name this explicitly.

**Common annotation failure:** Labeling UI elements instead of explaining decisions.
- Bad: "This is the comparison panel. Kit A is shown on the left."
- Good: "Showing only 2 kits at once reduces cognitive load — user is never evaluating more than one pair. The 3-round structure gives a sense of progress and agency."

### Sprint Doc Structure

Consistent with Day 1 format (D-13). Recommended Day 2 sections:

```markdown
# Design Sprint — Day 2 Notes
## House2Home | Sketch Day

## Context
[Brief recap of Day 1 outcome and what Day 2 addresses]

## Lightning Demos
### [Product Name] — [Category]
**What it does well:** ...
**What's missing:** ...
**Mechanism to borrow:** ...
[Screenshot or description]

[Repeat for all 10 products]

### Lightning Demo Summary
[Cross-category patterns; 2-3 mechanisms that emerged as most relevant]

## Critical Screen Decision
**Primary:** A/B Kit Comparison
**Rationale:** [The choice paralysis problem is the highest-stakes UX bet in the product]
**Secondary:** Style Selector

## Crazy 8s — Round 1: A/B Kit Comparison
**Question:** How do we reduce choice paralysis?
**HMW prompts used:** [list the 8 HMW notes used as panel headers]

[Embedded photo of Crazy 8s paper]

**Reflection:** [Which panels were distinct interaction models? Which panel or panels stood out and why?]

## Crazy 8s — Round 2: Style Selector
**Question:** How might we help users discover their style without making them feel tested?

[Embedded photo of Crazy 8s paper]

**Reflection:** [Same format]

## Solution Sketch — A/B Kit Comparison
[Embedded photo of 3-panel sketch]

**Panel 1 — Before:** [Description]
**Panel 2 — During:** [Description + design decision annotation]
**Panel 3 — After:** [Description + emotional outcome annotation]

**Key Design Decisions:**
[Written reflection on what the sketch commits to and why]

## Key Choices & Reflections
[What was hard, what surprised you, what you would do differently]
```

---

## Don't Hand-Roll

| Problem | Don't Build | Use Instead | Why |
|---------|-------------|-------------|-----|
| Crazy 8s prompts | Blank paper and improvised framing | Day 1 HMW notes written at top of each panel | Blank paper leads to echo-chamber iterations; HMW notes force distinct framing per panel |
| Solution sketch annotation | Verbal explanation after the fact | Written annotations on the sketch itself before photographing | GV method requires self-explanatory sketches — verbal explanation is a failure mode |
| Lightning demo notes | General impressions ("this app is cool") | 3-field structured notes (well / missing / borrow) | General impressions don't generate actionable Crazy 8s prompts |
| Critical screen rationale | Unstated assumption | Written sentence naming the screen and the reason before Crazy 8s begins | SKTCH-03 acceptance criterion; also creates accountability for the design bet |

**Key insight:** The sprint doc is not a record of what you did — it is the artifact that proves you did the right things. Each entry should be scannable by a reviewer and immediately clear about what was decided and why.

---

## Runtime State Inventory

Step 2.5 SKIPPED — this is a design artifact phase, not a rename/refactor/migration phase. No runtime state inventory required.

---

## Environment Availability

| Dependency | Required By | Available | Notes |
|------------|-------------|-----------|-------|
| Physical paper | Crazy 8s (D-12) | User-supplied | A4 or larger; fold into 8 panels |
| Black medium-tip pen | Crazy 8s (D-12) | User-supplied | Unscented recommended to avoid distraction during timed sessions |
| Phone/camera | Photo capture (D-12, D-14) | Standard | Photos embedded in Markdown sprint doc |
| Markdown editor | Sprint doc (D-13) | Available | Day 1 doc already exists in same format |
| Day 1 notes file | HMW prompts (D-04) | Available | `Day 1/Design Sprint Notes Day 1 - Expanded.md` confirmed present |
| Internet access | Lightning demos — live product screenshots | Required during demos | Products (Houzz, IKEA Place, etc.) accessed via browser |

**Missing dependencies with no fallback:** None.

**Missing dependencies with fallback:** None.

---

## Common Pitfalls

### Pitfall 1: Crazy 8s Panel Echo Chamber (Layout Variations)
**What goes wrong:** All 8 panels depict the same two-column kit comparison layout with minor visual tweaks — different background colors, text sizes, or button placements. The interaction model is identical across all 8 panels.
**Why it happens:** Starting from blank paper with no distinct prompt per panel defaults to the first idea that formed. Visual designers naturally iterate on layout before considering interaction model.
**How to avoid:** Write one HMW note at the top of each panel before setting the timer. The HMW note forces a distinct framing for each panel. If Panel 3 says "HMW make users feel like experts?" the sketch must answer that question, not redraw the same layout.
**Warning signs:** After 8 minutes, all panels show the same spatial arrangement of two kits side-by-side. Stop and re-run with explicit HMW prompts.

### Pitfall 2: Skipping the Second Crazy 8s Round
**What goes wrong:** Round 1 runs long or feels productive, and Round 2 gets abbreviated or skipped "to save time."
**Why it happens:** First round is energizing; second round feels less urgent. Solo sprints have no team accountability to complete the round.
**How to avoid:** Treat SKTCH-05 as a hard gate. Round 2 (style selector) feeds the secondary critical screen that becomes a Day 3 storyboard decision point. Skipping it leaves the style selector mechanic undecided going into Day 3.
**Warning signs:** Round 2 panels reuse ideas from Round 1 without reframing — means Round 2 wasn't prompted with distinct HMW notes.

### Pitfall 3: Solution Sketch Annotation Labels UI Instead of Explaining Decisions
**What goes wrong:** Annotations say "this is the comparison panel" or "user selects Kit A" — they describe what is visible, not why the design choice was made.
**Why it happens:** Annotation feels like extra work after sketching. Default mode is labeling.
**How to avoid:** Before sketching the solution, write out the UX bet in one sentence. Every annotation should connect to that bet. The annotation for Panel 2 must name the interaction model AND explain why it was chosen over alternatives.
**Warning signs:** A reader who has never seen the product would not understand what design decision is being made from the sketch and its annotations alone.

### Pitfall 4: Lightning Demos Produce Inspiration Without Borrowable Mechanism
**What goes wrong:** Notes say "Havenly is beautiful" or "IKEA Place feels futuristic" — impressionistic responses with no specific mechanism named.
**Why it happens:** 3-minute demos move fast; note-taking defaults to emotional response.
**How to avoid:** Force the third field — "mechanism to borrow" — to be a concrete behavioral description. Not "the comparison feels smooth" but "Havenly's thumbs up/down product rating gives the system a preference signal without requiring the user to articulate a style vocabulary."
**Warning signs:** Lightning demo notes contain adjectives (beautiful, intuitive, smooth) without describing what the product actually does that produces those feelings.

### Pitfall 5: Solution Sketch Panel 3 Depicts a UI State, Not an Emotional Outcome
**What goes wrong:** Panel 3 shows "Order Confirmed" or "Kit selected" — a transactional endpoint.
**Why it happens:** "After" state is naturally interpreted as "task completed."
**How to avoid:** Panel 3 must answer: how does the user feel at this moment, and what in the design made them feel that way? "I chose this" vs "I was shown this" is the distinction. The annotation must name the emotional outcome explicitly.
**Warning signs:** Panel 3 shows a confirmation screen or success state with no indication of emotional confidence.

---

## Code Examples

This is a design sprint phase with no code. This section contains equivalent patterns: annotation examples and mechanism descriptions.

### Lightning Demo Note — Correct Format

```
Product: Havenly
Category: Professional Tool
What it does well: Designer presents a curated set of products; client rates each thumbs up/down. System gives designer a preference signal without requiring client to articulate a style vocabulary.
What's missing: No mechanism for the client to see WHY certain items were selected — curation logic is opaque to the client. Trust relies on the designer's reputation.
Mechanism to borrow: Discrete preference signal (thumbs up/down per item) that populates a preference profile without asking the user to self-describe. This is analogous to how our style selector could capture emotional response to items rather than abstract style labels.
```

### Crazy 8s HMW Panel Setup — Correct Format

Before starting the 8-minute timer, write one HMW note at the top of each panel:

```
Panel 1: HMW make each comparison feel like the final one?
Panel 2: HMW make the user feel like an expert during the comparison?
Panel 3: HMW let the kits explain themselves rather than requiring a read?
Panel 4: HMW make "not choosing" feel like progress, not failure?
Panel 5: HMW create a sense of momentum through the 3-round structure?
Panel 6: HMW show the user what they're moving toward, not just away from?
Panel 7: HMW make the chosen kit feel inevitable in retrospect?
Panel 8: HMW reduce the fear of choosing wrong?
```

### Solution Sketch Annotation — Correct Format

```
Panel 2 — During [Title: "The Head-to-Head Round"]
Sketch: Two kits shown side-by-side. Large images. One detail attribute visible per kit 
(single strongest differentiator, not a full item list). "Choose" button below each.
Progress indicator: Round 1 of 3.

Annotation: Showing only ONE differentiating attribute per kit reduces the evaluation 
surface — user makes a gut call, not a spreadsheet decision. The 3-round structure 
reframes elimination as progress. At no point does the user see 6 options — only 2.
This is the core bet: structured elimination > open browsing.
```

---

## State of the Art

| Consideration | Current Understanding | Impact |
|--------------|----------------------|--------|
| IKEA Place vs. IKEA Kreativ | IKEA evolved from simple AR overlay (Place) to full Scene Scanner room replica (Kreativ, 2024). The original "Place" UX is simpler and more relevant to analogous research for House2Home's AR scope. | Use IKEA Place as the lightning demo reference, not IKEA Kreativ — the simpler onboarding model is the one worth borrowing. |
| Wayfair AR multi-item | Wayfair now supports multiple items in one AR scene (via RealityKit + LiDAR). | Relevant to House2Home's AR "kit in your space" concept — single-item placement is no longer the ceiling. |
| Modsy status | Modsy shut down in 2022. | Cannot be researched as a live product. Use archived reviews, case studies, or competitor analyses for Modsy insights. Alternative: substitute Decorilla or Spacejoy as a live comparable pro-consumer hybrid. |
| Havenly client approval | Havenly uses a thumbs up/down product rating per item — generates preference signal without style vocabulary requirement. | High-borrowability mechanism for House2Home's style selector. |

**Deprecated/outdated:**
- Modsy: Shut down 2022 — cannot access live product. Use archived documentation or substitute with Decorilla/Spacejoy.

---

## Open Questions

1. **Modsy is shut down**
   - What we know: Modsy closed in 2022. The CONTEXT.md includes it as a lightning demo target.
   - What's unclear: Whether archived screenshots/reviews are sufficient for the lightning demo, or whether a live substitute (Decorilla, Spacejoy) should replace it.
   - Recommendation: Use one article from the archived Modsy coverage (the design sprint question set can still be answered via reviews) AND note the substitution in the sprint doc. This is a research limitation, not a blocking issue.

2. **Which specific HMW notes from Day 1 to use as Crazy 8s prompts**
   - What we know: Day 1 HMW notes exist in the Day 1 expanded notes file. The file does not have a dedicated HMW section — notes are embedded in the problem statements and design decisions.
   - What's unclear: Whether there is a discrete HMW list to pull from, or whether HMW notes need to be derived from the problem statements before Crazy 8s begins.
   - Recommendation: The plan should include a Wave 0 task to extract/derive 8 HMW notes from Day 1 content before Crazy 8s begins. The 8 sample prompts in the Code Examples section can serve as defaults if Day 1 HMW notes are insufficient.

3. **Miro vs. FigJam for the collaborative tool lightning demo**
   - What we know: D-07 specifies "Miro/FigJam" as the collaborative tool category — either is acceptable.
   - What's unclear: Which platform more clearly demonstrates the individual-to-shared-output merge mechanism relevant to the Couple flow.
   - Recommendation: Use Miro's dot voting + voting reveal flow as the primary demo. It most directly parallels the concept of individual preferences converging to a shared decision with a visible result.

---

## Validation Architecture

> `workflow.nyquist_validation` is `true` in `.planning/config.json`. However, this phase produces no code — all outputs are physical/digital design artifacts (paper sketches, markdown doc, photographs). Automated testing is not applicable. Manual verification is the validation mechanism.

### Test Framework

| Property | Value |
|----------|-------|
| Framework | Manual artifact review (no automated test framework) |
| Config file | None — design sprint phase |
| Quick check command | Human review of sprint doc sections against SKTCH acceptance criteria |
| Full suite command | Complete review of all 7 SKTCH requirements against acceptance criteria |

### Phase Requirements → Verification Map

| Req ID | Behavior | Test Type | Verification Method | Automatable? |
|--------|----------|-----------|---------------------|-------------|
| SKTCH-01 | Lightning demos for 4+ products including 1 collaborative tool | Manual | Count entries in sprint doc; verify at least 1 is Miro/FigJam category | No |
| SKTCH-02 | Notes document mechanism per product (what / missing / borrow) | Manual | Each product entry has all 3 fields with concrete (non-impressionistic) content | No |
| SKTCH-03 | Critical screen named and justified before Crazy 8s | Manual | Sprint doc has a "Critical Screen Decision" section with rationale before Crazy 8s section | No |
| SKTCH-04 | Crazy 8s — 8 distinct interaction models, not layout variations | Manual | Review Crazy 8s photo: do panels show distinct decision mechanics? | No |
| SKTCH-05 | Second Crazy 8s round for at least one additional screen | Manual | Sprint doc has a second Crazy 8s section with photo for style selector | No |
| SKTCH-06 | 3-panel solution sketch with annotation explaining decisions | Manual | Photo exists; each panel has a title + description; at least one annotation per panel explains WHY | No |
| SKTCH-07 | Day 2 work documented — screenshots, reflection | Manual | Sprint doc contains all required sections; Crazy 8s photos embedded; reflection section present | No |

### Wave 0 Gaps

- [ ] Derive/extract HMW notes from Day 1 content — 8 notes needed as Crazy 8s panel prompts before Round 1 begins
- [ ] Confirm Modsy substitution decision (archived research vs. live alternative) — needed before lightning demo session begins
- [ ] Physical materials check: A4 paper, black pen, phone for photography — physical prerequisites before any sketching task

*(No code test files needed — this phase produces zero code.)*

---

## Sources

### Primary (HIGH confidence)
- GV Design Sprint Kit — Crazy 8s methodology (designsprintkit.withgoogle.com)
- Thoughtbot Sprint Guide — 3-step storyboard rules and lightning demo format (design.thoughtbot.com)
- GV Library — Sprint Tuesday overview (library.gv.com/sprint-week-tuesday)
- Day 1 notes: `Day 1/Design Sprint Notes Day 1 - Expanded.md` — user flow maps, design decisions, platform architecture
- CONTEXT.md (`01-CONTEXT.md`) — all locked decisions and sprint specifics

### Secondary (MEDIUM confidence)
- Design Sprint X — Tuesday facilitator tips, Crazy 8s best practices (designsprintx.com)
- SessionLab / pdmethods.com — Lightning demo structure and note-taking format
- NN/G — Choice overload and cognitive load reduction patterns (nngroup.com)
- Havenly review sources — client review/approval flow description (stuccco.com, decorilla.com)
- IKEA AR coverage — Onboarding and placement UX (academia.edu study, xrtoday.com review)
- Wayfair AR — Multi-item support and RealityKit integration (aboutwayfair.com, engadget.com)

### Tertiary (LOW confidence — flagged for validation)
- Modsy mechanism notes — based on archived reviews only; service is defunct (2022). Verify via archived coverage before including in lightning demo notes.

---

## Metadata

**Confidence breakdown:**
- Lightning demo structure and format: HIGH — confirmed against multiple GV-sourced references
- Crazy 8s methodology and distinct-vs-variation distinction: HIGH — canonical GV method, multiple sources agree
- Solution sketch format and annotation rules: HIGH — Thoughtbot sprint guide + GV library
- Per-product mechanism details (Havenly, IKEA Place, Wayfair): MEDIUM — secondary sources, live products accessible for verification during execution
- Modsy: LOW — defunct service, archived sources only

**Research date:** 2026-04-01
**Valid until:** 2026-05-01 (stable design methodology; product UX details may drift for live apps)
