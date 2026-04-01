# Architecture Patterns: Sprint Workflow for Expanded Scope

**Domain:** UX Design Sprint — multi-persona, multi-platform
**Project:** House2Home
**Researched:** 2026-04-01
**Confidence:** HIGH (GV sprint methodology is well-established; recommendations are grounded in sprint principles, not speculation)

---

## The Core Problem This Document Solves

Day 1 produced four user flow maps and three problem statements. That is richer than a standard sprint brief. The risk is not having too much — it is trying to honor everything equally across Days 2–5. A sprint only works when you commit to one focused prototype. The architecture of the remaining days is fundamentally about how to make that commitment without wasting the expanded scope you already built.

---

## Decision 1: Primary Persona for Sketching and Prototyping

**Recommendation: Solo Mover is the primary focus.**

**Rationale:**

The Solo Mover flow is the system's critical path. Every interaction that exists for the Couple and the Professional is a variant or extension of what the Solo Mover does. The style finder, the A/B kit comparison, the AR handoff, the cart — all of these originate in the Solo flow. If the Solo Mover experience is broken or unclear, the collaborative and professional layers have no foundation to build on.

The Couple flow adds one novel mechanism on top of the Solo flow: the style profile comparison and blending step. That is one screen group, not a separate flow.

The Professional flow is a different product mode entirely (Pro account, project management, spec export). Prototyping it in parallel would require building two separate mental models and would double your Figma scope without doubling your learning.

**The rule of thumb from GV sprint methodology:** prototype the riskiest assumption, not the most complete story. The riskiest assumption in House2Home is whether the style discovery mechanism (emoji/word selector + branching) gives users enough confidence to commit to a kit. That assumption lives most purely in the Solo Mover flow.

**What this means practically:**
- Day 2 Crazy 8s: sketch variations of the style finder and the A/B comparison screens
- Day 2 Solution Sketch: draw the Solo Mover flow end-to-end
- Day 3 Storyboard: build panels around the Solo Mover path
- Day 4 Prototype: build Solo Mover in Figma; add the couple's style merge screen as a secondary branch if time permits

The Professional flow is documented (Day 1) and can be referenced in the case study as a system-level design decision. It does not need to be prototyped to demonstrate that you thought about it.

---

## Decision 2: How to Identify the "Most Critical Screen"

**Recommendation: The style finder branch screen (Know it / AI / Gallery) is the most critical screen.**

**Framework for deciding:**

When multiple personas exist, the most critical screen is the one that:
1. Carries the highest risk of user failure or abandonment
2. Is unique to this product (not a pattern users already know)
3. Gates everything downstream — if users don't pass this point, nothing else matters

Apply this to House2Home:

| Screen | Risk of Failure | Unique Mechanism | Gates Downstream |
|--------|----------------|------------------|-----------------|
| Landing / entry | Low — familiar pattern | No | No |
| Style finder (emoji/word selector) | Medium | Yes | Yes |
| **Style finder branch (Know it / AI / Gallery)** | **High** | **Yes** | **Yes** |
| A/B kit comparison | Medium | Yes | Yes |
| Kit customization | Low | No | No |
| Checkout | Low — familiar pattern | No | No |

The style finder branch is where users must understand what each option means and choose correctly for their actual situation. A user who picks "AI Generate" when they actually know their style will feel the flow is slow. A user who picks "I know my style" and then gets stuck will abandon. This branching moment is the most fragile interaction in the system.

**The A/B kit comparison is the second most critical screen.** It is the mechanism the whole product concept rests on. If users find it confusing (too many choices, not enough differentiation, unclear criteria) the kit selection collapses.

**Implication:** Day 2 Crazy 8s should produce at least 3–4 variations of the style finder branch screen and 2–3 variations of the A/B comparison screen. These are your sketching priorities, not the checkout or the AR handoff.

---

## Decision 3: Build Order — Solo First, Then Collaborative Features

**Recommendation: Build Solo Mover completely, then layer in the Couple's style merge as a branch.**

**The dependency map:**

