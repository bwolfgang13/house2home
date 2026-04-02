# Roadmap: House2Home Design Sprint

## Overview

Day 1 is complete. This roadmap covers the five remaining phases of the sprint: sketching, storyboarding, prototyping, testing, and the final case study. Each phase maps 1:1 to a sprint day (or post-sprint deliverable). The execution spine is the Solo Mover desktop flow. The Couple merge branch is a small addition to the prototype. The Pro flow and full AR prototype are case study documentation only — not built.

---

## Phases

- [ ] **Phase 1: Day 2 — Sketch** - Lightning demos, Crazy 8s, and solution sketch commit the sprint to one direction
- [ ] **Phase 2: Day 3 — Storyboard** - Scope locked, storyboard built, wireframes created, participants confirmed
- [ ] **Phase 3: Day 4 — Prototype** - Figma prototype built from storyboard, shareable and testable
- [ ] **Phase 4: Day 5 — Test & Validate** - 5 Five-Act Interviews conducted, findings synthesized
- [ ] **Phase 5: Case Study** - Sprint narrative written and submitted to Springboard

---

## Phase Details

### Phase 1: Day 2 — Sketch
**Goal**: A committed solution direction exists — one 3-panel solution sketch identifies the primary UX bet, supported by documented lightning demo insights and Crazy 8s explorations
**Depends on**: Nothing (Day 1 complete)
**Requirements**: SKTCH-01, SKTCH-02, SKTCH-03, SKTCH-04, SKTCH-05, SKTCH-06, SKTCH-07
**Effort**: Moderate
**Success Criteria** (what must be TRUE):
  1. Lightning demos are documented with at least one specific borrowed mechanism per product (not general impressions)
  2. The most critical screen is named and justified in writing before Crazy 8s begins
  3. Crazy 8s panels show distinct interaction models — not layout variations of the same idea
  4. The 3-panel solution sketch tells a complete before/during/after story that a reader can understand without verbal explanation
  5. All Day 2 work is captured in the sprint doc with sketches photographed and a written reflection on key choices

**Critical decisions:**
- Style selector branch vs. A/B kit comparison — one must be named as the primary critical screen before Crazy 8s begins; the other is the secondary screen for the second Crazy 8s round
- Lightning demo targets must include at least one collaborative tool (not just single-user home decor apps)

**Risks:**
- Echo chamber: Crazy 8s panels become layout variations instead of interaction model variations — prevention: use HMW notes from Day 1 as prompts, not blank paper
- Skipping the second Crazy 8s round to save time leaves SKTCH-05 unmet and the secondary screen underexplored

**Plans:** 1/3 plans executed

Plans:
- [x] 01-01-PLAN.md — Prep, lightning demos (10 products), and critical screen decision
- [ ] 01-02-PLAN.md — Crazy 8s Round 1 (A/B kit comparison) and Round 2 (style selector)
- [ ] 01-03-PLAN.md — Solution sketch (3-panel) and final Day 2 documentation

---

### Phase 2: Day 3 — Storyboard
**Goal**: A complete storyboard covers every screen required for the Day 4 prototype, scope is locked to Solo Mover desktop as the spine, participants for Day 5 are confirmed
**Depends on**: Phase 1
**Requirements**: STRY-01, STRY-02, STRY-03, STRY-04, STRY-05, STRY-06, STRY-07, STRY-08
**Effort**: Heavy
**Success Criteria** (what must be TRUE):
  1. Scope decision is documented as a Key Decision before the first storyboard panel is drawn
  2. The storyboard has 8–12 panels covering the full Solo Mover path from style discovery to checkout confirmation
  3. Each panel represents a decision moment or emotional beat — not a screen state — and carries a label and annotation
  4. The storyboard includes a panel for the highest-risk moment (user abandonment or confusion point)
  5. Every screen needed to build the Figma prototype is represented — no prototype screen is missing from the storyboard
  6. Five Day 5 participants are confirmed by name, with session times agreed

**Critical decisions:**
- Couple branch representation: 3–4 annotated variant panels added to the Solo storyboard — not a separate storyboard
- AR branch: labeled branch point and one landing state panel only — not a full track
- Pro flow: noted in a companion annotation, not storyboarded

