# Feature Landscape: Sprint Deliverables

**Domain:** UX Design Sprint (GV methodology, Springboard bootcamp)
**Project:** House2Home — home decor starter kit platform
**Researched:** 2026-04-01
**Overall confidence:** HIGH — GV sprint methodology is well-documented in Jake Knapp's "Sprint" (2016), Springboard curriculum materials, and established UX practice

---

## How to Read This File

Each sprint day section covers:
- **What the deliverable is** — definition
- **Table stakes** — minimum required to produce a credible deliverable
- **Differentiators** — what separates passing work from excellent work
- **House2Home specifics** — how this applies to the expanded scope

---

## Day 2 Deliverables

### Deliverable 1: Lightning Demos

**What it is:** A rapid competitive review — 3 minutes per example, capturing the single best idea from each. Not deep analysis; a stimulus for sketching.

**Table stakes (minimum to pass):**
- 3–5 examples reviewed (can be direct competitors, analogous products, or best-in-class UI patterns)
- One specific "captured idea" per demo — not a general summary
- Notes capture what the idea is and why it's relevant to the sprint question
- Prior competitor notes (Houzz, Homestyler, Planner 5D, Pinterest) count if structured this way

**Differentiators (excellent):**
- Covers direct competitors AND analogous domains (e.g., subscription box onboarding, dating app preference matching — for the style selector mechanic)
- Each demo is tied to a specific part of the user flow (style discovery, kit selection, AR visualization, Pro export)
- Captures what NOT to do from failed patterns, not just what works
- Expanded scope is addressed: at least one demo per platform (desktop, mobile AR) and at least one per persona type (consumer, pro)

**House2Home notes:** The pre-existing competitor research (Houzz, Homestyler, Planner 5D, Pinterest) was done before scope expansion. Good lightning demos would add examples for: (1) collaborative decision tools (e.g., how Airbnb or Zola handle multi-user sessions), (2) AR furniture/decor placement (IKEA Place), (3) professional spec export flows.

---

### Deliverable 2: Crazy 8s Sketches

**What it is:** 8 rough sketches in 8 minutes — one per panel, hand-drawn, one idea each. Forces quantity over quality. The goal is to push past the obvious first idea.

**Table stakes (minimum to pass):**
- 8 distinct panels exist (the count matters — it proves you pushed past comfort)
- Each panel sketches a distinct UI idea or variation, not 8 versions of the same screen
- Sketches are for the most critical screen(s) in the sprint — not arbitrary screens
- Hand-drawn is acceptable and expected; pixel precision is not the point
- Panels are labeled or annotated enough that someone else can tell what the idea is

**Differentiators (excellent):**
- Meaningful variation across the 8 panels — early panels show "obvious" ideas, later panels show unexpected angles
- At least 1–2 sketches explore a pattern that wasn't in the lightning demos (novel thinking, not just recombination)
- Annotations explain the core idea briefly (1–2 words per element, not essays)
- Multiple rounds of Crazy 8s for multiple critical screens, or for each persona's key moment
- Sketches show the UI *in context* — not floating elements, but a screen/device frame that implies placement
- For House2Home: Crazy 8s done for the style selector AND the kit A/B comparison, since these are the two mechanics that define the product

**What a bad Crazy 8s looks like (avoid):**
- All 8 panels are minor variations of one design
- Panels left blank or labeled "TBD"
- Sketches too refined — if you're drawing details, you're spending too much time per panel
- Sketches of unrelated screens instead of the critical moment

**House2Home specifics:** The most critical screens to run Crazy 8s on:
1. Style discovery entry — the emoji/word selector mechanic
2. Kit A/B comparison (the 3-round narrowing mechanism)
3. The collaborative merge point (where individual style finds become a shared session)

---

### Deliverable 3: Solution Sketch (3-Panel Storyboard)

**What it is:** A single, detailed 3-panel comic-strip sketch. Not an overview of the whole product — it captures ONE moment in the flow, showing the user's state before, during, and after a key interaction. The best Crazy 8 idea gets refined here.

**Table stakes (minimum to pass):**
- Exactly 3 panels (or a clear beginning, middle, end structure)
- Drawn large enough to be legible — not thumbnail-sized
- Annotated with descriptive text: labels, callouts, or a short caption per panel
- Self-explanatory without a verbal walkthrough — someone should be able to understand the idea without you explaining it
- Based on the sprint question / critical moment (not an arbitrary screen)
- Has a title that communicates the solution concept clearly

