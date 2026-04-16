# Design Sprint -- Day 2 Notes
## House2Home | Sketch Day

## Context

Day 1 defined the core problem (users lack confidence decorating independently), scoped the sprint to 3 personas (Solo Mover, Couple/Roommates, Architect/Interior Designer), and mapped 4 user flows across desktop web and mobile AR. The critical design mechanism emerging from Day 1 is A/B kit comparison × 3 — a structured elimination that narrows 6 kit options to 1 through three binary decisions — with Solo Mover desktop as the prototype spine. Day 2 addresses the open question that mechanic leaves: how do we design the comparison moment itself so the user feels confident they chose their kit, not that they were guided to one?

## HMW Notes (Crazy 8s Prompts)

1. HMW make each comparison feel like the final one? *(from the A/B × 3 structure — each round must carry decisive weight, not feel like a preliminary filter)*
2. HMW make the user feel like an expert during the comparison? *(from Solo Mover problem statement — user lacks confidence; the mechanic itself should confer it)*
3. HMW let the kits explain themselves rather than requiring a read? *(from "overwhelmed by blank canvas" — reduce evaluation burden; the UI does the comparison work)*
4. HMW make "not choosing" feel like progress, not failure? *(from A/B elimination structure — each round removes options, which should feel like narrowing toward something, not giving something up)*
5. HMW create a sense of momentum through the 3-round structure? *(from A/B × 3 mechanism — 3 rounds can feel like a journey with a destination, not a chore)*
6. HMW show the user what they're moving toward, not just away from? *(from "no clear direction" in Solo Mover before-state — elimination needs a positive pole, not just subtraction)*
7. HMW make the chosen kit feel inevitable in retrospect? *(from "purchase decisions confidently" in problem statement — the emotional goal is that after-state clarity, not just completion)*
8. HMW reduce the fear of choosing wrong? *(from "balancing quality, quantity, and budget" in Solo Mover problem — the fear of a bad call is the primary paralysis driver)*

## Lightning Demos

### Houzz -- Consumer Tool
**What it does well:** One-click heart/save icon that captures inspiration photos directly into titled ideabooks without leaving the browsing context. Users save images to categorized collections without friction while scrolling through 25+ million curated design photos, maintaining discovery momentum.
**What's missing:** No bridge between inspiration and purchase. Users save dozens of photos into ideabooks but the flow breaks at translation — there's no mechanism to link saved inspiration directly to purchasable products, and ideabook navigation is hidden from product pages, forcing repeated context-switching.
**Mechanism to borrow:** Frictionless save-without-interruption. Allow users to flag/save kit comparison outcomes with a single gesture while keeping the comparison interface in focus — no modal, no navigation away.

### Homestyler -- Consumer Tool
**What it does well:** AI room styling generates 5–8 photorealistic design options (modern, classic, minimal, bohemian) in ~30 seconds from a single room photo. Users skip blank-canvas paralysis by seeing auto-populated furniture combos and color palettes in 3D before any manual customization.
**What's missing:** Engagement drops after auto-generation. 30–45 second load times per furniture item make refinement tedious. No mechanism to compare two full room designs side-by-side. Recent paywalling of colors, styles, and furniture has choked the refinement loop entirely.
**Mechanism to borrow:** Rapid AI-generated comparison snapshots. Generate 3 distinct kit variations automatically upfront — show them as thumbnail "snapshots" before committing to deep customization. Reduces upfront choice paralysis rather than creating a new bottleneck in refinement.

### Planner 5D -- Consumer Tool
**What it does well:** Drag-and-drop furniture placement in 2D/3D with real-time visual feedback and grid-line snapping. Users can swap furniture items instantly, see spatial relationships in 3D, and save multiple layout versions. Supports rapid iteration without CAD knowledge.
**What's missing:** Product selection is the decision bottleneck. With 8,000+ catalog items and no comparison mechanism, users drag in one item, see it, undo, drag in another. No "which of these two works better?" flow — only unlimited tweaking with no decision closure or exit ramp toward commitment.
**Mechanism to borrow:** Side-by-side layout comparison. Show two kit variations simultaneously (Kit A left, Kit B right in same room context) rather than sequential swapping, so users evaluate trade-offs directly rather than relying on memory.

