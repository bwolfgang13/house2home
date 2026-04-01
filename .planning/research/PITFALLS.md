# Domain Pitfalls: Solo UX Design Sprint

**Project:** House2Home — Springboard UX Bootcamp Design Sprint
**Domain:** Solo modified GV 5-day design sprint, multi-persona, multi-platform
**Researched:** 2026-04-01
**Confidence:** HIGH for methodology pitfalls (well-established GV canon + UX research literature); MEDIUM for scope-specific risks (inferred from project context); LOW where flagged

---

## The Overarching Risk for This Specific Project

Before the individual pitfalls: the single biggest threat to this sprint is that Day 1 scope expansion has created a structural tension that will surface on every remaining day. Three personas and two platforms means the sprint has roughly 3-4x the decision surface of a standard single-persona sprint — but the same time budget and a team of one.

Every pitfall below is amplified by this expansion. Read them with that lens.

---

## Critical Pitfalls

Mistakes that cause rewrites, failed usability tests, or a case study that reads as unfocused.

---

### Pitfall 1: The Solo Echo Chamber

**Affects:** Days 2, 3, 4 (Sketching, Storyboard, Prototype)

**What it looks like:**
You sketch 8 ideas in Crazy 8s, evaluate them, pick one — and every single decision confirms your original instinct from Day 1. No idea gets challenged. The "best" solution is the one you already believed in before you drew anything. The sprint process becomes retroactive justification rather than genuine exploration.

In a team sprint, a Decider breaks ties and other people's sketches force you to engage with assumptions you didn't know you had. Solo, there is no external friction.

**Why it happens:**
Without a team, the same brain that generates ideas also evaluates them. Cognitive biases (anchoring, confirmation bias, the IKEA effect — you love ideas you built) operate unchecked. The sprint structure is designed with team friction as a feature. Solo sprints remove that feature.

**Consequences:**
- You prototype the first good idea, not the best available idea
- Usability test failures feel surprising rather than anticipated
- Case study reads as "I built what I planned" rather than "the process shaped the outcome"

**Prevention:**
- Schedule a deliberate "devil's advocate" pass after every decision. Write down the strongest argument against the solution you're about to move forward with before moving forward.
- Use the **How Might We** + **Vote dot** ritual even when solo: write your HMW notes, let them sit overnight, then dot-vote cold.
- Treat Day 2 Lightning Demos as genuine constraints: if a competitor already solved this in a way you hadn't thought of, update your sketch direction before Crazy 8s.
- For this project specifically: ask one of your 11 test participants an informal 5-minute question about a key assumption before Day 3. Cheap external friction.

---

### Pitfall 2: Scope Hydra — Three Personas, Two Platforms

**Affects:** Every day, but most damaging on Days 3 and 4 (Storyboard and Prototype)

**What it looks like:**
Each time you try to constrain scope, you realize the excluded persona or platform still matters for the thing you kept. The Solo Mover flow seems simple until you realize the AR view needs to work differently there. The Couple flow needs the collaborative style-finder. The Pro flow needs spec export. None of them share a single storyboard cleanly. You end up with four parallel storyboards, then four prototype flows, and by Day 4 you have something too large to build and too diffuse to test.

**Why it happens:**
Expanding scope in Day 1 before the sprint methodology's built-in scope-limiting mechanisms (Heat Map voting, Storyboard narrowing) had a chance to operate. The expansion was additive. The sprint's discipline is subtractive. The two impulses haven't been reconciled.

**Consequences:**
- Prototype takes 2-3x as long as allocated → either deadline slips or fidelity collapses
- Usability test has no single testable hypothesis — participants are testing different things and findings are incomparable
- Case study lacks a coherent narrative spine: "we tested everything" is not a sprint story

**Prevention:**

**Pick one primary persona and one primary platform as the spine of Days 3-5.** The other personas and the AR platform become documented decision branches — shown in the case study as considered, not abandoned.

For this project, the recommended spine is:
- **Primary:** Solo Mover, Desktop Web, style discovery → kit selection → checkout
- **Secondary (documented, not prototyped):** Couple collaborative flow as an annotated storyboard variant; Pro as a role-based view difference; AR as a connected companion documented in architecture

