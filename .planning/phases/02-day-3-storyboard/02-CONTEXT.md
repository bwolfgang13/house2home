# Phase 2: Day 3 — Storyboard - Context

**Gathered:** 2026-04-16
**Status:** Ready for planning

<domain>
## Phase Boundary

Produce a complete storyboard covering every screen required for the Day 4 Figma prototype, lock scope to Solo Mover desktop as the prototype spine, add Couple branch variant panels and AR branch representation, and confirm 5 Day 5 participants.

This phase ends with:
1. An 11-panel Solo Mover storyboard (physical artifact photographed, notes documented)
2. 4 Couple branch variant panels appended to the storyboard
3. 1 AR branch point labeled + 1 landing state panel added at Screen 7
4. 5 participants confirmed by name with session times
5. Day 3 sprint doc updated with reflection and all artifact references

The phase delivers a STORYBOARD — a complete, buildable map from which the Day 4 Figma prototype can be constructed directly. Not the prototype itself.

</domain>

<decisions>
## Implementation Decisions

### Storyboard Scope

- **D-01:** Solo Mover desktop = prototype spine. The primary storyboard has 11 panels covering the full Solo Mover path from style discovery to order confirmation. Panel cap: 12 maximum for the Solo track.
- **D-02:** Couple branch and AR branch are additions to the Solo storyboard — not separate storyboards. Total panels: 11 Solo + 4 Couple + 1 AR = 16, within acceptable range.
- **D-03:** The existing Day 3 physical artifact (photographed in Design Sprint-notes day 3 new.pdf) covers the 11 Solo Mover screens and is the ground truth. The Couple and AR panels are additional panels to be added.

### Couple Branch Panels (STRY-04)

- **D-04:** The Couple branch diverges at **Screen 1 (Style Finder Entry)**. The user selects "Shopping together" at the landing screen — the branch is explicit from the start, keeping the variant self-contained.
- **D-05:** 4 Couple branch panels in sequence:
  - **Panel C-1: Couple Entry** — "Shopping together" option selected on the landing screen; invite mechanism shown (send a link or share a code to partner)
  - **Panel C-2: Side-by-Side Style Profiles** — both partners have completed their individual style finders; profiles shown side by side
  - **Panel C-3: Overlap Highlight** — shared preferences highlighted between the two profiles; shows what they agree on
  - **Panel C-4: Blended Style Confirmation** — merged style result displayed; single CTA advances both users into A/B comparison
- **D-06:** After Panel C-4, the Couple flow reconnects to **Screen 4 (A/B Kit Comparison Round 1)** — same A/B mechanic, shared session.

### AR Branch Representation (STRY-05)

- **D-07:** AR branch point appears at **Screen 7 (Chosen Kit Detail)**. A "Test in Your Space" CTA sits alongside "Add to Cart" on the kit detail screen — the natural purchase-intent moment.
- **D-08:** One AR landing state panel: static mockup of a phone/tablet screen showing a real room with kit items AR-placed. Label: "Test in Your Space — AR concept." This is a branch point only — not interactive, not a full flow. After this panel, the user returns to Screen 7 to proceed to checkout.

### Storyboard Panel Structure (STRY-03)

- **D-09:** Each storyboard panel represents a decision moment or emotional beat — not a UI screenshot. Every panel carries a label (screen name/moment) and an annotation explaining the UX purpose or emotional state.
- **D-10:** The highest-risk moment panel must be present. Per Day 3 analysis: Screen 4 (A/B Round 1) is the highest-risk abandonment point — binary forced choice with no escape. This panel's annotation explicitly names the abandonment risk and the mechanic designed to prevent it.

### Participant Confirmation (STRY-07)

- **D-11:** 5 of the 11 identified participants (Anna, Orion, Isa, Eli, Nathaniel, Ray, Sadie, Mary, Craig, Seth, Birdie) must be confirmed with session times before Day 3 ends.
- **D-12:** Participant split: 3 in Solo Mover context (recently moved or about to move; no professional design background), 2 in Couple context (shopping with a partner or roommate).
- **D-13:** Screening criteria from the roadmap apply: exclude participants with professional interior design backgrounds.

### Sprint Doc (STRY-08)