**Risks:**
- Panel bloat: storyboard exceeds 12 panels and creates ambiguity about which screens must be built; hard cap at 12 total including Couple variant panels
- Figma wireframes not built before Day 3 ends — the wireframes are the Day 4 scaffolding; starting Day 4 without them makes Day 4 unbuildable in time
- Participants not confirmed: arriving at Day 5 without scheduled participants collapses the test phase

**UI hint**: yes

**Plans**: TBD

---

### Phase 3: Day 4 — Prototype
**Goal**: A clickable Figma prototype runs the primary Solo Mover task flow start to finish without facilitator intervention and is shareable via link for remote testing
**Depends on**: Phase 2
**Requirements**: PROT-01, PROT-02, PROT-03, PROT-04, PROT-05, PROT-06, PROT-07, PROT-08, PROT-09
**Effort**: Heavy
**Success Criteria** (what must be TRUE):
  1. A person unfamiliar with the product can complete the primary task flow (style discovery through checkout confirmation) without explanation
  2. All four non-negotiable screens contain real-ish content — actual style names, plausible product names, prices in the $10–$50 range, no lorem ipsum
  3. The style selector offers all three branch entry points (Know it / AI / Browse gallery), with at least one path flowing through completely
  4. The A/B kit comparison mechanic runs through all three rounds with visible progression
  5. The Couple branch is reachable from the prototype — invite mechanism, side-by-side style profiles, and a blended result frame exist (3–4 frames)
  6. The AR concept is represented as a single labeled static frame — present but not interactive
  7. The Figma prototype is shareable via a public link usable for remote testing
  8. The Professional/Architect flow is explicitly documented as out of scope in the sprint doc

**Critical decisions:**
- Hard frame cap: 8–12 frames for the Solo Mover flow; Couple branch adds 3–4; AR adds 1 static frame — total prototype must stay under 17 frames
- Build order: style finder branch first, A/B comparison second, style profile result third, kit detail fourth, everything else fifth, AR and Couple last if time allows
- Fidelity threshold: "realistic facade" — users can make genuine decisions from the content, but pixel-perfect polish is not the goal

**Risks:**
- Fidelity over-investment: polishing early screens consumes time needed for later screens; set a per-screen time budget before starting
- Lorem ipsum anywhere: kills test validity because participants can't make genuine choices without real content
- Prototype not shareable before Day 5 sessions begin: check Figma share settings and test the link from a different device before the first interview

**UI hint**: yes

**Plans**: TBD

---

### Phase 4: Day 5 — Test & Validate
**Goal**: Five usability test sessions are completed using the Five-Act Interview structure, findings are synthesized across participants by screen, and patterns are documented for the case study
**Depends on**: Phase 3
**Requirements**: TEST-01, TEST-02, TEST-03, TEST-04, TEST-05, TEST-06, TEST-07, TEST-08
**Effort**: Heavy
**Success Criteria** (what must be TRUE):
  1. All 5 sessions are conducted using the Five-Act structure: welcome, background questions, scenario tasks, prototype debrief, wrap-up
  2. Act 2 background questions probe purchase confidence and whether participants typically shop alone or with others
  3. Every task prompt is scenario-framed — the participant is told a situation, not instructed to click anything
  4. Structured notes exist per participant per screen (behavior observed, verbatim quote, hesitation point, what they expected)
  5. A debrief is completed after each individual session — not deferred until after all five
  6. Findings are organized by screen and flow section, not by participant
  7. Patterns are defined as behaviors or comments appearing in 3 or more of 5 participants, distinguished from individual observations

**Critical decisions:**
- Participant selection: 3 participants in Solo Mover scenario context, 2 in Couple scenario context; same prototype tested with all 5
- The same interview script is used for all 5 sessions — persona scenario framing is set in Act 1/2, not by using a different instrument
- Sessions are recorded (with permission) and notes are completed immediately after each session, not after all five are done

**Risks:**
- Leading questions in task prompts: cold-read test the script before the first session — any question where "no" feels weird is a leading question
- Late debrief: waiting until after all 5 sessions to analyze findings produces interference between sessions and weakens pattern recall
- Wrong participant profile: participants with professional interior design backgrounds will behave differently; screen against this before Day 5

**Plans**: TBD

---