This lets you say in the case study: "I designed a system that accounts for three user types. I prototyped and tested the highest-risk flow (Solo Mover completing a first purchase). The other personas were validated through process documentation and peer review."

**The rule:** The prototype tests one hypothesis. One persona. One task. Five users. That is the sprint format, even when the design system it sits inside is broader.

---

### Pitfall 3: Storyboard That's Actually a Wireframe Dump

**Affects:** Day 3

**What it looks like:**
The storyboard has 15 panels, each showing one screen state. Panel 1: homepage. Panel 2: style selector open. Panel 3: emoji selected. Panel 4: branch screen. It reads like annotated wireframes, not a story.

**Why it happens:**
Storyboards feel like they should show screens because you're a designer. But the GV storyboard's purpose is to de-risk the prototype build, not to document UI. The panels should show **moments of decision and transition**, not UI states.

**Consequences:**
- You miss the connective tissue: what does the user feel/think between screens?
- The prototype ends up as a collection of screens without a through-line
- Reviewers and interviewers who read the case study don't understand why screens exist

**Prevention:**
Each panel should answer: "What is the user trying to accomplish right now, and what does success look like for this moment?" If the answer is "they're on the homepage," that's not a panel — that's a screen. The panel is "they land and feel uncertain, see the style quiz CTA, decide to try it."