```
Solo Mover prototype (complete path)
    └── Couple's merge screen (one new screen group inserted after individual style finders)
            └── Shared A/B session (reuses Solo's A/B screens — same UI, different context)
```

The Couple flow is not a separate prototype. It is the Solo flow with one insertion point: after both individuals complete their style finders, a new "styles compared" screen appears before proceeding to the A/B kit comparison. From that merge screen onward, the interface is functionally identical to Solo.

**Build order:**
1. Complete the Solo Mover flow from style finder entry through order confirmation
2. Add the style profile comparison screen as a branch off the style finder completion screen
3. Connect that branch back into the shared A/B comparison (same Figma frames, different entry annotation)

This approach means you build one prototype, not two, and the collaborative scenario tests whether the merge mechanism makes sense — which is its own distinct risk worth validating.

**Do not build the Professional flow in the prototype.** Log it as a system design decision in the case study. If a participant happens to be a designer or architect, you can describe the Pro mode verbally and ask for reactions without prototyping it.

---

## Decision 4: Storyboard to Figma Structure

**How a storyboard panel maps to Figma:**

A storyboard panel represents a moment of user experience, not necessarily a single screen. The translation rule is:

| Storyboard Panel Type | Figma Equivalent |
|----------------------|------------------|
| Context / opening scene (who, where, why) | Not a Figma frame — this is your test script intro |
| User arrives at product | Frame: Landing / entry screen |
| User makes a choice | Frame: The screen where the choice appears |
| System responds | Frame: The result screen (style profile generated, etc.) |
| User interacts with mechanism | 2–3 frames showing the interaction state (before, during, after) |
| Moment of realization or decision | Frame: The key decision screen — give it full detail |
| User completes goal | Frame: Confirmation / success screen |

**Recommended Figma structure for House2Home:**

```
Page 1: Solo Mover Flow
    Frame 01 — Landing screen
    Frame 02 — Style Finder (emoji/word grid)
    Frame 03 — Branch screen (Know it / AI / Gallery)
    Frame 04a — AI Generate result (style profile card)
    Frame 04b — Gallery browse (if branching tested)
    Frame 05 — A/B Comparison Round 1 (Kit A vs Kit B)
    Frame 06 — A/B Comparison Round 2 (narrowed)
    Frame 07 — A/B Comparison Round 3 (final selection)
    Frame 08 — Chosen Kit detail (items, cost, breakdown)
    Frame 09 — Customize Pack (swap items)
    Frame 10 — AR handoff prompt (optional exit point)
    Frame 11 — Add to Cart + Add-ons
    Frame 12 — Order Confirmation

Page 2: Couple Branch (shared with Page 1 after merge)
    Frame C1 — Style Profile A Generated
    Frame C2 — Style Profile B Generated
    Frame C3 — Side-by-side comparison (overlap highlighted)
    Frame C4 — Blended style suggested + both confirm
    [connects to Frame 05 on Page 1]

Page 3: AR View (optional, low-fidelity acceptable)
    Frame AR1 — Scan prompt
    Frame AR2 — AR overlay with kit items placed
    Frame AR3 — Item manipulation (move/swap)
    Frame AR4 — Confirm and return / checkout in app
```

**Prototype connections:**
- Primary path (Solo): 01 → 02 → 03 → 04a → 05 → 06 → 07 → 08 → 09 → 11 → 12
- Couple branch entry: after both style finders → C1 → C2 → C3 → C4 → Frame 05
- AR branch entry: Frame 10 → AR1 → AR2 → AR3 → AR4

**Fidelity guidance:**
- Frames 02, 03, 05–07, 08: High detail — these are the test targets
- Frames 01, 11, 12: Medium detail — functional but not the focus
- AR frames: Low detail — enough to communicate the concept, not to test AR mechanics
- Couple frames C3–C4: Medium detail — the merge mechanism is worth testing

---

## Decision 5: Testing Structure Across 5 Participants with 3 Personas

**Recommendation: Test the Solo flow with all 5 participants. Use persona context as a framing variable, not a segmentation variable.**