### Phase 5: Case Study
**Goal**: A submitted case study demonstrates the full sprint process using a Problem -> Bet -> Evidence -> Decision -> Learning narrative, explicitly addresses the expanded scope decision, and meets Springboard assignment requirements
**Depends on**: Phase 4
**Requirements**: CASE-01, CASE-02, CASE-03, CASE-04, CASE-05, CASE-06, CASE-07
**Effort**: Moderate
**Success Criteria** (what must be TRUE):
  1. The case study is structured around the narrative spine — not a per-day process log — with each sprint day contributing to the Problem/Bet/Evidence/Decision/Learning arc
  2. The scope expansion (single persona to 3 personas and 2 platforms) is named explicitly, the rationale is explained, and its effect on each day's work is described
  3. Prototype screenshots or Figma frames are embedded as visual evidence — rough sketches from Day 2 appear alongside the final prototype
  4. Testing findings are presented with quantified patterns ("3 of 5 participants...") and implications for the next design iteration, not just raw notes
  5. Pro flow and AR flow are addressed as "designed but not prototyped" with rationale — neither is ignored nor presented as built
  6. The case study is submitted per Springboard assignment requirements

**Critical decisions:**
- Narrative over log: the case study earns its grade by showing design thinking — what was uncertain, what the bet was, what the evidence showed, what would change
- Expanded scope positioning: lead with why three personas were defined (system-level thinking), explain which persona drove the prototype and why (Solo Mover is the critical path), position other personas as validated through process documentation

**Risks:**
- Writing the case study from memory: all sprint artifacts (Crazy 8s photos, storyboard, Figma link, interview notes) must be gathered before writing begins
- Confirm Springboard-specific rubric requirements against course materials before finalizing — the narrative spine recommendation is solid general UX practice but specific rubric nuances may vary by cohort

**Plans**: TBD

---

## Coverage

| Requirement | Phase | Status |
|-------------|-------|--------|
| SKTCH-01 | Phase 1 | Pending |
| SKTCH-02 | Phase 1 | Pending |
| SKTCH-03 | Phase 1 | Pending |
| SKTCH-04 | Phase 1 | Pending |
| SKTCH-05 | Phase 1 | Pending |
| SKTCH-06 | Phase 1 | Pending |
| SKTCH-07 | Phase 1 | Pending |
| STRY-01 | Phase 2 | Pending |
| STRY-02 | Phase 2 | Pending |
| STRY-03 | Phase 2 | Pending |
| STRY-04 | Phase 2 | Pending |
| STRY-05 | Phase 2 | Pending |
| STRY-06 | Phase 2 | Pending |
| STRY-07 | Phase 2 | Pending |
| STRY-08 | Phase 2 | Pending |
| PROT-01 | Phase 3 | Pending |
| PROT-02 | Phase 3 | Pending |
| PROT-03 | Phase 3 | Pending |
| PROT-04 | Phase 3 | Pending |
| PROT-05 | Phase 3 | Pending |
| PROT-06 | Phase 3 | Pending |
| PROT-07 | Phase 3 | Pending |
| PROT-08 | Phase 3 | Pending |
| PROT-09 | Phase 3 | Pending |
| TEST-01 | Phase 4 | Pending |
| TEST-02 | Phase 4 | Pending |
| TEST-03 | Phase 4 | Pending |
| TEST-04 | Phase 4 | Pending |
| TEST-05 | Phase 4 | Pending |
| TEST-06 | Phase 4 | Pending |
| TEST-07 | Phase 4 | Pending |
| TEST-08 | Phase 4 | Pending |
| CASE-01 | Phase 5 | Pending |
| CASE-02 | Phase 5 | Pending |
| CASE-03 | Phase 5 | Pending |
| CASE-04 | Phase 5 | Pending |
| CASE-05 | Phase 5 | Pending |
| CASE-06 | Phase 5 | Pending |
| CASE-07 | Phase 5 | Pending |

**v1 requirements: 36/36 mapped. No orphans.**

---

## Progress

| Phase | Plans Complete | Status | Completed |
|-------|----------------|--------|-----------|
| 1. Day 2 — Sketch | 1/3 | In Progress|  |
| 2. Day 3 — Storyboard | 0/TBD | Not started | - |
| 3. Day 4 — Prototype | 0/TBD | Not started | - |
| 4. Day 5 — Test & Validate | 0/TBD | Not started | - |
| 5. Case Study | 0/TBD | Not started | - |

---

*Roadmap created: 2026-04-01*
*Granularity: standard*
*Coverage: 36/36 v1 requirements mapped*
