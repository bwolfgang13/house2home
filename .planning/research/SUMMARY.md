# Project Research Summary

**Project:** House2Home Design Sprint — Days 2–5
**Domain:** Solo modified GV 5-day design sprint, multi-persona, multi-platform
**Researched:** 2026-04-01
**Confidence:** HIGH (methodology is well-established canon; tool recommendations are curriculum-aligned)

---

## Executive Summary

House2Home is a home decor starter kit platform being developed through a solo GV-format design sprint as a Springboard bootcamp assignment. Day 1 produced an unusually rich foundation: four user flow maps, three personas (Solo Mover, Couple/Roommates, Architect/Interior Designer), two platform targets (desktop web and mobile AR), and 11 identified test participants. The challenge for Days 2–5 is not generating more ideas — it is committing to one testable hypothesis and protecting that commitment from the gravitational pull of the expanded scope.

The recommended approach across all remaining days is: Solo Mover on desktop web is the spine. The style finder branch screen (Know it / AI / Gallery) is the most critical interaction and the primary test hypothesis. The A/B kit comparison is the second. All other flows — Couple, Pro, AR — are documented as system design decisions in the case study and do not require prototype coverage. The Couple's style merge screens are the one justified secondary branch because they require only 3–4 additional Figma frames added to the Solo flow.

The top risks are scope creep (building too much across three personas), the solo echo chamber (no external friction to challenge design assumptions), and prototype fidelity miscalibration (too polished to build in a day, or too rough to test meaningfully). All three are manageable with explicit rules set before each day starts: one primary persona, one primary platform, 8–12 Figma frames maximum, and a structured five-act interview that tests the prototype rather than the personas.

---

## Key Findings

### Recommended Stack (Tools by Day)

The tool stack for this sprint is driven by two constraints: Figma is a curriculum requirement, and this is a solo sprint against a tight daily time budget. Every tool recommendation optimizes for zero switching cost and maximum reuse across days.

**Core tools by role:**

- **Paper + pen:** Crazy 8s and first-draft solution sketches — speed is the point; no UI tool should be open during ideation
- **Figma:** Storyboard wireframes (Day 3), prototype (Day 4), and prototype sharing for testing (Day 5) — the Day 3 work becomes the Day 4 scaffolding directly; nothing is rebuilt from scratch
- **Zoom or Google Meet + Figma share link:** Day 5 remote testing — one URL, no installation, screen sharing gives behavioral observation data
- **Simple paper or spreadsheet grid:** Post-interview debrief — the simplest tool you will actually use beats a sophisticated one you set up but don't finish

**Tools to avoid:**
- Marvel: no advantage over Figma once you are already building in Figma
- Framer: over-engineered for sprint fidelity; steep setup cost buys nothing at this scale
- InVision: sunset as of 2024; do not use
- Adobe XD: maintenance mode since 2023; do not use
- Lookback / Maze / unmoderated platforms: wrong method for the Five-Act Interview, which is explicitly moderated

### Expected Deliverables (Table Stakes vs. Differentiators)

The deliverables chain is sequential and each day's output is the direct input for the next day. Breaking the chain — by skipping a deliverable or shortcutting its minimum standard — cascades forward.

**Must have (table stakes — course requirements and sprint validity):**

- Day 2: 8 distinct Crazy 8s panels on the most critical screen; a 3-panel solution sketch that is self-explanatory without verbal walkthrough; labeled with the UX bet it represents
- Day 2: 3–5 lightning demos with one specific captured idea per demo (not general summaries)
- Day 3: 8–12 storyboard panels covering the full critical path from entry to order confirmation; each panel = one decision moment, not one screen state; annotations show user goal, not UI description
- Day 3: Light wireframes for every unique screen, with correct layout zones and real-ish button labels
- Day 4: Clickable Figma prototype — every storyboard panel has a corresponding frame, primary task flow runs start to finish without facilitator intervention, real-ish content (not lorem ipsum), shareable via link
- Day 5: 5 Five-Act Interviews conducted; scenario-based task prompts (not "click on X"); open probing questions; structured notes for every session; pattern analysis after all 5

