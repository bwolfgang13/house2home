---
phase: 1
slug: day-2-sketch
status: draft
nyquist_compliant: false
wave_0_complete: false
created: 2026-04-01
---

# Phase 1 — Validation Strategy

> Per-phase validation contract for feedback sampling during execution.
> **Note:** This phase produces no code — all outputs are design artifacts (paper sketches, markdown doc, photographs). Automated testing is not applicable. Manual artifact review is the validation mechanism.

---

## Test Infrastructure

| Property | Value |
|----------|-------|
| **Framework** | Manual artifact review (no automated test framework) |
| **Config file** | None — design sprint phase |
| **Quick check command** | Human review of sprint doc sections against SKTCH acceptance criteria |
| **Full suite command** | Complete review of all 7 SKTCH requirements against acceptance criteria |
| **Estimated runtime** | ~5 minutes |

---

## Sampling Rate

- **After every task:** Review sprint doc section against acceptance criteria for that task
- **After every plan wave:** Full checklist review against all SKTCH requirements for that wave
- **Before `/gsd:verify-work`:** All 7 SKTCH requirements must be met
- **Max feedback latency:** Immediate — review happens as soon as each artifact is created

---

## Per-Task Verification Map

| Task ID | Plan | Wave | Requirement | Test Type | Verification Method | Status |
|---------|------|------|-------------|-----------|---------------------|--------|
| 1-01-W0 | 01 | 0 | SKTCH-01 | Manual | HMW notes derived from Day 1 content; 8 notes documented before Crazy 8s | ⬜ pending |
| 1-01-01 | 01 | 1 | SKTCH-01 | Manual | Sprint doc has 4+ product entries, at least 1 is a collaborative tool category | ⬜ pending |
| 1-01-02 | 01 | 1 | SKTCH-02 | Manual | Each product entry has all 3 fields (what / missing / borrow) with concrete content | ⬜ pending |
| 1-01-03 | 01 | 1 | SKTCH-03 | Manual | Sprint doc has "Critical Screen Decision" section with rationale before Crazy 8s section | ⬜ pending |
| 1-01-04 | 01 | 2 | SKTCH-04 | Manual | Crazy 8s photo reviewed: panels show distinct decision mechanics, not layout variations | ⬜ pending |
| 1-01-05 | 01 | 2 | SKTCH-05 | Manual | Sprint doc has second Crazy 8s section with photo for secondary screen | ⬜ pending |
| 1-01-06 | 01 | 3 | SKTCH-06 | Manual | Photo exists; each panel has title + description; at least 1 annotation per panel explains WHY | ⬜ pending |
| 1-01-07 | 01 | 3 | SKTCH-07 | Manual | Sprint doc contains all sections; photos embedded; reflection section present | ⬜ pending |

*Status: ⬜ pending · ✅ green · ❌ red · ⚠️ incomplete*

---

## Wave 0 Requirements

- [ ] Derive/extract HMW notes from Day 1 content — 8 notes needed as Crazy 8s panel prompts before Round 1 begins
- [ ] Confirm Modsy substitution decision (archived research vs. live alternative: Decorilla or Spacejoy)
- [ ] Physical materials check: A4 paper, black pen, phone for photography

---

## Manual-Only Verifications

| Behavior | Requirement | Why Manual | Test Instructions |
|----------|-------------|------------|-------------------|
| Lightning demos include 1 collaborative tool | SKTCH-01 | Physical/digital research task | Count entries; verify at least 1 is Miro/FigJam category |
| Mechanism notes are specific, not impressionistic | SKTCH-02 | Requires judgment on content quality | Each product: does "borrow" field name a concrete UI mechanism? |
| Critical screen named before Crazy 8s | SKTCH-03 | Document ordering / timing | Sprint doc section order: Critical Screen before Crazy 8s |
| Crazy 8s panels are distinct interaction models | SKTCH-04 | Visual/conceptual judgment | Review photo: do 8 panels show different decision mechanics? |
| Second Crazy 8s round completed | SKTCH-05 | Physical sketching task | Photo of second round exists in sprint doc |
| Solution sketch tells before/during/after story | SKTCH-06 | Narrative judgment | Can a reader understand the flow without verbal explanation? |
| All work documented with reflection | SKTCH-07 | Documentation completeness | All sections present, photos embedded, reflection written |

---

## Validation Sign-Off

- [ ] All tasks have manual verification criteria defined
- [ ] Wave 0 prerequisites confirmed before sketching begins
- [ ] No tasks skipped — all 7 SKTCH requirements addressed
- [ ] Physical artifacts photographed and embedded in sprint doc
- [ ] `nyquist_compliant: true` set in frontmatter

**Approval:** pending