**Differentiators (excellent):**
- The 3 panels tell a mini user story: what the user is trying to do (context), the interaction itself (interface detail), and the outcome/value delivered (resolution)
- Interface detail is specific — not "a button here," but the actual label, the layout logic, the visual hierarchy cue
- Annotations explain the *why* of design choices ("shows only 3 options to avoid choice paralysis") not just what is shown
- The sketch reveals something non-obvious about the solution — it's an argument, not just a wireframe
- For expanded scope: multiple solution sketches can address different persona moments (Solo vs. Couple vs. Pro) if each is a distinct 3-panel argument

**What a bad solution sketch looks like (avoid):**
- A single full-page wireframe (not a 3-panel story)
- Panels so rough that intent is unclear without explanation
- No labels or annotations — pure visual with no textual reinforcement
- Covers the whole product flow instead of one critical moment
- The three panels don't logically follow each other (they're three random screens)

**House2Home specifics:** Strong candidates for the primary solution sketch:
- Panel 1: User at style quiz entry, overwhelmed by blank "what's your style?" question → sees emoji/word selector
- Panel 2: Selector in use — showing branching (Know it / AI / Gallery) and the confidence it builds
- Panel 3: User reaches the kit results screen having internalized their own style — "I now know what I want"

A second solution sketch for the Couple flow is a differentiator: it would show the collaborative merge from individual selectors to shared A/B session.

---

## Day 3 Deliverables

### Deliverable 1: Storyboard (5–15 Panels)

**What it is:** A full scene-by-scene map of the prototype you will build on Day 4. This is the screenplay. Every panel = one screen or one decision point in the user journey. The team (or in solo sprints, the sprinter) votes on solution sketches first, then maps the winning concept into a storyboard.

**Table stakes (minimum to pass):**
- 5 panels minimum, 15 maximum — fewer = incomplete flow, more = too much to prototype in one day
- Each panel represents ONE screen or ONE decision/transition — not a cluster of multiple interactions
- Panels are in sequential order representing a real user journey (not a feature list)
- Opening panel establishes the user's entry point and context (where are they, what do they want)
- Closing panel shows a resolution — the user has completed the task or received clear feedback
- Annotations on each panel describe what the user is doing/seeing/deciding (not just what the UI looks like)
- Covers the full critical path from beginning to end

**Differentiators (excellent):**
- Each panel has three layers: (1) what the screen/state looks like, (2) what the user's goal is at that moment, (3) what happens if they succeed or fail
- Decision points are explicit panels — not implied between panels
- The storyboard resolves the sprint question — you can point to the panel where the answer will be tested
- Error states or friction moments are included as panels (not just the happy path)
- Panel count is deliberate: tight enough that Day 4 prototype is feasible in one day
- For multi-persona scope: panels are labeled by persona when the flow diverges, showing the branching architecture clearly
- Each panel could be handed to a prototyper cold and they'd know what to build

**What a bad storyboard looks like (avoid):**
- Panels that represent whole sections of a flow rather than individual screens
- Missing the opening context panel (user just appears on a product page with no setup)
- Missing the closing resolution panel (flow just ends mid-task)
- No annotations — just sketched boxes
- More than 15 panels (prototype will be impossible to build in one day)
- Jumps in logic between panels that require explanation

**House2Home panel count guidance:**
The expanded scope (3 personas, 2 platforms) risks panel bloat. Recommended approach: storyboard ONE primary flow completely (8–10 panels for Solo Mover desktop), then add 3–5 branch panels for either the Couple divergence OR the Pro exit. Mobile AR is a 3-panel branch (enter AR, place item, return to purchase). Total target: 12–15 panels maximum.

**What each panel should include (minimum standard):**
1. A rough sketch of the screen layout (not wireframe-quality, but legible)
2. A title or label (e.g., "Style Quiz — Emoji Selector")
3. A 1–2 sentence description of what the user is doing and deciding
4. Any branching decision clearly marked (arrows to next panel, Y/N paths)

---

### Deliverable 2: Iterated Light Wireframes

**What it is:** Taking the storyboard panels and refining the key screens into slightly more structured wireframes — still low-fidelity, but cleaner than hand sketches. These become the direct blueprint for Figma prototype screens.