**Should have (differentiators that separate passing from excellent):**

- Crazy 8s that explore radically different interaction models (not 8 variations of the same layout)
- Solution sketch that labels the UX bet explicitly, not just describes the UI
- Storyboard that includes one explicit "failure/abandonment" panel showing the highest-risk moment
- Prototype covering the Couple's style merge as a secondary branch (3–4 additional frames)
- Act 2 context questions tailored to participant's likely persona context
- Debrief notes organized by screen, not by participant — makes pattern recognition faster
- Case study with a narrative spine (Problem → Bet → Evidence → Decision → Learning) rather than a process log

**Defer (not needed for this sprint — document in case study):**

- Professional flow prototype (Pro account, project dashboard, spec export)
- Working AR prototype (static concept screen is sufficient)
- Error states and off-path branches in the prototype
- Couple flow as a full separate storyboard (annotated variant on the Solo storyboard is enough)
- Checkout/payment form detail (one confirmation frame with a "Place Order" button is sufficient)

### Architecture Approach

The sprint architecture for Days 2–5 is a single-spine, two-branch structure. The Solo Mover flow is the spine — it is the only fully prototyped and tested path. The Couple branch grafts onto that spine at one insertion point (after both style finders complete, a merge screen appears before the shared A/B comparison). The AR flow is a three-frame static sidebar. The Pro flow is not prototyped.

**Major components by prototype priority:**

1. **Style finder branch screen** (Know it / AI / Gallery) — Critical; most critical screen in the product; highest risk of user failure; gates all downstream decisions; primary test hypothesis
2. **A/B kit comparison (3 rounds)** — Critical; the core purchase mechanism the product concept rests on; second test priority
3. **Style profile result** — High; the payoff moment that validates the style finder investment; must feel earned
4. **Couple merge screens (C3–C4)** — Medium; architecturally novel; worth the 3–4 extra frames to test whether the merge mechanism is legible
5. **Kit detail + customize** — High; where the purchase decision crystallizes
6. **Landing, checkout, confirmation** — Medium; familiar patterns, need to be clickable but not detailed
7. **AR placement screens** — Low; one static concept mockup labeled as "what AR would show" is sufficient; do not build real AR interaction
8. **Pro dashboard / spec export** — Out of scope for prototype; include in case study as system design documentation

**Recommended Figma file structure:**
- Page 1: Solo Mover Flow (12 frames, fully connected)
- Page 2: Couple Branch (4 frames: C1–C4, connecting back to Frame 05 on Page 1)
- Page 3: AR View (4 frames, low-fidelity, optional connection from Frame 10)

### Critical Pitfalls

1. **Scope Hydra** — The single greatest threat. Three personas and two platforms multiply the decision surface without extending the time budget. Prevention: declare the primary persona and primary platform before Day 2 begins; everything else is case study documentation, not prototype scope. The prototype tests one hypothesis. One persona. One task. Five users.

2. **Solo Echo Chamber** — No team means no external friction. The same brain generating ideas also evaluates them. Prevention: run a deliberate devil's advocate pass after every major decision; write the strongest argument against the chosen direction before moving forward; use Day 1 HMW notes as Crazy 8s prompts to force variety; consider a quick 5-minute informal check with one participant before Day 3 to introduce external friction cheaply.

3. **Prototype Fidelity Miscalibration** — Too polished: Day 4 blows its time budget and users critique aesthetics instead of flow. Too rough: participants spend the test asking clarifying questions. The fidelity test: can someone who has never seen this product complete the primary task without explanation? If yes, it's ready. The hard cap: 8–12 Figma frames maximum for Day 4.

4. **Usability Test Leading Questions** — Scripts written while attached to the design drift toward confirming the design works. Prevention: cold-read test — give the script to someone unfamiliar with the project and check whether any question would feel weird to answer "no" to. Task prompts must describe the scenario, not the solution.

