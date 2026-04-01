# Technology Stack — Tools & Approaches

**Project:** House2Home Design Sprint (Days 2–5)
**Researched:** 2026-04-01
**Confidence note:** WebSearch unavailable. All findings drawn from training data (knowledge cutoff August 2025) and direct knowledge of GV sprint methodology, Figma, Marvel, and UX testing standards. Confidence levels reflect that basis.

---

## Overview

This sprint is a **solo, school-assignment GV design sprint** with an expanded scope: 3 personas (Solo Mover, Couple/Roommates, Architect/Interior Designer) and 2 platforms (desktop web + mobile AR). The prototype fidelity target is "realistic facade" — enough to test the primary task flow, not pixel-perfect. Figma is already in the course curriculum and strongly preferred per project constraints.

---

## Day 2 — Sketching (Crazy 8s + Solution Sketch)

### Recommended Approach

**Use paper + pen or iPad (Procreate/Notability) for Crazy 8s. Use paper for the solution sketch first draft, then optionally digitize.**

| Tool | Role | Why |
|------|------|-----|
| Paper + pen (A4 folded to 8 panels) | Crazy 8s sketching | Speed is the point. No UI overhead. Forces commitment in 1 minute per panel. |
| iPad + Procreate or Notability | Crazy 8s if you prefer digital | Layers make it easy to export; Apple Pencil keeps sketch speed high. Acceptable substitute. |
| Paper or whiteboard | Solution sketch (3-panel) | Thinking on paper is faster than any tool; convert to digital after committing to the idea. |
| Figma (optional) | Digitize final solution sketch only | Only useful AFTER the idea is committed — not during ideation. |

**Do NOT use Figma or any wireframe tool during Crazy 8s.** The tool friction defeats the purpose. The constraint is 8 ideas in 8 minutes; UI software slows that to 8 ideas in 80 minutes.

### Solo Crazy 8s Protocol

The GV sprint was designed for teams. Running it solo requires deliberate structure to compensate for the lack of divergence pressure from teammates.

**Recommended sequence:**

1. **Set a physical timer** — 1 minute per panel, no extensions. Treat it like an exam.
2. **Run 3 rounds, not 1** — Round 1: obvious ideas (get them out). Round 2: variations on your best Round 1 idea. Round 3: push one constraint — what if it were invisible / instant / the opposite?
3. **Sketch from your flow maps** — You have 4 user flow maps from Day 1. For each Crazy 8s session, pick one critical moment from one flow (e.g., "the style discovery branch" or "the A/B kit comparison"). Focused scope produces usable sketches; open-ended prompts produce chaos.
4. **Do one session per critical screen type**, not per persona — since the platform is role-based on a shared foundation, most screens are shared. Identify the 2–3 screens that differ meaningfully by persona (e.g., the Pro's "Build Proposals" screen vs. the consumer's "Customize Pack") and run separate sessions only for those.
5. **Decide before sketching** — write a 1-sentence "this is the moment I'm sketching" on a Post-it before starting the timer. Without this, 8 minutes produces 8 variations on the same idea.

### Solution Sketch (3-Panel)

The solution sketch is your clearest, most considered idea from Crazy 8s. For a solo practitioner, this is also your "vote."