**The constraint:** 5 participants is too few to distribute across 3 personas and get statistically meaningful signal from any one group. If you assign 2 participants to Solo, 2 to Couple, and 1 to Pro, you learn nothing reliable about any of them.

**The principle:** In a GV sprint, you are not validating personas — you are validating the prototype. The prototype is the Solo Mover flow. Everyone tests the same prototype.

**How to use personas within a unified test:**

Assign each participant a scenario context at the start of the test. This gives them a real-life frame of reference without changing what they're testing:

| Participant | Persona Context (Test Script Framing) | What They Test |
|-------------|--------------------------------------|----------------|
| P1 | "You just moved into your first apartment alone..." | Solo flow, full path |
| P2 | "You and your partner just moved in together..." | Solo flow + couple branch screen (C3–C4) |
| P3 | "You just moved into a new place and want to decorate quickly..." | Solo flow, full path |
| P4 | "You and a roommate are trying to agree on a style..." | Solo flow + couple branch screen |
| P5 | "You're a designer looking to source items for a client..." | Solo flow; verbal probe on Pro mode at end |

**What this structure achieves:**
- All 5 participants validate the core mechanism (style finder, A/B comparison)
- 2 participants validate the couple merge screens specifically
- 1 participant gives qualitative signal on whether the Pro concept makes sense without requiring a prototype
- You have 5 data points on every critical screen, not 1–2 per persona

**Recruiting from your identified list:**
- Anna, Orion, Isa — likely strong fits for Solo or Couple context
- Craig, Seth — possible Pro context if professional background
- Ray, Sadie, Mary — consumer contexts
- Eli, Nathaniel, Birdie — fill remaining slots based on actual availability and background

Do not over-engineer participant selection. The most important thing is that participants are willing to talk through their thinking. Context-fit is secondary.

**Test script structure (Five-Act Interview applied to this prototype):**

1. **Welcome and warm-up** (5 min) — background questions about decorating experience, moving history
2. **Context setting** (2 min) — give them their scenario framing (one of the five above)
3. **Prototype exploration** (20–25 min) — think-aloud while navigating; do not guide, only observe
4. **Probing questions** (10 min) — "What would you do next?", "What made you confident here?", "Where did you feel stuck?"
5. **Close** (5 min) — overall reactions, anything missing, what they'd tell a friend

---

## Sprint Day-by-Day Architecture for Remaining Days

### Day 2: Sketching

**Goal:** Generate and select the best solution for the most critical screens.

**Lightning demos (first):** Look at 4–6 products for inspiration on specific mechanisms:
- Style quiz / personality quiz UX (e.g., how Warby Parker or Typeform handles branching)
- A/B comparison interfaces (e.g., how insurance or subscription comparison sites structure choices)
- Collaborative decision tools (e.g., how Doodle or shared wishlists handle joint input)
- AR placement UX patterns (e.g., IKEA Place, Houzz AR)

Demos should be narrow. You are not reviewing entire products — you are capturing one specific mechanism from each.

**Crazy 8s:** 8 sketches in 8 minutes. Focus on:
- The style finder branch screen (variations on how the three paths are presented)
- The A/B comparison screen (variations on layout, information hierarchy, decision criteria)

Do not sketch the landing page or checkout. Those are standard patterns with low learning value.

**Solution sketch (3-panel):** Draw the critical moment as a sequence:
- Panel 1: User arrives at style finder and makes initial selections
- Panel 2: User hits the branch screen and chooses a path
- Panel 3: Style profile is generated and user sees their result

This is the hypothesis you are committing to prototype.

### Day 3: Storyboarding and Wireframes

**Goal:** Expand the solution sketch into a full storyboard, then translate to Figma wireframes.

**Storyboard (5–15 panels):** Follow the Solo Mover path from arrival to order confirmation. Include the couple branch as panels 4a–4c (clearly labeled as the alternate path). Do not storyboard the Professional flow.

Recommended panel count: 10–12 panels for Solo, 3 additional for couple branch.