### Pinterest -- Consumer Tool
**What it does well:** Related Pins algorithm uses multimodal embeddings and a "Taste Graph" to show semantically similar content adjacent to any viewed pin. As users save to boards, the platform infers style preferences and tightens recommendations in real-time — a self-reinforcing discovery loop that adapts without explicit input.
**What's missing:** Style synthesis never happens. Users accumulate 30+ pins across multiple boards ("Farmhouse," "Modern," "Eclectic") with no dominant aesthetic emerging. No mechanism to compare boards, surface style conflicts, or synthesize taste into a decision. The jump from "liked 100 pins" to "I'm buying this sofa in this finish" is unscaffolded.
**Mechanism to borrow:** Adaptive recommendations from implicit preference signals. Track which kit variations users linger on or re-view during comparison rounds, and use those signals to surface similar kits in the next round — so the app learns and narrows iteratively rather than asking users to articulate style upfront.

### Miro -- Collaborative Tool
**What it does well:** Dot voting uses anonymous parallel vote-casting with a fixed vote pool per participant. Votes aggregate into a ranked leaderboard. Results remain hidden until voting closes, then reveal with a "See all results" option. The hidden-until-reveal mechanic prevents social anchoring — the second voter can't see the first voter's choice, so minority preferences surface without pressure.
**What's missing:** Requires all participants present in a live 99-minute window — no asynchronous preference capture. Provides no style profiling before voting and no product comparison context within the voting interface. Results show counts but no reasoning or trade-off explanation.
**Mechanism to borrow:** Anonymous parallel voting with fixed vote pools and hidden-until-reveal results. In House2Home's couple/roommate flow, distribute preference credits across comparison rounds, reveal winner only after both parties vote. Prevents the second person anchoring on the first.

### Houzz Pro -- Professional Tool
**What it does well:** Approval-by-line-item mechanic lets clients accept or reject individual products within a proposal using checkmarks and X buttons, with undo support. The system auto-recalculates payment schedules based on approvals. Professionals receive immediate email notification of client decisions. Proposal visibility (pricing, specs) is customizable per client.
**What's missing:** Line-item approval flow doesn't show trade-offs or context. Clients see products in isolation without side-by-side comparison or staging of how items work together. Clients can cherry-pick incompatible elements. No feedback loop that helps clients understand the designer's intent before rejecting.
**Mechanism to borrow:** Checkmark/X-mark rapid-accept pattern for final kit approval — not written review, just binary. Pair each kit with a single justification phrase (e.g., "Modern minimalist, $1,200 total") beside the approval buttons so clients understand the curator's intent before accepting or rejecting the bundle.

### Modsy -- Professional Tool *(defunct — closed June 2022)*
**What it does well:** Core mechanic was interactive 3D room rendering with "Live Swap" — click any item in the photorealistic render, instantly swap it from a visual catalog without re-rendering. Customers could customize designs via drag-and-drop 3D editor. ~Two-thirds of customers used the 3D editor to personalize designs, indicating low friction for preference refinement. Style quiz auto-labeled preference upfront ("Rustic Traditional") and seeded initial design accordingly. *(Sources: TechCrunch, Business of Home, Decorilla retrospectives)*
**What's missing:** No structured feedback loop between customer edits and designer response. Live Swap patterns weren't fed back to the AI — if a customer repeatedly swapped in modern pieces, recommendations didn't adapt. Approval was implicit (you placed an order) rather than explicit. Some users reported the 3D editor taking over an hour to rearrange a single design.
**Mechanism to borrow:** Embedded "Live Swap" on final kit previews. Let users click each category (e.g., artwork, rug) to see 2–3 alternatives instantly without a full design revision. Track which swaps users attempt; capture approval by asking "Do you want this design?" only after live-swap experimentation ends. Users arrive at approval having already mentally customized the design.