**Structure:**
- Panel 1: Entry state (what the user sees before the critical moment)
- Panel 2: The critical interaction (the thing you're testing)
- Panel 3: Resolution / next step (what success looks like immediately after)

**Given your scope, prioritize these critical moments:**
1. **Style Finder → Branch decision** (all personas) — this is where confidence either forms or breaks
2. **A/B Kit Comparison × 3** (Solo + Couple) — the primary decision mechanism
3. **Pro: Build Proposals → Client Share** (Pro persona) — the handoff moment that defines Pro value
4. **AR entry point** ("Test in Your Space" trigger) — justifies the mobile platform

You do not need a solution sketch for every persona. Sketch the flow with the most complexity or risk first; simpler persona variants are refinements, not new sketches.

**Confidence: HIGH** — GV sprint sketching methodology is well-documented and not tool-dependent.

---

## Day 3 — Storyboarding (Wireframe Storyboard)

### Recommended Approach

**Use Figma for the storyboard. Build it as a series of low-fidelity wireframe frames in a single page.**

| Tool | Role | Why |
|------|------|-----|
| Figma | Primary storyboard tool | Directly reusable as prototype scaffolding on Day 4. Draw the storyboard in Figma and your Day 4 work is already started. |
| Paper storyboard | Pre-Figma draft only | Fast to sequence, slow to revise. Acceptable for rough panel order before going digital. |
| Miro or FigJam | Avoid for storyboard | Good for collaborative mapping, but you're solo and the output is not directly portable to a prototype. Extra work with no payoff. |

### Storyboard Best Practices

**Target: 8–12 panels per primary flow.** 5 is too sparse to test; 15+ is prototype territory (you're not there yet).

**Panel content:**
- Each panel = one user decision or one visible state change
- Include brief captions (1 sentence) — these become your usability test task prompts on Day 5
- Show the screen AND a minimal context note (e.g., "Solo Mover. Just finished Style Finder. Sees 2 kit options.")

**For your scope specifically:**

Given 3 personas and 2 platforms, you do not need 4 full storyboards. You need:

1. **Primary storyboard** — Solo Mover, desktop, full flow from landing to order confirmation. This is your "spine" — all other flows branch from it. (10–12 panels)
2. **Couple variant panels** — only the panels that differ from Solo: the individual style finders, the side-by-side comparison, the blended style confirm, the shared A/B. (~4–5 panels branching from the spine)
3. **Pro variant panels** — Pro account entry, "Build Proposals," client share, client AR annotation feedback, finalize. (~5–6 panels)
4. **AR flow panels** — entry point, scan, AR overlay, interact, exit. (~4–5 panels, shown as a sidebar to the main flow)

**Total: approximately 25–28 panels across 4 flows, but shared panels are not duplicated.** This is manageable in a day.

**What to include in wireframe fidelity:**
- Correct layout zones (header, main content, sidebar, CTA position)
- Real labels on buttons (not "Button" — write "Find My Style" or "Compare Kits")
- Placeholder boxes for product images (labeled "Kit A Image")
- No colors, no type hierarchy, no icons — save that for Day 4

**Confidence: HIGH** — storyboard practice is stable; Figma as the tool is a curriculum requirement and practically standard.

---

## Day 4 — Prototyping

### Recommended Tool: Figma

**Use Figma exclusively. Do not use Marvel, Framer, or any other tool.**

| Tool | Verdict | Reason |
|------|---------|--------|
| Figma | **Use this** | Curriculum requirement. Best-in-class for interactive prototyping at sprint fidelity. Auto Layout handles responsive-ish layouts without engineering. Prototyping tab connects frames directly; no separate export step. Sharing via link works for remote testing. |
| Marvel | Avoid | Adds a tool-switch cost. Figma does everything Marvel does and more. Marvel's primary use case (uploading static images and adding hotspots) is genuinely faster than Figma for very rough click-through prototypes — but you're already building in Figma from Day 3, so there's no advantage. |
| Framer | Avoid for this sprint | Framer is excellent for high-fidelity, code-based prototypes. It is significantly more complex to set up and has a steeper learning curve. For a "realistic facade" sprint prototype, this complexity buys nothing. |
| InVision | Avoid — largely deprecated | InVision's core prototyping product has been sunset. Do not invest time here. |
| Adobe XD | Avoid | Adobe XD is in maintenance mode as of 2023. No active development. Not worth learning or using for new work. |

### Figma Prototype Strategy

**The goal is a clickable flow, not a full application.** Test the critical path, not every screen.

**Setup:**

1. **Build on your Day 3 storyboard frames** — add visual design (color, type, product imagery) directly on top of the wireframes. Do not recreate from scratch.
2. **Use Figma Components for repeated elements** — the kit card (used in A/B comparison) appears multiple times. Make it a component with variants for "selected" vs "unselected." This saves significant time.
3. **Use Auto Layout on containers** — particularly for the item list inside a kit. Auto Layout lets you add/remove items without manually repositioning everything.
4. **Use real-ish content, not Lorem Ipsum** — product names, prices ($14.99, $22.50), and style names ("Modern," "Bohemian Eclectic") make the prototype feel testable. Users should be able to make real-seeming decisions. Placeholder text breaks the illusion during testing.

**Prototype connections (Figma's Prototype tab):**

Wire these minimum paths:
- Style Finder completion → Branch choice visible
- A/B comparison panel 1 → selecting A or B → panel 2 → panel 3 → Kit Selected
- "Customize Pack" → item swap interaction (can be a modal overlay with 2–3 real options)
- "Test in Your Space" → shows an AR preview mockup frame (static image of AR is fine — you don't need real AR)
- Pro: "Share with Client" → client review view

**What to fake:**
- AR: a static image showing kit items placed over a photo of a living room is sufficient. Users understand "this represents what AR would show."
- Product catalog: 6 real-looking product items with names and prices is enough. You do not need 50 items.
- Payment/checkout: a single checkout summary frame with a "Place Order" button. Do not prototype the full payment form.

**Fidelity target:**
- Desktop: medium fidelity — correct layout, real labels, brand colors, product images (use free stock from Unsplash)
- Mobile AR: low-medium fidelity — show the AR state as a static overlay on a real room photo; interactive elements are limited to move/rotate mockups

**Confidence: HIGH** — Figma's capabilities for sprint-level prototyping are extremely well established, curriculum-aligned, and actively maintained as of 2025.

---

## Day 5 — User Testing (Five-Act Interview)

### Recommended Approach

**Use Figma's share link for prototype access. Conduct interviews via video call (Zoom or Google Meet) or in person. Record with explicit permission. Use a simple paper debrief grid.**

| Tool | Role | Why |
|------|------|-----|
| Figma share link | Prototype delivery | One URL, no installation, works on any browser. Give participants "can view" access only — prevents accidental editing. |
| Zoom or Google Meet | Remote sessions | Both support screen share (participant shares their screen so you see their interactions). Both record. Pick whichever your participants already have. |
| In-person | Best option if available | You can observe body language, hesitation, and physical pointing. Reduces technical friction. |
| Lookback.io or Maze | Avoid for this sprint | These are unmoderated testing platforms. The Five-Act Interview is explicitly moderated — facilitator-participant dialogue is the method. Unmoderated tools remove the acts that make the Five-Act work. |
| Notion or Google Docs | Note-taking during session | Keep a simple observation grid open in a second window. Do not try to take verbatim notes — write keywords and behavior observations only. |

### Five-Act Interview Structure

The GV Five-Act Interview has a specific structure. Running it correctly matters for valid findings.

**Act 1 — Friendly Welcome (5 min)**
- Put the participant at ease. Explain this is a test of the prototype, not a test of them.
- Say explicitly: "There are no wrong answers. If something is confusing, that's useful information for us."
- Get consent to record. Explain the recording is for your notes only, not published.
- Key line: "We built this, so we may have made mistakes. Your honest reaction helps us find them."

**Act 2 — Background Questions (10 min)**
- Ask about their relevant experience, not about the product.
- For House2Home: "Tell me about the last time you moved or decorated a space. What was that process like?" "How do you typically shop for home items?" "Have you ever felt stuck trying to make decorating decisions?"
- This establishes their mental model before you show them anything.
- **Do not ask leading questions.** "Have you ever found it hard to decorate?" is leading. "Tell me about your experience decorating" is open.

**Act 3 — Context Scenarios (tasks) (20–25 min)**
- Give scenarios, not instructions. "Imagine you just moved into a new apartment. You want to make the living room feel like yours. Use this to see if it helps." Not: "Click on Style Finder and then choose a kit."
- Watch where they look first. Hesitation and backtracking are data.
- Ask "think aloud" prompts: "What are you thinking right now?" "What did you expect to happen?" "What would you do from here?"
- For your scope, test these scenarios in order:
  1. **Solo Mover task** — find and select a starter kit for a living room
  2. **Couple variant** (if participant is willing, run as a role-play or use a second test session with an actual pair) — "Imagine you're picking a kit with your partner. They're on their way. What would you do first?"
  3. **AR preview** — "You've selected a kit. Before buying, you want to see what it looks like in your space."
- You do not need to test the Pro flow with all 5 participants. Test it with 1–2 who have relevant background (design, procurement, client-facing work).

**Act 4 — Debrief (10 min)**
- Ask retrospective questions after the tasks, not during.
- "Which part felt most natural?" "Where did you feel uncertain?" "Is there anything you expected to see that wasn't there?"
- "If you could change one thing, what would it be?"
- Do not defend design decisions during this act. Listen.

**Act 5 — Wrap-Up (5 min)**
- Thank them. Confirm the recording will not be shared publicly.
- Ask if they have any questions for you.
- Optional: "Would you be willing to be contacted for follow-up if we have questions?"

### Participant Recruitment (from Day 1)

You have 11 identified potential participants: Anna, Orion, Isa, Eli, Nathaniel, Ray, Sadie, Mary, Craig, Seth, Birdie. You need exactly 5. Prioritize:

- At least 2 who have recently moved or will move soon (Solo Mover validation)
- At least 1 who shares living space with a partner or roommate (Couple flow validation)
- At least 1 with design/procurement background for Pro flow validation (Craig or Seth if applicable)
- Screen for: comfortable browsing on a desktop, willing to share screen on video call

**Session length:** Schedule 60 minutes per participant. The interview runs 45–50 minutes; buffer for setup and late starts.

### Debrief Method

After all 5 sessions, use an observation grid (paper or spreadsheet) to find patterns:

| Observation | P1 | P2 | P3 | P4 | P5 | Pattern? |
|-------------|----|----|----|----|----|----|
| [behavior or quote] | Y/N | Y/N | ... | ... | ... | 3+/5 = pattern |

Surface findings in three buckets:
1. **Works well** — behaviors showing confidence, task completion, positive reactions
2. **Needs iteration** — moments of hesitation, confusion, wrong paths
3. **Critical failures** — task abandonment, complete misunderstanding of the interaction

If 3 of 5 participants share a behavior, treat it as a finding. If only 1 does, note it but do not generalize.

**Confidence: HIGH** — Five-Act Interview methodology is directly from the GV sprint playbook (Sprint, Knapp/Zeratsky/Kowitz, 2016) and widely validated.

---

## Alternatives Considered

| Category | Recommended | Alternatives | Why Not |
|----------|-------------|--------------|---------|
| Prototyping | Figma | Marvel, Framer, InVision | Marvel: no advantage over Figma when already in Figma. Framer: over-engineered for sprint fidelity. InVision: deprecated. |
| Sketching | Paper + pen | Figma, Balsamiq, Whimsical | All digital tools add friction that defeats the speed purpose of Crazy 8s. |
| Storyboarding | Figma | Miro, FigJam, paper | Miro/FigJam output is not directly portable to prototype. Paper not reusable as Day 4 scaffolding. |
| Remote testing | Zoom + Figma link | Lookback, Maze, UserTesting.com | Unmoderated tools are wrong method for Five-Act Interview. UserTesting.com has cost and setup overhead unnecessary for a 5-person study. |
| Note-taking | Simple grid (paper/Notion) | Dedicated UX research tools (Dovetail, Airtable) | Dovetail/Airtable are analysis tools for large-scale studies. Overkill for 5 sessions. The simplest grid you'll actually use is better than a sophisticated one you set up but don't finish. |

---

## Sources

- Sprint (Knapp, Zeratsky, Kowitz — GV, 2016): canonical Five-Act Interview, Crazy 8s, and solution sketch methodology
- Figma documentation (2025): Auto Layout, components, prototyping connections — current product
- GV Sprint resources at sprintbook.com: updated sprint facilitation guides including solo adaptations
- Training knowledge (August 2025 cutoff): Marvel deprecation trajectory, Adobe XD maintenance mode, InVision sunset status
- Note: WebSearch was unavailable during this research session. Tool comparison claims (particularly InVision sunset, Adobe XD maintenance mode) should be spot-checked if currency is critical.