**Wireframe iteration:** Start in Figma with low-fidelity frames. The order of frames to build first:
1. Style finder branch screen — this is your hypothesis; get it right before anything else
2. A/B comparison screens (rounds 1–3) — these are the core mechanism
3. Style profile result screen — the payoff moment users need to feel
4. Kit detail screen — where the purchase decision crystallizes
5. Everything else in order (landing, customize, cart, confirmation)

Do not spend Day 3 time on the AR frames. Build placeholder screens you can click through.

### Day 4: Prototyping

**Goal:** A clickable Figma prototype that can be handed to a participant with minimal explanation.

**Build to this spec:**
- Every frame a participant might land on must have enough visual detail to seem real
- Dead-end states are acceptable if they are clearly outside the test path
- Transitions should be simple (instant or basic dissolve — no animations)
- Prototype should work on desktop (present via browser or Figma mirror)
- Couple branch should be demoable as an alternate starting path

**What to leave out of the Day 4 prototype:**
- Real product images (use placeholders with style labels)
- Actual pricing (use representative numbers)
- Working AR (use static mockup screenshots)
- Error states (no time; note them for post-sprint iteration)

**Figma file hygiene for the case study:** Name frames clearly. Organize by page (Solo / Couple Branch / AR). This file will become a portfolio asset — structure it so a reader can follow the flow without your narration.

### Day 5: Testing

**Goal:** 5 interviews, patterns identified, findings documented.

**Session logistics:** Each session 45–50 minutes. Use the five-act structure above.

**Note-taking method:** For each session, capture on a simple grid:
- Screen name | What participant did | What participant said | Observation (positive / confusion / failure)

After all 5 sessions, look for patterns: which screens generated confusion in 3+ sessions. That is your signal. One participant struggling is noise. Three is a finding.

**Debrief structure:**
1. List every observation across all sessions
2. Group by screen
3. For each group: does this represent a usability failure, a copy/label problem, or a flow problem?
4. Prioritize: what would need to change before this could ship?

---

## Component Boundaries Summary

| Component | Scope | Prototype Priority |
|-----------|-------|-------------------|
| Style finder (entry + selector) | Solo, Couple, Pro | High |
| Branch screen (Know it / AI / Gallery) | All personas | Critical |
| Style profile result | All personas | High |
| Couple merge screen (C3–C4) | Couple only | Medium |
| A/B kit comparison (3 rounds) | Solo, Couple | Critical |
| Kit detail + customize | Solo, Couple | High |
| AR handoff prompt | Solo, Couple | Low (placeholder) |
| AR placement interface | All personas | Low (static mockup) |
| Pro project dashboard | Pro only | Out of prototype scope |
| Spec export | Pro only | Out of prototype scope |
| Checkout + confirmation | All personas | Medium (familiar pattern) |

---

## Architecture Principles for This Sprint

**1. The prototype is a test instrument, not a product demo.**
Build only what is needed to generate a testable reaction. Everything else is documentation.

**2. One primary path, one branch.**
Solo Mover is the primary path. Couple merge is the only branch worth prototyping. Everything else is described, not built.

**3. The case study carries the expanded scope.**
The three personas and two platforms do not all need to appear in the prototype — they need to appear in your process documentation. Day 1 built the system map. Days 2–5 validate one critical path within it. The case study connects them.

**4. Test the mechanism, not the persona.**
All 5 participants test the same prototype. Persona context is a test script variable that makes the scenario feel real. It is not a segmentation strategy.

**5. Fidelity is proportional to risk.**
High-risk screens (style finder branch, A/B comparison) get the most design detail. Low-risk screens (checkout, confirmation) get enough to be clickable.

---

## Sources

- GV Design Sprint methodology (Jake Knapp, *Sprint*, 2016) — HIGH confidence, canonical source
- Sprint process knowledge grounded in training data through August 2025 — HIGH confidence for established methodology
- Figma prototype structure recommendations — grounded in standard UX practice, HIGH confidence
- WebSearch unavailable during this research session; all findings derived from methodology knowledge and project-specific analysis of Day 1 artifacts