### Havenly -- Professional Tool
**What it does well:** Binary thumbs-up/thumbs-down rating on product items during early-stage design reviews. Clients rapid-fire approve or reject items with a single thumb gesture. Designers receive aggregated feedback showing which product categories were rejected most (e.g., "80% of contemporary art rejected, 40% of leather sofas") — quantified preference signals instead of vague comments.
**What's missing:** Thumbs system provides no context for *why* an item is rejected — price, color, style, or size? Rejected products disappear without explanation. No comparison mode (sofa A vs. sofa B) within the rating interface — clients make isolated judgments. Flow is unidirectional: client rates → designer redesigns, with no mechanism for the client to propose alternatives.
**Mechanism to borrow:** Extend the thumbs pattern with micro-feedback. After a thumbs-down, offer three fast-tap options: price / color / style / size. Send designers rejection *reasons*, not just counts, enabling targeted adjustment. For final-round approval, use thumbs-up on the full kit bundle (not individual items) paired with cost + style label.

### IKEA Place -- AR Tool
**What it does well:** One-finger drag and two-finger rotate with immediate visual feedback. Anchoring behavior locks items to detected floor/surface planes, removing spatial confusion by showing where an item will actually sit. Multiplacement (added 2019) lets users layer multiple items simultaneously in a single room view without switching contexts.
**What's missing:** AR visualization doesn't connect to purchase. Items placed in AR aren't automatically added to cart — users must navigate back into product browsing, find the item again, and add it manually. Room Sets (themed bundles) exist but lack a "buy this entire setup" button inside the placement view.
**Mechanism to borrow:** Anchored multi-item comparison. Anchor each kit's items to the same surface so users see competing styles in the exact same spatial footprint simultaneously — making A/B comparison the default state in AR, not a secondary action. Embed an add-to-cart button inside that view so the decision moment stays inside AR.

### Wayfair AR -- AR Tool
**What it does well:** "Interactive Photo" decouples AR from being physically in the room — users photograph their space once, then add products asynchronously. Products are true-to-scale with 3D manipulation. Swipe gestures toggle between AR, 3D interactive photo, and standard product view. Feature drove 20% engagement on product pages and 92% conversion lift with 22–40% return rate reduction.
**What's missing:** Conversion breaks at "placed → purchased." Users can view and screenshot AR placements but adding a placed item to cart requires exiting AR and finding the product page manually. Interactive Photo supports multiple items but no comparison mechanism for alternatives side-by-side. Feature discoverability was poor — many users on product pages missed the AR entry point entirely.
**Mechanism to borrow:** Deferred design + in-AR purchase. Let users save their room scan and revisit kit comparisons later (separates "choose your style" from "commit to purchase"). Pair with a direct add-to-cart button positioned *inside* the AR view — a floating button or swipe-up — so purchase doesn't require a context switch.

### Lightning Demo Summary
**Cross-category patterns:** (1) Every tool breaks down at the decision-to-purchase moment — inspiration or visualization is strong, but the bridge to commitment is weak. (2) Side-by-side comparison is nearly absent across all tools; users are forced to compare from memory or sequential viewing. (3) The most effective preference-capture mechanisms are implicit (Pinterest's Taste Graph, Havenly's rejection aggregation) rather than explicit (style quizzes that ask users to self-report).
**Strongest borrowable mechanism:** Havenly's binary thumbs + rejection micro-feedback. It's the only pattern that captures *directional* preference signals (not just approval/rejection) with near-zero friction, and those signals can directly drive the next comparison round's content. Applied to House2Home: track not just which kit wins each round, but *why* the other lost — use that signal to weight the next round's matchup.
**Gap no product solves:** None of the 10 products presents two complete, styled kit options side-by-side in context and lets the user make a single binary choice that progresses the experience. Every tool either shows items in isolation, enables open-ended browsing, or requires the user to manually configure comparisons. House2Home's forced A/B × 3 structure is genuinely novel in this space.