5. **Case Study Written as a Process Log** — Listing what was done per day rather than what was learned, decided, and why. Reviewers are evaluating design thinking, not execution. Prevention: structure the case study around the narrative spine (Problem → Bet → Evidence → Decision → Learning), not the sprint calendar.

---

## Implications for Roadmap

The remaining sprint days have clear sequential dependencies. Each day's output directly gates the next day. The scope constraint must be set explicitly before Day 2, or it compounds into every subsequent day.

### Day 2: Diverge and Commit (Sketching)

**Rationale:** Lightning Demos must happen first — they are the external stimulus that prevents Crazy 8s from being pure self-reference. Crazy 8s produces quantity. Solution sketch commits to one direction. This sequence is non-negotiable; reversing it or merging steps produces the echo chamber pitfall.

**Delivers:** One committed solution direction (the 3-panel solution sketch) plus raw ideation evidence (Crazy 8s) for the case study

**Key decisions before starting:**
- Confirm primary persona: Solo Mover
- Confirm primary platform: Desktop web
- Identify the 2–3 critical screens to sketch (style finder branch and A/B comparison are mandatory; everything else is optional)
- Lightning demo targets: style/personality quiz UX (Warby Parker, Typeform), A/B comparison interfaces, collaborative decision tools, AR placement (IKEA Place)

**Addresses:** Style finder branch (the sprint hypothesis), A/B comparison layout variations
**Avoids:** Echo chamber (3 rounds of Crazy 8s; different mental model per panel — not different layouts of the same model), scope hydra (one solution sketch, primary persona only)

**Research flags:** None — methodology is well-established. Do not over-engineer the day structure.

---

### Day 3: Sequence and Translate (Storyboard + Wireframes)

**Rationale:** The storyboard is the screenplay for the prototype. Building it before opening Figma prevents the most common Day 4 failure: building screens that don't add up to a flow. The storyboard also forces the failure moment to be acknowledged before it's discovered in testing.

**Delivers:** An 8–12 panel storyboard (Solo spine + Couple branch variant) plus Figma wireframes that become Day 4 scaffolding

**Scope constraints for this day:**
- Solo Mover storyboard: 8–10 panels maximum
- Couple branch: 3–4 annotated variant panels (not a separate storyboard)
- Pro flow: mentioned in a companion note, not storyboarded
- AR: 2–3 panels maximum, clearly labeled as conceptual

**Build order in Figma (once storyboard is committed):**
1. Style finder branch screen (the hypothesis — get this right first)
2. A/B comparison screens (rounds 1–3)
3. Style profile result screen
4. Kit detail screen
5. Everything else (landing, customize, cart, confirmation)
6. AR placeholder screens last, if time remains

**Addresses:** Complete testable flow, Couple merge screens, explicit failure/risk panel
**Avoids:** Wireframe dump (each panel = decision moment, not screen state), panel bloat (cap at 12 total), missing the failure moment (add it explicitly)

**Research flags:** Standard patterns apply. No deeper research needed. The Figma-as-storyboard-tool decision is straightforward.

---

### Day 4: Build the Test Instrument (Prototype)

**Rationale:** The prototype is not the product — it is a test instrument. Every hour spent on polish beyond the "realistic facade" threshold is an hour not testing the hypothesis. The hard constraints must be set before opening Figma.

**Delivers:** A clickable Figma prototype that runs the primary task flow start to finish without facilitator intervention, shareable via link

**Hard constraints:**
- 8–12 frames maximum for the Solo flow
- Real-ish content required: actual product names, plausible prices ($10–$50 range), real style names
- AR: one static concept frame with a label ("This represents what AR would show") — do not attempt real AR interaction
- Couple branch: build only if Solo flow is complete with time remaining; 3–4 additional frames
- Do not build Pro flow at all

