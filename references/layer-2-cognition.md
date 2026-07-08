# Layer 2 — Cognition: Deep Reference

## Cognitive Load Theory — Applied Checklist

**Sweller (1988, 1994) — Key Effects to Avoid:**

### Split-Attention Effect
When related information is separated spatially (e.g., a diagram with labels on a separate page), cognitive load increases because the user must mentally integrate the pieces.
- **Fix:** Place labels directly on diagrams, put instructions inline with the interface
- **Example:** Form validation messages should appear directly next to the field, not at the top of the page

### Redundancy Effect
Presenting the same information in multiple forms simultaneously can increase load rather than decrease it.
- **Fix:** Don't provide both a text explanation AND an identical audio narration AND a diagram saying the same thing
- **Example:** Don't show a tooltip that repeats the button label. Either show additional info or show nothing.

### Modality Effect
Working memory has separate channels for visual and auditory processing. Using both channels effectively increases total capacity.
- **Fix:** Pair visual instructions with audio cues for complex tasks (e.g., navigation apps combine map visuals with voice instructions)
- **Example:** Show a video tutorial (visual+auditory) rather than a wall of text (visual only)

### Expertise Reversal Effect
Techniques that reduce load for novices can increase load for experts (because experts have already automated the underlying knowledge).
- **Fix:** Allow users to dismiss/skip scaffolding (progressive disclosure handles this naturally)
- **Example:** "Don't show me this again" checkboxes, keyboard shortcuts for power users

## Miller's Law — Practical Chunking Guide

**Original finding:** 7±2 items in working memory. Modern research (Cowan, 2001) suggests the actual capacity is closer to **4±1** chunks.

### Chunking by Context

| Context | Recommended Max | Rationale |
|---|---|---|
| Navigation items | 5-7 | Users scan nav items as chunks |
| Form fields per group | 3-5 | More feels overwhelming |
| Pricing tiers | 3 | Good/Better/Best is the gold standard |
| List items per view | 7-10 | Beyond this, add search/filter |
| Notification categories | 3-5 | More creates notification fatigue |
| Onboarding steps | 3-5 total | Each step should be atomic |
| Feature comparison points | 5-7 | Beyond this, users stop comparing |

### Effective Chunking Strategies
- **Spatial grouping** — Cards, sections, white space
- **Categorization** — Group by user's mental model, not technical architecture
- **Progressive disclosure** — Reveal detail on demand
- **Temporal sequencing** — Step-by-step wizards (but keep total steps ≤ 5)
- **Search** — For large option sets (>20), replace browsing with search + filter

## Mental Models — Identification Guide

**Common user mental models:**

| Domain | User's Mental Model | Design Implication |
|---|---|---|
| File storage | Physical filing cabinet (folders, documents) | Use folder/file metaphor |
| Shopping cart | Physical shopping basket | Cart icon, "add to cart," "checkout" |
| Social media | Physical social gathering | "feed" (like a table), "share," "like" (nod) |
| Email | Physical mailbox | Inbox, sent, drafts, trash |
| Photo management | Physical photo album | Albums, collections, favorites |
| Settings | Physical controls/dials | Toggles, sliders, knobs |
| Search | Physical index/directory | Search bar, results list |
| Calendar | Physical wall calendar | Monthly/weekly view, events as blocks |

**When mental models conflict with your product:**
1. Match the dominant model if possible (lowest friction)
2. If innovating, explicitly teach the new model with a metaphor or analogy
3. Use existing conventions for navigation but innovate in the core interaction
4. Never assume users will "figure it out" — if the model is novel, teach it