**The right storyboard for this project has:**
- An opening scene (context: who is this person, what just happened that brought them here)
- 2-3 key decision moments (not every micro-interaction, just forks in the road)
- One moment of potential failure or confusion (the thing you're most worried about)
- A closing scene (they completed the task — what do they do next?)

Target: 8-10 panels, not 15. If you have 15, you're wireframing.

**What gets overdone:**
- Annotating every UI element in the storyboard panels (save that for the prototype)
- Drawing both "happy path" AND "error state" paths in the storyboard (pick the happy path; test catches errors)
- Spending more than 90 minutes on storyboard art quality — it should be rough sketches

---

### Pitfall 4: Prototype That Tries to Prove the Design Works

**Affects:** Day 4

**What it looks like:**
The Figma prototype has real product photography, polished typography, micro-animations, and 40 connected frames. It took 8 hours. You're proud of it. Users notice the craft and talk about aesthetics instead of the flow. Or they assume it's a real product and their feedback is about business model, not UX.

Alternatively: the prototype is too low-fidelity — grey boxes, placeholder text — and users spend the test session asking clarifying questions about what things are rather than trying to use them.

**Why it happens:**
"Realistic facade" is the sprint guidance, but designers instinctively push fidelity up. The sprint specifies enough fidelity to provoke realistic behavior, not enough to impress reviewers.

**Consequences (too high):**
- Build time blows the budget
- Users critique craft, not concept
- The critical UX question doesn't get answered

**Consequences (too low):**
- Users can't engage naturally
- Feedback is about confusion from placeholders, not about the actual design decisions

**Prevention:**

**The fidelity test:** Can a person who has never seen this product pick up the prototype, complete the primary task, and make real decisions along the way — without you explaining anything? If yes, it's ready. If no, it needs more. If they're admiring it instead of using it, it has too much.

**Scope constraints for this project's Day 4:**
- One flow only: Solo Mover, style discovery → A/B kit comparison → add to cart
- 8-12 connected frames maximum (Figma). Every frame beyond that is a scope decision, not a design decision.
- Real enough: use actual item images (not placeholder boxes), real pricing ($10-$50 range), readable labels
- Fake enough: lorem text in non-critical areas, placeholder avatars for personas, static loading states
- Do NOT build: the collaborative couple flow, the Pro spec export, the AR feature (document these as "not tested, future sprint")
- Do NOT connect: error states, empty states, off-path taps (let users get stuck — that is data)

**The AR temptation:** The mobile AR flow is the most visually impressive part of the concept and the most technically complex to fake. It will eat a disproportionate chunk of Day 4 if you let it. Prototype it as a static screen showing "what AR would look like" with a clear label. That is sufficient to ask "would you use this?"

---

## Moderate Pitfalls

Mistakes that reduce test quality and weaken the case study, but don't cause full restarts.

---

### Pitfall 5: Crazy 8s Performed as "Eight Versions of the Same Idea"

**Affects:** Day 2

**What it looks like:**
Eight panels, all exploring variations on the style quiz UI. Slightly different button placements. Same fundamental interaction model throughout. At the end, you pick the version with the cleanest layout and call it done.

**Why it happens:**
Crazy 8s has a time constraint (8 minutes, 1 minute per frame) that forces quantity. But without a team pushing different directions, the solo practitioner naturally converges. The technique's divergence pressure only works if you actively fight your instincts.

**Prevention:**
- Frame each panel as a different mental model, not a different layout. Panel 1: the quiz is a checklist. Panel 2: the quiz is a single big question. Panel 3: the quiz is a drag-ranking. Panel 4: there is no quiz — instead a gallery. Panel 5: AI asks you questions. Panel 6: the style profile is built passively from behavior.
- Use **How Might We notes from Day 1** as prompts for each panel — one HMW per frame forces variety.
- The rule: if two panels have the same core interaction, replace one.

**For this project specifically:** House2Home's style discovery mechanism is the highest-risk interaction in the product. Crazy 8s should explore radically different models for that one mechanism — not different visual treatments of the same model.

---

### Pitfall 6: Solution Sketch That Presents Rather Than Explains

**Affects:** Day 2

**What it looks like:**
A three-panel comic-style sketch that shows three screens of the chosen flow with UI drawn in the panels and a title at the top. Visually clean, conceptually opaque. A reviewer looks at it and sees "screens" but doesn't understand what's new, what the UX insight is, or why these three moments were chosen.

**Why it happens:**
The solution sketch format looks like a visual artifact (it is) so designers draw it visually. But the sprint purpose is to communicate your bet — the thing you believe is true about users that this design is testing.

**Prevention:**
- Panel 1: The user's situation before the key interaction (context, emotion, what they want)
- Panel 2: The moment of truth — the key interaction your design is betting on
- Panel 3: The outcome if the bet pays off (what success looks like for the user)
- Add annotation: one sentence per panel explaining the design decision, not describing what's drawn

**Label the bet explicitly:** "We believe users prefer to narrow style options through comparisons rather than open-ended input. This sketch tests that bet."

---

### Pitfall 7: Usability Test Leading Questions and Interview Script Problems

**Affects:** Day 5

**What it looks like:**
"Does this style quiz help you feel more confident?" (leading — presupposes it helps)
"Would you say this layout is intuitive?" (leading — "intuitive" is evaluative)
"What do you think of the kit comparison feature?" (priming — you've named the feature before they've noticed it)
"Did you notice the AR button?" (yes/no, confirms or denies your hypothesis instead of observing behavior)

Also: reading the task aloud in a way that describes the solution. "Please find the style quiz and use it to select a kit." — you've told them where to go and what it's for.

**Why it happens:**
Script-writing happens while you're still attached to the design. You want to know if it works. Questions naturally drift toward confirming it does.

**Prevention:**
**The cold read test:** Give your script to someone who has never seen the project. Can they understand the tasks? Do any questions feel like they're rooting for a particular answer? Any question they'd feel weird answering "no" to is leading.

**Task framing formula:** Describe the scenario without describing the solution.
- Wrong: "Use the style selector to find a kit for your apartment."
- Right: "You just moved into your first apartment and you want to make it feel like home. Start on this screen and show me what you'd do."

**For this project:** The five-act interview structure (welcome, context questions, prototype tour, task observation, debrief) is exactly right. The debrief is where you ask evaluative questions, not during the task observation.

**What to capture during tests:**
- Exact quotes, verbatim (not paraphrases)
- Where users pause, hesitate, backtrack — timestamp or note frame number
- What users say they expected vs. what they found
- Do NOT capture: your interpretations during the session (save that for debrief)

---

### Pitfall 8: Wrong Participants for the Primary Test Flow

**Affects:** Day 5

**What it looks like:**
You recruit from your list of 11 and end up with 3 participants who are interior designers (because they were enthusiastic and available) and 2 who have never moved. You test the Solo Mover flow. The feedback is expert-level critique of the style taxonomy, not behavior data from your actual persona.

**Why it happens:**
Convenience recruiting from a fixed list of 11 people means you take who's available. The list wasn't screened against the primary persona being tested.

**Consequences:**
- Interior designers will complete the task easily and complain the quiz is too simple (this is not the target user's experience)
- Non-movers have no stake in the outcome and their engagement is academic

**Prevention:**
Map your 11 participants against the primary flow being tested:

| Name | Relevant experience | Best for |
|------|---------------------|----------|
| Anna | (review Day 1 notes) | Solo Mover flow |
| Orion | — | — |
| Isa | — | — |
| ...etc | | |

Prioritize 4-5 people who match the Solo Mover persona for the primary test. Keep the Pro-persona participants for a secondary review round or case study validation, not the main test session.

**The minimum screen:** Participant should have moved to a new place (or be about to) AND not have a professional background in interior design. That is the target user's actual experience level.

---

## Minor Pitfalls

Mistakes that reduce polish or efficiency but are recoverable.

---

### Pitfall 9: Lightning Demos That Don't Feed Sketching

**Affects:** Day 2

**What it looks like:**
You research 6 competitors (Houzz, Homestyler, Planner 5D, Pinterest, Wayfair, IKEA), document what each does, and then open Crazy 8s and sketch ideas completely unconnected to the demos.

**Why it happens:**
Lightning demos and Crazy 8s feel like separate activities. In a team sprint they're causally linked because people present demos immediately before sketching. Solo, there's a gap.

**Prevention:**
Extract one "steal-worthy" element per demo before starting Crazy 8s. Write it on a sticky note or a note in your doc. Keep those 6 elements visible while sketching. At least two of your eight Crazy 8s frames should consciously remix a stolen element.

---

### Pitfall 10: Storyboard Missing the Failure Moment

**Affects:** Day 3

**What it looks like:**
The storyboard shows a clean happy path from arrival to purchase. Every step works. Users in testing get stuck in a place the storyboard never acknowledged as a risk.

**Why it happens:**
Storyboards are optimistic by instinct — you're building the thing you believe will work.

**Prevention:**
Add one panel that asks: "What is the most likely place this user abandons the flow?" Draw that moment. This becomes the primary thing you're watching for in usability testing. If the storyboard doesn't show a risk, you haven't identified your actual hypothesis.

---

### Pitfall 11: Case Study Written as a Process Log

**Affects:** Post-sprint

**What it looks like:**
"Day 1: I defined the problem. Day 2: I did Crazy 8s. Day 3: I built a storyboard. Day 4: I prototyped in Figma. Day 5: I ran tests. Here are the results."

A process log. A diary. A checklist completed.

**Why it happens:**
The sprint is chronological so the case study gets written chronologically. The writer describes what they did rather than what they learned, decided, and why.

**Why reviewers cringe:**
Case studies are evaluated on design thinking, not execution. The question reviewers are asking is: "Does this person understand why they made each decision and can they communicate that reasoning?" A process log answers "what did you do" not "why did it matter."

**Prevention:**
The case study narrative spine should be:
1. **Problem** — what was uncertain and what was at stake
2. **Bet** — what hypothesis the sprint was testing
3. **Evidence** — what the prototype and testing revealed
4. **Decision** — what would be built next and why, based on that evidence
5. **Learning** — what you'd do differently

Each sprint day becomes evidence for one of those five things, not a chapter in a diary.

**Specific cringe patterns for this project:**
- Listing all three personas without explaining why three were necessary and which one drove the prototype — looks like scope padding
- Showing polished Figma screens without showing the rough sketches they came from — looks like the "sprint" was just a design project with a fancy name
- Quoting 5 users without synthesizing what the quotes mean — looks like data collection without analysis
- Not mentioning what was cut and why — a sprint that tests everything is a sprint that tested nothing

---

### Pitfall 12: Notes During Testing That Are Too High-Level

**Affects:** Day 5

**What it looks like:**
"User 3 had trouble with the style quiz." That is the entire note. Usable? Barely. Actionable? No.

**Prevention:**
Use a structured note template per participant:

```
Participant: [name]
Task 1:
  - Behavior observed: [exact action sequence]
  - Quote: "[verbatim]"
  - Point of hesitation: [frame/screen, what they did]
  - What they expected: [if stated]
Task 2: ...
Overall:
  - What worked: [1-2 things]
  - What didn't: [1-2 things with evidence]
  - Most useful quote: "[verbatim]"
```

Note-taking and facilitating simultaneously is hard solo. Consider: record the session (with permission) and take sparse live notes, then fill the template from the recording immediately after. Do not wait until all five sessions are complete — memory degrades fast.

---

## Scope Risk Register: Three Personas + Two Platforms

This is a concentrated summary of where the expanded scope creates compounding risk across days.

| Day | Activity | Scope risk | Mitigation |
|-----|----------|------------|------------|
| Day 2 | Lightning Demos | Research 3 persona contexts = 3x time | Cap at 2 demos per persona type; use existing competitor notes from Day 1 |
| Day 2 | Crazy 8s | Unclear which persona to sketch for | Declare a target persona before the timer starts. Repeat for each persona only if time permits. |
| Day 2 | Solution Sketch | Temptation to create 3 solution sketches | One sketch. Primary persona. Primary platform. |
| Day 3 | Storyboard | Three separate storyboards = 15+ hours | One primary storyboard (8-10 panels, Solo Mover). Annotated variants for Couple/Pro as a companion doc, not a full storyboard. |
| Day 4 | Prototype | All three flows + AR = unbuildable in 1 day | One flow. 8-12 frames. AR is one static screen, clearly labeled as concept. |
| Day 5 | Testing | Testing three flows requires 15 participants | Test one flow with 5 participants. Document other flows as "future sprint" in case study. |
| Case Study | Writing | Three personas = no clear story | The story is about the system design decision, not three separate stories. Lead with the Solo Mover test; position other personas as scope framing. |

**The meta-rule:** The expanded scope lives in the case study's framing and the Day 1 documentation. It does not live in the prototype or the test plan. Scope expansion earns its keep by showing system-level thinking in the case study — not by multiplying prototype surfaces.

---

## Phase-Specific Warnings Summary

| Phase | Specific Warning | Mitigation |
|-------|-----------------|------------|
| Day 2 Crazy 8s | All 8 frames explore same interaction model | Force one different mental model per frame |
| Day 2 Solution Sketch | Sketch shows screens, not decisions | Label each panel with the UX bet it represents |
| Day 3 Storyboard | Too many panels (15+), reads as wireframes | Cap at 10 panels; each panel = decision moment, not screen state |
| Day 3 Storyboard | No failure moment included | Add one "where users abandon" panel explicitly |
| Day 4 Prototype | Fidelity too high, builds too long | 8-12 Figma frames maximum; AR = one static concept screen |
| Day 4 Prototype | Builds Couple and Pro flows | Declare out of scope before starting; document in case study |
| Day 5 Testing | Leading questions in script | Cold-read test: would it feel weird to answer "no"? |
| Day 5 Testing | Wrong participants recruited | Map 11 participants against Solo Mover criteria before scheduling |
| Day 5 Testing | Notes too vague to use | Use structured template per participant; record sessions |
| Case Study | Process log format | Narrative spine: Problem → Bet → Evidence → Decision → Learning |
| Case Study | Three-persona scope appears padded | Explain why three, which drove the prototype, what each persona validated |

---

## Sources

**Confidence levels:**

- GV sprint methodology (Crazy 8s, solution sketch, storyboard, five-act interview, Heat Map): HIGH — sourced from Knapp, Zeratsky, Kowitz "Sprint" (2016), GV design sprint official materials, and Jake Knapp's sprint.weekdone.com documentation
- Solo sprint echo chamber and confirmation bias patterns: HIGH — established cognitive bias literature; sprint team structure as bias mitigation is documented in the GV methodology rationale
- Usability testing leading question patterns: HIGH — Nielsen Norman Group usability testing guidelines, Steve Krug "Rocket Surgery Made Easy" (2010)
- Case study writing patterns (process log vs. narrative): MEDIUM — synthesized from UX portfolio review community standards (ADPList, UX Collective), Springboard and General Assembly portfolio guidance; no single authoritative source
- Scope hydra specific to this project: MEDIUM — inferred from project context; specific risk pattern well-supported by GV sprint narrowing methodology but project-specific application is analyst judgment
- Participant recruiting screen for this project: MEDIUM — general usability testing recruiting guidelines are HIGH confidence; specific participant mapping to this project's 11 names is LOW confidence (Day 1 notes not available to this researcher)
