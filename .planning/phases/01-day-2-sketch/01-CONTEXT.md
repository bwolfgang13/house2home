# Phase 1: Day 2 — Sketch - Context

**Gathered:** 2026-04-01
**Status:** Ready for planning

<domain>
## Phase Boundary

Produce a committed solution direction for the House2Home design sprint. This phase ends with:
1. Lightning demos documented for 10 products across 4 categories
2. Two Crazy 8s rounds completed (A/B kit comparison primary, style selector secondary)
3. One 3-panel solution sketch committed — tells the A/B comparison before/during/after story
4. All Day 2 work captured in the sprint markdown doc

The phase delivers a DIRECTION — a committed UX bet the team (solo practitioner) will carry forward into storyboarding. Not a wireframe, not a prototype.

</domain>

<decisions>
## Implementation Decisions

### Critical Screen Priority

- **D-01:** A/B kit comparison is the PRIMARY critical screen — first Crazy 8s round targets this screen
- **D-02:** The Crazy 8s question to answer for A/B comparison: "How do we reduce choice paralysis?" — explore the decision mechanic itself, not just the visual layout
- **D-03:** Style selector is the SECONDARY critical screen — second Crazy 8s round
- **D-04:** HMW notes from Day 1 are the prompts for Crazy 8s — do not start from blank paper; use them to ensure panels are distinct interaction models, not layout variations

### Lightning Demo Set

- **D-05:** 10 products total across 4 categories (see specifics below for per-category focus)
- **D-06:** Consumer tools (Houzz, Homestyler, Planner 5D, Pinterest) — brief 3-field notes: what it does well, what's missing, what mechanism to borrow
- **D-07:** Collaborative tool (Miro/FigJam) — mechanism focus: how individual contributions merge into a shared output — directly analogous to the Couple flow's style profile merge
- **D-08:** Pro tools (Houzz Pro, Modsy, Havenly) — use the specific question sets from the user's research guide (captured in Specifics below)
- **D-09:** AR tools (IKEA Place, Wayfair AR) — use the specific question sets from the user's research guide (captured in Specifics below)

### Solution Sketch

- **D-10:** The 3-panel solution sketch captures the A/B kit comparison moment
  - **Before:** User has a style profile but faces 6 kit options — no clear direction
  - **During:** The comparison mechanic plays out — the specific interaction model that reduces paralysis
  - **After:** User feels confident, not just decided — emotional resolution, not a UI state
- **D-11:** Annotations on the solution sketch explain the design decisions, not just label the UI — a reader must be able to understand the UX bet without verbal explanation (per SKTCH-06)

### Sprint Doc Format

- **D-12:** Crazy 8s done on physical paper — photographed and embedded in the sprint doc
- **D-13:** Sprint doc is a Markdown file in this project (Day 2/ directory), consistent with Day 1 structure
- **D-14:** Doc must include: screenshots/photos of Crazy 8s, lightning demo notes per product, solution sketch photo, written reflection on key choices made

### Claude's Discretion

- Per-category mechanism lens for consumer tools (Houzz etc.): identify what each product does to reduce style/decision uncertainty and where the flow breaks down
- Order of lightning demos within a session: start consumer tools (context), then collaborative (mechanism analogy), then pro tools (client flow), then AR (placement UX)
- Specific format/structure of the Day 2 markdown doc sections

</decisions>

<canonical_refs>
## Canonical References

**Downstream agents MUST read these before planning or implementing.**

### Project Foundation
- `.planning/PROJECT.md` — Core value, constraints, platform architecture, key decisions
- `.planning/REQUIREMENTS.md` — Day 2 requirements: SKTCH-01 through SKTCH-07 with acceptance criteria

### Existing Sprint Work
- `Day 1/Design Sprint Notes Day 1 - Expanded.md` — Full Day 1 notes including problem statements, platform architecture decision, user flow maps for all 4 scenarios, style discovery mechanism, kit selection mechanic, collaborative model

### Assignment Brief
- `Assingment details.rtfd/` — Springboard assignment requirements (source of truth for what must be submitted)
- `Day 2/1686949288_IXC_32.4.2_Design_Sprint__Day_2.pdf` — Day 2 course materials (methodology reference for lightning demos, Crazy 8s, solution sketch format)

</canonical_refs>

<code_context>
## Existing Work Insights

### Reusable Assets
- Day 1 HMW notes: exist in Day 1 notes — use as Crazy 8s prompts (D-04 above)
- Prior competitor notes: Houzz, Homestyler, Planner 5D, Pinterest already sketched in Day 1 notes — build on these, don't re-research from scratch
- 4 user flow maps (Solo, Couple, Pro, AR): documented in Day 1 expanded notes — reference for solution sketch "before" state

### Established Patterns
- Sprint doc structure: Day 1 markdown file sets the template — context, problem statements, flows, decisions, reflections
- Platform architecture: locked in Day 1 — single product, role-based views, desktop primary / mobile AR secondary

### Integration Points
- Day 2 markdown doc connects directly to Day 3 storyboarding — the solution sketch "during" panel becomes the first storyboard panel
- Lightning demo insights feed directly into Crazy 8s HMW prompts — document mechanisms in a way that generates "How might we..." questions

</code_context>

<specifics>
## Specific Ideas

### Lightning Demo Research Guide (from user)

**Professional Tools:**

**Houzz Pro:**
- How do they handle project/client management?
- Can professionals curate product selections for clients?
- How does client sharing and approval work?
- What does the project dashboard look like?

**Modsy:**
- How do they bridge the professional-to-consumer handoff?
- How are room visualizations presented to clients?
- What's the purchase flow — does the professional buy, or does the client?

**Havenly:**
- How do designers present mood boards or product selections?
- How does the client review and approval process work?
- What's the communication model between designer and client?

**AR Tools:**

**IKEA Place:**
- How does AR onboarding work — what does scanning feel like?
- How do you place, move, and swap items?
- What's the path from AR placement to purchase?

**Wayfair AR:**
- Same questions as IKEA Place
- How accurate is style filtering before AR placement?
- Can you view multiple items together or just one at a time?

### Key UX Bet
The solution sketch must communicate one thing clearly: the A/B comparison mechanic that makes a user feel confident in their kit choice, not just guided to one. The emotional outcome is "I chose this" not "I was shown this."

</specifics>

<deferred>
## Deferred Ideas

None — discussion stayed within phase scope.

</deferred>

---

*Phase: 01-day-2-sketch*
*Context gathered: 2026-04-01*