**Table stakes (minimum to pass):**
- Wireframes exist for every unique screen in the storyboard (not every panel — repeated screens like a nav bar don't need separate wireframes)
- Layout logic is clear: what is in the header, body, footer, sidebars
- Interactive elements are identified: buttons, inputs, toggles, navigation
- Content hierarchy is visible: headline vs. body vs. CTA distinction exists

**Differentiators (excellent):**
- Annotations explain layout decisions (not just what is there, but why)
- Component reuse is identified: which UI elements appear across multiple screens
- States are captured: empty state, loading state, success state for key interactions
- Figma-ready: wireframe resolution is close enough that moving to Figma requires refinement, not re-invention

---

## Day 4 Deliverables

### Deliverable: Low-Fidelity Prototype in Figma

**What it is:** A clickable, testable "realistic facade" — enough fidelity to simulate the experience for a test participant without revealing it's unfinished. The goal is a prototype that prompts genuine user reactions, not a polished product.

**How realistic does it need to be?**
The GV standard: realistic enough that a user can complete the task without stopping to ask "is this a real app?" Low fidelity means visual polish is optional; cognitive clarity is not. The prototype must look like a real interface even if it doesn't look like a finished one.

**Table stakes (minimum to pass):**
- Every panel from the storyboard has a corresponding Figma frame
- All links required to complete the primary task flow are functional (tapping/clicking moves between screens)
- Key UI elements are labeled with real-ish content, not "Lorem ipsum" — placeholder text that sounds like the actual product
- The prototype can be run from start to finish without the facilitator intervening to advance it
- Exported or shareable via Figma link (for remote testing)
- At minimum: desktop web flow for the Solo Mover persona (the primary test flow)

**Differentiators (excellent):**
- Covers primary persona (Solo Mover) AND at least one secondary persona branch (Couple or Pro)
- Mobile AR screens exist as a separate flow or as linked branch, not skipped entirely
- Micro-interactions are present at key decision points (hover states, button state changes, selection indicators)
- Content is real enough to test: actual product names, plausible prices ($10–$50 range), real-enough decor categories
- Navigation is consistent across screens (header, back behavior, progress indicators where relevant)
- Error states or "wrong path" branches exist so interviews can probe what users do when lost
- Prototype reflects the kit A/B comparison mechanic visually — not just described in a task prompt
- Figma components used where possible so iteration after Day 5 is fast

**What a bad prototype looks like (avoid):**
- Dead links that break the flow mid-task
- Lorem ipsum text anywhere the participant needs to read to make a decision
- Only 2–3 screens for a 5-step flow (participant can't actually complete the task)
- So polished that Day 5 time was spent on aesthetics instead of testability
- Screens that require the facilitator to explain what to tap

**Fidelity calibration for House2Home:**
The most critical screens to get right (sacrifice other screens for these if time is short):
1. Style quiz / selector screen — this is the key differentiator of the product
2. Kit comparison screen (A/B × 3 rounds) — this is the core purchase mechanism
3. Final kit display / add to cart — this is the conversion moment
4. Collaborative merge screen (if testing Couple flow) — this is architecturally novel

The AR visualization screens can be wireframe-level with a placeholder image if needed. What matters is that the flow in/out of AR is testable.

---

## Day 5 Deliverables

### Deliverable 1: Five-Act Interview (x5 participants)

**What it is:** A structured user interview protocol from the GV sprint methodology, run with 5 participants one at a time. The Five Acts are a pacing framework — not five separate activities, but five phases within a single 60-minute session.

**The Five Acts:**

| Act | Duration (approx.) | Purpose |
|-----|--------------------|---------|
| 1. Friendly welcome | 5 min | Put participant at ease; remind them you're testing the product, not them |
| 2. Context questions | 10–15 min | Understand who they are and their real-world behaviors related to the domain |
| 3. Prototype introduction | 2–3 min | Hand off the prototype; give the opening scenario/task prompt |
| 4. Tasks and probing | 30–35 min | Observe the participant navigate the prototype; probe with open questions |
| 5. Quick debrief | 5–10 min | Ask closing questions; capture their summary mental model |

**Table stakes (minimum to pass):**
- 5 interviews conducted (course requirement — not negotiable)
- Act 2 context questions are asked for every participant (skipping this means you have no baseline to interpret their prototype reactions)
- Task prompts in Act 4 are scenario-based, not "click on the style quiz" — participants are given a situation to inhabit
- Probing questions are open-ended: "What were you thinking when you saw that?" not "Did you like it?"
- The facilitator does not help participants when they get stuck — observation of struggle is data
- Notes are taken during or immediately after each session

**Differentiators (excellent):**
- Context questions in Act 2 are persona-calibrated: different opening questions for a Solo Mover vs. a Couple participant vs. a professional designer
- Multiple task prompts exist for testing different branches (e.g., "You and your partner are both doing this together" for Couple flow)
- The facilitator has a prepared list of probing questions for anticipated friction points (the style quiz, the A/B comparison, the AR entry)
- A second observer is present or session is recorded for debrief accuracy (even as a solo student, screen recording the Figma mirror counts)
- Facilitator stays neutral under pressure — no leading responses when participant is confused

**What Act 2 context questions should cover for House2Home:**
- How recently have they moved or redecorated
- Their current process for buying home decor (online, in-store, with help)
- Whether they've used style quizzes, AR apps, or Pinterest boards
- Whether they make purchases alone or with others
- Their confidence level in their own taste (this primes interpretation of the style selector)

**What Act 4 task prompts should cover:**
- Primary task: "You just moved into a new place and want to pull together your bedroom. Use this app to find a starter kit you'd actually buy."
- Secondary task (if time): "Your partner has different taste. Show me how you'd handle that."
- Pro task (if participant is designer persona): "A client just sent you their new apartment dimensions. How would you use this to help them?"

---

### Deliverable 2: Interview Debrief Notes

**What it is:** After all 5 interviews, the team (or solo sprinter) reviews findings using a structured note-taking exercise — typically sticky notes or a shared doc — to identify patterns before making conclusions.

**GV debrief method:** Each observer reviews their notes and calls out observations (not interpretations) one at a time. Observations are grouped by theme or by screen. Patterns that appear in 3+ of 5 interviews are treated as signals.

**Table stakes (minimum to pass):**
- Notes exist from every interview (not just the ones that were interesting)
- Observations are separated from interpretations ("participant scrolled past the A/B screen without interacting" is an observation; "participant didn't understand A/B comparison" is an interpretation)
- Patterns are identified: which behaviors or reactions appeared in 3+ sessions
- A clear summary of what worked and what failed exists for each critical prototype screen
- An explicit "what to fix" list is produced (even if nothing will be fixed — this goes in the case study)

**Differentiators (excellent):**
- Notes are organized by screen/moment, not just by participant — this makes pattern recognition much faster
- Debrief captures both failures AND successes (too many debriefs only document problems)
- Surprising findings are highlighted separately — things participants did that no one predicted
- Debrief includes a confidence rating per finding: "5/5 participants did X" vs. "1 participant said Y" are weighted differently
- Explicit note of which findings change the solution concept vs. which are surface-level polish issues

**Debrief note structure (recommended for House2Home):**

For each critical screen (style selector, A/B comparison, AR entry, collaborative merge, checkout):
- What participants tried to do first
- Where they hesitated or got confused
- What they said spontaneously (quote if possible)
- What they did when stuck
- Did 3+ participants have the same reaction?

---

## Case Study Deliverable

### What a UX Design Sprint Case Study Includes

A case study documents the full process: not just the final prototype, but the thinking, pivots, and learning. For a Springboard bootcamp context, the audience is reviewers/instructors and future employers seeing the work in a portfolio.

**Table stakes (minimum to pass):**
- Project overview: what House2Home is, who it's for, what problem it solves
- Problem statement: clearly articulated, specific (not "people want good decor")
- Process documentation: each sprint day covered with the key deliverable shown
- Deliverable artifacts shown: photos or screenshots of Crazy 8s sketches, storyboard, prototype screens, interview notes
- Key decisions documented: what you chose and why (not just what you built)
- User testing findings: what you learned from the 5 interviews
- Reflection: what you would do differently, what the next iteration would address
- Clearly structured with headers, visual flow — readable in under 10 minutes

**Differentiators (excellent):**

**Process depth:**
- Explains the sprint question and how Day 1 work set up the rest of the sprint
- Documents the scope expansion decision (from single persona to three) and the rationale — this is an unusual and sophisticated choice that should be explained
- Shows Crazy 8s iterations, not just the final solution sketch — the messy middle is part of the story
- Shows storyboard panels, not just the prototype — demonstrates UX thinking, not just UI output

**Findings quality:**
- Interview findings are quantified where possible ("3 of 5 participants expected the A/B screen to refresh automatically")
- Findings are connected to design decisions: "We learned X, which means the next iteration should Y"
- Distinguishes between validated assumptions and invalidated ones
- Captures what would have been cut if the sprint had a real timeline constraint

**Writing quality:**
- Written in first person with clear thinking, not marketing copy
- Explains tradeoffs honestly (e.g., "The AR flow was deprioritized because...")
- Avoids "the user" genericism — refers to personas by name and characteristic
- Clear visual hierarchy: reader can skim to any sprint day and understand what happened

**Portfolio differentiation (goes beyond bootcamp pass):**
- Annotated prototype screenshots that explain design decisions inline
- A "what I'd do with one more week" section
- Side-by-side before/after: early sketch vs. final prototype screen for the same interaction
- Explicit discussion of the expanded scope as a self-directed decision — shows initiative
- Competitive analysis integrated: how House2Home's approach differs from Houzz, Homestyler, etc. and why

**What a bad case study looks like (avoid):**
- Only shows final deliverables — no process artifacts
- Prototype screenshots without annotation or context
- Interview findings that are just "users liked it" / "users didn't like it"
- No reflection or iteration thinking
- Wall of text with no visual anchors
- Generic problem statement that could apply to any product

---

## Consolidated Table Stakes vs. Differentiators

| Day | Deliverable | Table Stakes | Differentiator |
|-----|-------------|-------------|----------------|
| 2 | Lightning demos | 3–5 examples, one captured idea each | Analogous domains covered; tied to specific flow moments |
| 2 | Crazy 8s | 8 distinct panels, most critical screen | Multiple rounds; variation across panels; novel ideas beyond demos |
| 2 | Solution sketch | 3 panels, self-explanatory, annotated | Tells a user story; explains design logic; multiple sketches for persona branches |
| 3 | Storyboard | 5–15 panels, full critical path, annotated | 3-layer panels; explicit decision points; persona branching shown; prototype-ready |
| 3 | Light wireframes | All unique screens, layout logic visible | States captured; component reuse identified; Figma-ready |
| 4 | Prototype | All storyboard panels built, full flow clickable, real-ish content | Multi-persona branches; micro-interactions; error states; AR flow included |
| 5 | Five-Act Interview | 5 sessions, scenario tasks, open probing, notes taken | Persona-calibrated Act 2; recorded/observed; prepared friction probes |
| 5 | Debrief notes | All 5 sessions, observations vs. interpretations, patterns identified | Organized by screen; confidence-rated; successes documented alongside failures |
| Case study | Full process doc | Overview, process per day, artifacts, decisions, findings, reflection | Scope decision explained; Crazy 8s shown; findings quantified; iteration thinking explicit |

---

## Feature Dependencies

```
Lightning demos → Crazy 8s (demos are the stimulus for sketch ideas)
Crazy 8s → Solution sketch (sketch picks and refines best Crazy 8 idea)
Solution sketch → Storyboard (storyboard expands the sketch into a full flow)
Storyboard → Prototype (prototype builds every storyboard panel)
Prototype → Five-Act Interview (nothing to test without prototype)
Five-Act Interview → Debrief notes (notes synthesize the sessions)
All deliverables → Case study (case study documents everything)
```

---

## Sources

**Confidence level: HIGH**

Primary sources (training knowledge, well within knowledge cutoff):
- Jake Knapp, John Zeratsky, Braden Kowitz — "Sprint: How to Solve Big Problems and Test New Ideas in Just Five Days" (2016, Simon & Schuster). The canonical source for all GV sprint methodology.
- GV (Google Ventures) official sprint website: thesprintbook.com
- Springboard UX Design curriculum — Five-Act Interview protocol, sprint deliverable standards
- Nielsen Norman Group — usability testing and interview best practices (well-established methodology)

Note: WebSearch was unavailable during this research session. All content draws from established GV sprint methodology documentation, which is stable and well-codified. The GV sprint framework has not materially changed since 2016. Confidence is HIGH for methodology questions; MEDIUM for Springboard-specific grading rubric nuances (which may vary by cohort/instructor).