- **D-14:** The Day 3 sprint doc (Day 3/Design Sprint Notes Day 3.md) must be updated to include: (a) photo/reference to the storyboard physical artifact, (b) reflection on the solution selection process (why Iteration 3 logic on Iteration 2's frame), (c) note on Couple and AR panels added.
- **D-15:** SKTCH-06 and SKTCH-07 (Phase 1 pending items) — solution sketch and Day 2 documentation — should be backfilled in the Day 2 notes before Phase 5 case study writing. This is a noted carry-forward, not a Phase 2 blocker.

### Claude's Discretion

- Order of work within the day: Solo storyboard confirmation first, Couple panels second, AR panel third, participant outreach last
- Exact annotation wording per storyboard panel
- Format of the participant confirmation record in the sprint doc

</decisions>

<canonical_refs>
## Canonical References

**Downstream agents MUST read these before planning or implementing.**

### Project Foundation
- `.planning/PROJECT.md` — Core value, constraints, platform architecture, key decisions
- `.planning/REQUIREMENTS.md` — Phase 2 requirements: STRY-01 through STRY-08 with acceptance criteria

### Existing Sprint Work
- `Day 1/Design Sprint Notes Day 1 - Expanded.md` — Day 1 problem statements, user flow maps for all 4 scenarios, 11 identified participants
- `Day 3/Design Sprint Notes Day 3.md` — Existing Day 3 notes covering Solo Mover 11-screen storyboard, solution sketch selection rationale, Pro flow documentation
- `Day 3/Design Sprint-notes day 3 new.pdf` — Physical storyboard artifact (photographed paper sketches) — ground truth for Solo Mover panel content

### Assignment Materials
- `Assingment details.rtfd/` — Springboard assignment requirements
- `Day 3/1686949456_IXC_32.5.2_Design_Sprint__Day_3.pdf` — Day 3 course materials (methodology reference for storyboarding)

### Prior Phase Context
- `.planning/phases/01-day-2-sketch/01-CONTEXT.md` — Phase 1 decisions including A/B mechanic design, solution sketch rationale, sprint doc structure

</canonical_refs>

<code_context>
## Existing Work Insights

### Reusable Assets
- Day 3 Solo Mover storyboard (11 panels): fully documented in Day 3 notes — no need to re-derive; Couple and AR panels are additions only
- 11 potential participants named in Day 1 notes: Anna, Orion, Isa, Eli, Nathaniel, Ray, Sadie, Mary, Craig, Seth, Birdie — use as the confirmed pool
- A/B kit comparison mechanic (binary forced-choice, 3 rounds, cost/item count/thumbnails): locked from Phase 1; Couple flow uses the same mechanic in a shared session

### Established Patterns
- Sprint doc structure: markdown file per day, physical artifacts photographed and referenced
- Storyboard format: paper sketch, photographed; panels labeled with screen name and annotation
- Scope boundary: Solo Mover desktop = buildable prototype; Couple/AR = storyboard representation only; Pro = case study annotation only

### Integration Points
- Storyboard → Day 4 Figma prototype: every panel in the storyboard maps to a frame in the prototype; the storyboard is the build spec
- Couple C-4 (Blended Result) → Screen 4 (A/B Round 1): this is the reconnection point; the prototype must support this entry path
- AR panel → Screen 7 (Kit Detail): AR branch point and CTA must appear on the Kit Detail frame in the prototype

</code_context>

<specifics>
## Specific Ideas

- The Couple branch uses the same individual style finder (Screens 1–3) for each partner independently; the merge happens at Panel C-2/C-3, not during style finding
- "Test in Your Space" AR CTA on Screen 7 should visually sit secondary to "Add to Cart" — it's an enhancement option, not the primary action
- The overlap highlight panel (C-3) should show the shared preferences as a visual callout — not a score or percentage, but the actual style words/emojis they both selected
- Storyboard panel count: 11 Solo + 4 Couple + 1 AR branch point annotation + 1 AR landing state = the physical artifact may need supplementary panels added (or annotated on the existing sketch)

</specifics>

<deferred>
## Deferred Ideas

- Participant outreach logistics (how to contact the 11 identified participants) — operational detail, not a design decision
- SKTCH-06/07 backfill into Day 2 notes — noted as a pre-Phase 5 task, not a Phase 2 blocker
- Couple flow A/B comparison redesign (shared voting mechanic within the A/B rounds) — would be a new capability; the current decision is that the Couple flow uses the same A/B mechanic in a shared session with the blended style as context

</deferred>

---

*Phase: 02-day-3-storyboard*
*Context gathered: 2026-04-16*