**Prototype connections (minimum wired paths):**
- Style finder → branch screen → style profile result → A/B round 1 → A/B round 2 → A/B round 3 → kit detail → add to cart → confirmation
- Couple branch entry → C1 → C2 → C3 → C4 → A/B round 1
- AR entry → AR concept screen → return to kit detail

**Addresses:** Testable style finder branch, testable A/B comparison, real-ish content for genuine participant decisions
**Avoids:** Fidelity over-investment (hard frame cap), building the wrong flows (declare scope before starting), lorem ipsum (kills test validity)

**Research flags:** None — Figma prototype methodology is extremely well established. The decisions are scope decisions, not research questions.

---

### Day 5: Test and Learn (Five-Act Interviews + Debrief)

**Rationale:** The Five-Act Interview structure is the GV sprint methodology's most validated element. The risk on Day 5 is not methodology failure — it is participant selection and script quality. Both must be prepared before the first session.

**Delivers:** 5 interview sessions with structured notes, pattern analysis, and an explicit "what to fix" list

**Participant selection (from the 11 identified):**
- Priority criterion: has moved or is about to move, no professional interior design background
- Assign 3 participants to Solo Mover context, 2 to Couple context, 1 of the 5 with design/procurement background for Pro verbal probe only
- Test the same prototype with all 5 — persona context is a scenario framing variable, not a segmentation strategy

**Script quality check:**
- Every task prompt must describe a scenario, not a solution ("You just moved in and want to make it feel like home" not "Use the style quiz to find a kit")
- Cold-read test: would any question feel weird to answer "no" to?
- Debrief evaluative questions happen in Act 4/5 only — not during task observation

**Note-taking:** Use a structured template per participant (behavior observed / verbatim quote / point of hesitation / what they expected). Record sessions with permission; fill the template immediately after, not days later. Do not wait for all 5 sessions to debrief.

**Pattern threshold:** 3 of 5 participants sharing a behavior = finding. Fewer = note but do not generalize.

**Addresses:** Five-act protocol execution, pattern recognition, explicit findings for case study
**Avoids:** Leading questions, wrong participant profile, vague notes that cannot support case study claims

**Research flags:** Standard methodology — no deeper research needed. The one area requiring judgment is participant selection mapping (Day 1 participant notes needed to finalize the 5 slots).

---

### Case Study: Narrative, Not Log (Post-Sprint)

**Rationale:** The case study is the portfolio artifact that demonstrates design thinking. Its value is proportional to how clearly it communicates the design bet, the evidence gathered, and the reasoning behind decisions — not how thoroughly it documents the sprint calendar.

**Delivers:** A portfolio case study that demonstrates system-level thinking (3 personas, 2 platforms) while showing focused execution (one prototype, one primary test)

**Narrative spine:**
1. Problem — what was uncertain and what was at stake
2. Bet — which hypothesis the sprint was testing and why (style finder branch confidence)
3. Evidence — what the prototype and testing revealed (quantified: "3 of 5 participants...")
4. Decision — what the next iteration would address based on that evidence
5. Learning — what would be done differently

**Expanded scope positioning:** Lead with why three personas were defined (system-level thinking), explain which persona drove the prototype and why (Solo Mover is the critical path), then position other personas as validated through process documentation. This reads as sophisticated scoping judgment, not scope padding.

**Addresses:** All sprint days, scope decision rationale, testing findings, iteration thinking
**Avoids:** Process log format, showing polished Figma without showing rough sketches, quoting participants without synthesizing meaning, omitting what was cut and why

**Research flags:** Case study structure guidance is MEDIUM confidence (community standards, not a single authoritative source). The narrative spine recommendation is solid; specific Springboard rubric nuances may vary by cohort/instructor and should be confirmed with the course materials.

---

### Phase Ordering Rationale

