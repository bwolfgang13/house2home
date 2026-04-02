---
phase: 01-day-2-sketch
plan: "01"
subsystem: ux-research
tags: [lightning-demos, hmw-notes, competitive-analysis, design-sprint, house2home]

# Dependency graph
requires:
  - phase: day-1-complete
    provides: "Problem statements, 3 personas, 4 user flow maps, A/B kit comparison × 3 mechanism, Solo Mover desktop as prototype spine"
provides:
  - "8 HMW notes framed around A/B kit comparison, ready as Crazy 8s prompts"
  - "10 lightning demo entries across 4 categories (Consumer, Collaborative, Professional, AR) with structured 3-field mechanism notes"
  - "Lightning Demo Summary identifying cross-category patterns, strongest borrowable mechanism, and competitive gap"
  - "Critical Screen Decision committing A/B Kit Comparison as primary with written rationale"
  - "Sprint doc Day 2/Design Sprint Notes Day 2.md structured and ready for Crazy 8s"
affects: [01-02, 01-03, storyboard, prototype]

# Tech tracking
tech-stack:
  added: []
  patterns:
    - "3-field lightning demo format: What it does well / What's missing / Mechanism to borrow"
    - "HMW notes derived from Day 1 problem statements, not generated from blank paper"

key-files:
  created:
    - "Day 2/Design Sprint Notes Day 2.md"
  modified: []

key-decisions:
  - "A/B Kit Comparison named as primary critical screen — confirmed by lightning demos showing this is the universal breakdown point across all 10 competitors"
  - "Style Selector named as secondary critical screen — more borrowable patterns exist, so primary design bet goes to A/B comparison"
  - "Havenly binary thumbs + rejection micro-feedback identified as strongest borrowable mechanism for House2Home"
  - "House2Home's forced A/B × 3 structure identified as genuinely novel — no competitor presents two complete styled kit options side-by-side for binary decision"

patterns-established:
  - "Lightning demo analysis: mechanisms over impressions — each entry names a concrete UI behavior, not an adjective"
  - "Critical screen decision documented in writing BEFORE Crazy 8s begins — locks the sprint direction"

requirements-completed: [SKTCH-01, SKTCH-02, SKTCH-03]

# Metrics
duration: multi-session (Task 1 prior session, Task 2 research agents)
completed: 2026-04-01
---

# Phase 01 Plan 01: Prep, Lightning Demos, and Critical Screen Decision Summary

**10 lightning demos across Consumer, Collaborative, Professional, and AR categories revealed A/B Kit Comparison as an unsolved problem in every competitive product — establishing it as the primary critical screen with no direct mechanism to borrow, only patterns to adapt**

## Performance

- **Duration:** Multi-session (Task 1 completed prior session; Task 2 completed via research agents)
- **Started:** 2026-04-01
- **Completed:** 2026-04-01
- **Tasks:** 2
- **Files modified:** 1

## Accomplishments

- Created Day 2 sprint doc with 2-sentence context recap linking Day 1 outcomes to Day 2's design question
- Extracted 8 HMW notes from Day 1 problem statements, each targeting a distinct angle on choice paralysis during A/B kit comparison
- Documented 10 lightning demos with structured 3-field notes: Consumer tools (Houzz, Homestyler, Planner 5D, Pinterest), Collaborative (Miro), Professional (Houzz Pro, Modsy [defunct/archived], Havenly), AR (IKEA Place, Wayfair AR)
- Identified Havenly's binary thumbs + rejection micro-feedback as strongest borrowable mechanism for House2Home's comparison rounds
- Documented critical finding: no competitor presents two complete styled kit options side-by-side for a single binary decision — House2Home's A/B × 3 structure is novel
- Committed Critical Screen Decision (A/B Kit Comparison primary, Style Selector secondary) with written rationale before any Crazy 8s work

## Task Commits

Each task was committed atomically:

1. **Task 1: Prep — Extract HMW Notes, Confirm Materials, Create Sprint Doc** - `ee9052d` (feat)
2. **Task 2: Lightning Demos — Research 10 Products and Document Critical Screen Decision** - `402b3e7` (feat)

## Files Created/Modified

- `Day 2/Design Sprint Notes Day 2.md` - Sprint doc with Context, 8 HMW Notes, 10 Lightning Demo entries, Lightning Demo Summary, and Critical Screen Decision

## Decisions Made

- **Primary critical screen: A/B Kit Comparison.** Lightning demos confirmed that the decision-to-purchase breakdown is universal across all 10 products. Because no competitor has solved it, there is no mechanism to borrow directly — it must be designed from scratch. This is the highest-stakes UX bet.
- **Secondary critical screen: Style Selector.** The failure modes of style discovery are well-documented (Homestyler AI generation, Pinterest Taste Graph) and borrow-ready. The Style Selector enters the sprint as the second Crazy 8s round, not the first.
- **Modsy documented as defunct (closed June 2022)** using archived sources (TechCrunch, Business of Home, Decorilla retrospectives). Entry focuses on the Live Swap mechanism and its failure to create feedback loops.
- **Havenly's thumbs + micro-feedback identified as the mechanism to extend**, not just copy — applied to final-round kit bundle approval with rejection reason capture (price / color / style / size) rather than line-item rejection.

## Deviations from Plan

None — plan executed exactly as written. Both tasks completed per specified format and structure.

## Issues Encountered

None. Modsy's defunct status was anticipated in the plan and handled per the specified instruction (use archived sources, note limitation in sprint doc).

## User Setup Required

None — no external service configuration required.

## Next Phase Readiness

- Sprint doc `Day 2/Design Sprint Notes Day 2.md` is structured and ready for Crazy 8s sections to be added
- 8 HMW notes are numbered and ready to serve as Crazy 8s panel prompts (Plan 01-02, Round 1 and Round 2)
- Critical screen decision is committed in writing: A/B Kit Comparison = Round 1; Style Selector = Round 2
- Strongest mechanism to adapt: Havenly binary thumbs + rejection micro-feedback
- Key insight for sketching: the side-by-side simultaneous comparison view (Planner 5D borrow) combined with single binary decision (Havenly borrow) is the core interaction model to explore in Crazy 8s
- No blockers for Plan 01-02

---
*Phase: 01-day-2-sketch*
*Completed: 2026-04-01*