**Red flags that your product's model mismatches users:**
- Users click "back" expecting it to undo their last action (not navigate)
- Users look for "save" when the product auto-saves
- Users search for a feature in the place it "should" be, not where you put it
- Users call things by the wrong name (they're using their own model)

## Hick's Law — Choice Optimization

**The Formula:**
`RT = a + b · log₂(n + 1)`
- RT = reaction time
- n = number of choices
- a, b = empirical constants

**Key insight:** The relationship is logarithmic, not linear. The difference between 2 and 4 choices is small. The difference between 2 and 32 choices is large.

### Optimal Choice Counts by Context

| Context | Optimal Choices | Maximum Acceptable |
|---|---|---|
| Primary navigation | 4-7 | 10 (with grouping) |
| Pricing tiers | 3 | 4 (never more) |
| Form dropdowns | 5-7 | 15 (with search) |
| Action menus (contextual) | 3-5 | 10 (with grouping) |
| Settings toggles per page | 5-7 | 15 (with grouping) |
| Notification types | 3-5 | 8 |

### Techniques for Reducing Effective Choice Count
1. **Defaults** — Pre-select the most common option (reduces effective n by 1)
2. **Smart sorting** — Put the most likely choice first (reduces scan time even if n stays the same)
3. **Recommendation** — "We recommend X" (reduces effective choices to 2: the recommended one and "other")
4. **Progressive disclosure** — Show 3-5, with "More options..." for the rest
5. **Categorization** — Group 20 items into 4 categories of 5 items each (effectively 4 choices then 5)

## Information Foraging Theory — Design Patterns

**Pirolli & Card (1999):** Users navigate information systems like animals forage for food — they follow "scent" and optimize for information gained per unit of effort.

### Information Scent Optimization

**What creates strong scent:**
- Descriptive, specific labels ("Upload CSV file" not "Upload")
- Preview text and thumbnails for links
- Clear icons that match expectations
- Breadcrumbs showing path
- Search result snippets with highlighted matches
- Price and availability visible before clicking

**What kills scent:**
- Generic labels ("Learn More," "Click Here," "Submit")
- Mystery meat navigation (icon-only buttons without labels)
- Hidden content behind hover (mobile users can't hover)
- Missing preview images for content
- Vague category names ("Resources," "Solutions")

### Patch Model Application
Users stay in a "patch" (page/section) until the perceived yield drops below the cost of moving to a new patch.

**Design for good patch transitions:**
- Related content suggestions at the bottom of articles (reduces cost of moving)
- Breadcrumbs and persistent navigation (lowers switching cost)
- "Back to results" from detail pages (obvious exit from current patch)
- Content feeds that keep surfacing relevant items (extends the current patch)

### Navigation Cost Reduction
- **Reduce clicks:** Every click between the user and value adds cost
- **Persistent navigation:** Users shouldn't have to scroll to the top to navigate
- **Keyboard shortcuts:** Dramatically reduce navigation cost for power users
- **Predictive navigation:** Suggest where the user might go next (recent items, favorites, frequently visited)

---

## Mere Exposure Effect (Zajonc, 1968)

**Source:** Zajonc, R. B. (1968). "Attitudinal Effects of Mere Exposure." *Journal of Personality and Social Psychology*, 9(2), 1-27.

**Core Finding:** Repeated exposure to a stimulus increases liking — no reward or reinforcement needed. This is one of the most robust findings in social psychology.

**Design Implications:**
- Consistent design patterns across a product build preference through exposure, not just learnability
- New design patterns are initially disliked but grow on users with repeated interaction — don't abandon a redesign based only on first-impression feedback
- Familiar UI conventions are preferred partly because of mere exposure
- Repeated brand exposure in-product (consistent logo placement, color scheme, typography) increases brand affinity over time
- Onboarding benefits from using familiar patterns — users already have positive exposure to them from other products

---

## Zeigarnik Effect (1927)

**Source:** Zeigarnik, B. (1927). "Über das Behalten von erledigten und unerledigten Handlungen" (On the Retention of Completed and Uncompleted Tasks). *Psychologische Forschung*, 9, 1-85.

**Core Finding:** Unfinished or interrupted tasks are remembered significantly better than completed ones — up to 90% better recall for incomplete tasks.

**Design Implications:**
- Profile completion bars, setup checklists, and "2 of 5 steps remaining" leverage the Zeigarnik effect to drive completion
- Shopping cart indicators ("3 items in your cart") create persistent cognitive tension
- Unread notification badges work through the same mechanism
- "Finish setting up your profile" reminders are effective because the brain holds incomplete tasks in active memory

**Caution:**
- Overuse creates anxiety — too many incomplete indicators overwhelm users
- Use for 1-2 critical completion tasks, not for every possible incomplete state
- Always pair with a clear, easy path to completion

---

## Flow State (Csikszentmihalyi, 1975)

**Source:** Csikszentmihalyi, M. (1975). *Beyond Boredom and Anxiety: The Experience of Play in Work and Games*. Jossey-Bass.

**Core Finding:** Flow is a state of optimal experience where challenge matches skill. In flow: time distorts, focus is total, performance peaks, and satisfaction is high.

**The Flow Channel:**

```
High Challenge
    │
    │  ANXIETY ←── Flow ──→ BOREDOM
    │              (optimal)
    │
Low Skill              High Skill
```

**Design Implications:**
- Match default difficulty/settings to the user's likely skill level (not the power user's level)
- Progressive difficulty in onboarding: start simple, add complexity as competence builds
- Clear, immediate feedback is essential to maintaining flow — users need to know how they're doing
- Avoid interruptions during flow states (don't show modals, requests, or prompts during active work)
- Games and productivity tools are the most obvious flow candidates, but any tool that supports deep work should optimize for flow
- Skill-appropriate defaults are one of the most impactful onboarding decisions

**Flow Killers to Avoid:**
- Frequent interruptions (notifications during active use)
- Tasks that are too easy (boredom → disengagement)
- Tasks that are too hard (anxiety → abandonment)
- Unclear goals or progress indicators
- Lag, errors, or unpredictable behavior

---

## Serial Position Effect (Primacy & Recency)

**Source:** Ebbinghaus, H. (1885/1964). *Memory: A Contribution to Experimental Psychology*. Dover.

**Core Finding:** Items at the beginning (primacy) and end (recency) of a list are remembered significantly better than items in the middle. This is one of the most robust findings in memory research.

**Design Implications:**
- **Navigation:** First and last nav items get disproportionate attention — place the most important actions there
- **Pricing tiers:** Leftmost and rightmost tiers are most memorable; the middle tier benefits from the compromise effect but is least remembered in isolation
- **Feature lists:** First and last features in comparison tables carry disproportionate weight — lead with your strongest feature, end with your second strongest
- **Error messages:** In multi-field forms, the first error gets the most attention (also related to serial position)
- **CTA groups:** If you have multiple buttons, the first and last get the most clicks
- **Menus and dropdowns:** Items at the top and bottom are selected most frequently

---

## Conservation of Complexity (Tesler's Law)

**Source:** Tesler, L. (1984). "The Limits of Intelligence." *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*.

**Core Finding:** "Every application has an inherent amount of complexity that cannot be removed, only moved between user and system." Complexity is conserved — simplifying the UI means the system must be smarter.

**Design Implications:**
- Before removing a feature to "simplify," ask: did you actually reduce complexity, or just push it onto the user?
- Smart defaults absorb complexity (the system makes good choices so the user doesn't have to)
- AI-powered suggestions and automation are complexity absorbers — they let the system handle the inherent complexity
- Progressive disclosure redistributes complexity across time (showing advanced options later, not eliminating them)
- The difference between simplifying (removing capability) and abstracting (hiding complexity behind a better interface) is critical
- When users say "make it simpler," they often mean "make the system handle the complexity for me"

---

## Mayer's Multimedia Learning Principles (2009)

**Source:** Mayer, R. E. (2009). *Multimedia Learning* (2nd ed.). Cambridge University Press.

**Core Finding:** 25+ years of research synthesized into 12 evidence-based principles for designing instructional content. The most UX-relevant:

| Principle | Description | UX Application |
|---|---|---|
| **Coherence** | Remove extraneous material | Onboarding should only teach what's needed immediately; cut decorative illustrations, background music, extra details |
| **Contiguity** | Place related elements together | Labels next to (not below) form fields; explanations next to the feature they describe |
| **Modality** | Use narration + graphics rather than text + graphics | Video walkthroughs with voiceover outperform text overlays for onboarding |
| **Signaling** | Highlight essential information | Visual cues (arrows, highlights, step indicators) direct attention to what matters |
| **Segmenting** | Present complex lessons in learner-paced segments | Break long tutorials into steps the user controls — don't auto-play a 5-minute walkthrough |
| **Pre-training** | Teach key concepts before the lesson | Name key features/terms before explaining how to use them (familiar terminology reduces cognitive load) |

**Design Implications:**
- Directly applicable to onboarding flows, help documentation, and instructional UI
- Explains WHY video onboarding outperforms text-only onboarding (modality principle)
- Explains why progressive disclosure works better than information dumps (segmenting + coherence)
- Most effective when combined with Cognitive Load Theory (already covered in this layer)

---

## Dual-Task Interference / Task Switching Cost

**Sources:**
- Miyake, A., et al. (2000). "The Unity and Diversity of Executive Functions." *Journal of Experimental Psychology: General*, 129(1), 4-28.
- Monsell, S. (2003). "Task Switching." *Trends in Cognitive Sciences*, 7(3), 134-140.

**Core Finding:** Switching between tasks has a measurable cognitive cost. Each switch degrades performance on both tasks. The cost persists even when the switch is voluntary.

**Design Implications:**
- Modal dialogs that interrupt a primary task impose dual-task interference (user must manage both the modal and their original goal)
- Inline validation (showing errors next to the field) is better than post-submission validation (which forces a switch to an "error review" task)
- Multi-step flows should maintain single-task focus — don't ask users to configure settings while also completing a primary action
- Context switching between product features (e.g., switching from editing to viewing to settings) should be minimized or made seamless
- Notifications during active use are the most common source of forced task switching in products