## Crazy 8s -- Round 1: A/B Kit Comparison
**Question:** How do we reduce choice paralysis?
**HMW prompts used:**
1. HMW make each comparison feel like the final one?
2. HMW make the user feel like an expert during the comparison?
3. HMW let the kits explain themselves rather than requiring a read?
4. HMW make "not choosing" feel like progress, not failure?
5. HMW create a sense of momentum through the 3-round structure?
6. HMW show the user what they're moving toward, not just away from?
7. HMW make the chosen kit feel inevitable in retrospect?
8. HMW reduce the fear of choosing wrong?

*[Physical artifact: paper sketch — 8 panels, photographed in Day 3 PDF]*

**Panels sketched (from artifact):**
1. Style Finder entry — "Find Your Style and decorate your home" with Find+ button and kit preview below
2. Style Finder word/emoji selector — "words that describe your style, select 5–8" with emoji grid
3. Style Finder AI branch — "Tell me what I'm missing" / "Generate AI" option
4. Style confirmed — "Your Style: Modern" with kit thumbnail and CTA
5. **A/B Kit Comparison — "1 or 2 — Pick Your Starter Pack"** *(selected as primary direction)*
6. Numbered comparison variant — "9 or 3" with "most" / "3×" labels
7. Kit detail — "Modern... Pack" with items list, price ~$53, Add to Cart / Add Items CTAs
8. AR test entry — "Test Your Starter Pack IN the Home" with Upload App / Take Photo options

**Reflection:**
- **Panels that stood out:** Panel 5 ("1 or 2 — Pick Your Starter Pack") — binary forced choice with no distraction, already style-matched kits pre-loaded so the user only decides between two curated options. Panel 8 (AR test entry) — separates visualization from commitment cleanly.
- **Panels that were layout variations:** Panels 1 and 4 were effectively the same screen at different states rather than distinct interaction models.
- **Interaction model selected:** Binary forced-choice comparison with style-pre-matched kits — "1 or 2" with no third option, no back-out, no browsing. Each round eliminates one option and advances the user toward a single kit.

## Crazy 8s -- Round 2: Style Selector
**Question:** How do we help users identify and commit to a style without overwhelming them?

*[Physical artifact: paper sketch — 8 panels, photographed in Day 3 PDF. Panels explored across the same session as Round 1.]*

**Panels sketched (from artifact):**
1. Word/emoji multi-select — tap 5–8 descriptors from a grid to seed style profile
2. AI generation branch — "Tell me what I'm missing" prompt with AI-generated style suggestions
3. "Your Style: Modern" confirmation screen — style label displayed with kit thumbnails as proof
4. Numbered kit comparison variant — shows multiple options simultaneously with count/price indicators
5. Kit detail with customization — individual item list with swap affordance, total price, add to cart
6. AR test-in-home entry — Upload App / Take Photo two-path entry
7. AR/Generate AI full-screen — immersive visualization of placed items/packs
8. *(Panel left blank / exploratory)*

**Reflection:**
- **Panels that stood out:** The word/emoji multi-select (low cognitive load, implicit style signal) and the AI generation branch (removes the burden of self-knowledge from the user).
- **Interaction model selected:** Two-branch entry into style — users who know their style self-select a label; users who don't use the emoji/word grid or AI generation. Both paths converge on a style confirmation screen before entering kit comparison.

## Critical Screen Decision
**Primary critical screen:** A/B Kit Comparison
**Rationale:** Every lightning demo confirmed that the breakdown point across competitive products is the same: users can discover and visualize, but they stall when forced to commit. The A/B Kit Comparison screen is the moment House2Home either solves this or reproduces it. If the comparison doesn't communicate trade-offs clearly, give the user a decisive signal, and make commitment feel low-risk, the entire upstream UX (style finder, kit curation) loses its value. No competitor has solved this screen — which means getting it right is the primary design bet of the sprint.
**Secondary critical screen:** Style Selector
**Why secondary:** Style Selector determines what enters the comparison rounds. If it produces the wrong kits, the comparison mechanic can't recover. But the Style Selector's UX failure modes (overwhelm, inaccuracy) are well-documented in existing patterns (Homestyler's AI generation, Pinterest's taste graph) — there's more to borrow from. The A/B comparison moment has no direct precedent to borrow from, which is why it takes priority.