- Days are strictly sequential — each day's output is the direct input to the next
- The scope declaration must happen before Day 2, not during it; ambiguity compounds at every step
- Figma work begins on Day 3 (storyboard), not Day 4 — this is the key efficiency decision that makes Day 4 achievable; reversing this makes Day 4 impossible
- The Couple branch is the only secondary flow worth building because it reuses all of the Solo frames after the merge point; it is not a separate prototype, it is a 3-frame insertion
- AR and Pro are explicitly deferred to case study documentation — this is not a compromise, it is the correct sprint strategy for flows that are documented but not yet at risk

### Research Flags

**Phases that need additional research or judgment before execution:**
- Participant selection mapping (Day 5): Day 1 notes on each of the 11 participants are needed to finalize the 5 slots against the Solo Mover screening criteria. This is not a research question — it is a data access question.
- Case study rubric specifics: Springboard-specific grading criteria may differ from general UX portfolio guidance. Confirm with course materials before writing.

**Phases with standard, well-documented patterns (no additional research needed):**
- Day 2 (Crazy 8s + solution sketch): GV methodology is canonical and fully documented
- Day 3 (storyboard + wireframes): standard sprint practice; Figma-as-storyboard is a well-established approach
- Day 4 (Figma prototype): methodology and tool are extremely well established
- Day 5 (Five-Act Interview): directly from the GV sprint playbook, widely validated

---

## Confidence Assessment

| Area | Confidence | Notes |
|------|------------|-------|
| Stack (tools) | HIGH | Figma is curriculum requirement; tool comparison draws on training data through Aug 2025; InVision/XD deprecation should be spot-checked if currency is critical |
| Features (deliverable standards) | HIGH | GV sprint deliverable standards are stable and well-codified since 2016; Springboard-specific rubric is MEDIUM |
| Architecture (sprint workflow) | HIGH | GV methodology is canonical; solo sprint adaptation is grounded in documented sprint principles |
| Pitfalls | HIGH (methodology) / MEDIUM (project-specific) | Echo chamber, fidelity, leading questions are HIGH confidence from established literature; scope hydra risk specific to this project is analyst judgment |

**Overall confidence: HIGH**

### Gaps to Address

- **Participant background data:** PITFALLS.md could not map the 11 participants to personas because Day 1 notes were not available to the research agent. Before scheduling Day 5, review Day 1 interview/recruitment notes and screen the 11 names against the Solo Mover criteria (recently moved or about to move; no professional design background).

- **Springboard rubric specifics:** Deliverable standards in FEATURES.md reflect GV methodology and general UX portfolio practice. The specific rubric Springboard uses for grading this sprint may have nuances not captured here. Verify with course materials, particularly for the case study section.

- **WebSearch unavailability:** All four research agents operated without live web search. Tool deprecation claims (InVision sunset, Adobe XD maintenance mode) are based on training data through August 2025 and are reliable but worth a quick spot-check if using these tools is under consideration (it should not be).

---

## Sources

### Primary (HIGH confidence)

- Jake Knapp, John Zeratsky, Braden Kowitz — *Sprint: How to Solve Big Problems and Test New Ideas in Just Five Days* (2016, Simon & Schuster) — canonical GV sprint methodology, Five-Act Interview, Crazy 8s, solution sketch, storyboard
- GV official sprint resources — thesprintbook.com — sprint facilitation guides including solo adaptations
- Figma documentation (2025) — Auto Layout, components, prototyping connections
- Nielsen Norman Group — usability testing and interview methodology
- Steve Krug — *Rocket Surgery Made Easy* (2010) — usability test facilitation and leading question patterns

### Secondary (MEDIUM confidence)

- UX Collective, ADPList, General Assembly portfolio review community standards — case study narrative structure
- Springboard UX Design curriculum (general) — Five-Act Interview protocol and sprint deliverable standards; specific rubric nuances LOW confidence

### Tertiary (LOW confidence)

- Analyst judgment on scope hydra risk specific to House2Home — inferred from project context and GV narrowing methodology; not sourced from external literature

---

*Research completed: 2026-04-01*
*Ready for roadmap: yes*
