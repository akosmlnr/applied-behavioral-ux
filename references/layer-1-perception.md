# Layer 1 — Perception: Deep Reference

## Fitts's Law — Detailed Design Implications

**The Formula:**
`T = a + b · log₂(D/W + 1)`
- T = time to acquire the target
- D = distance from starting point to target center
- W = width of the target along the axis of motion
- a, b = empirical constants (device/input-dependent)

**Key thresholds (derived from research):**

| Context | Guidance |
|---|---|
| Touch targets | Minimum 44×44pt (iOS HIG) / 48×48dp (Material Design) — non-negotiable for mobile/tablet |
| Desktop pointer targets | No strict minimum — ensure comfort for pointing and adequate spacing to prevent misclicks |
| Primary CTAs | Most visually prominent through contrast, weight, and spacing — not necessarily through raw size |
| Responsive designs | Must meet touch minimums at mobile breakpoints; use fluid sizing and spacing scales |

**Practical Applications:**
- **Edge/corner targets (desktop):** The cursor stops at screen edges, making them effectively infinite in one dimension. This is why fixed/sticky headers and sidebars work well on desktop. On touch devices, edges are less accessible due to device bezels and safe areas — use sticky positioning within comfortable thumb zones instead.
- **Action grouping:** Related actions should be spatially grouped — it reduces the distance between sequential interactions. In modern UIs, this applies to icon clusters in nav bars, grouped action buttons in tool panels, and contextually clustered menu items.
- **Destructive actions:** Place Delete, Remove, etc. far from common actions and require deliberate travel or confirmation (e.g., confirmation dialogs, drag-to-trash).
- **Dropdown menus (desktop):** On desktop, hover-triggered dropdowns should eliminate gaps between the trigger and menu to prevent accidental closure during mouse movement. On mobile/touch, hover is unavailable — use tap-to-toggle menus, bottom sheets, or full-screen selectors. For cross-platform consistency, many modern products use click/tap-to-open everywhere.

## Yarbus — Task-Driven Scanning Patterns

**Key Study (1967):** Yarbus had subjects view Repin's painting "The Unexpected Return" while giving them different tasks: estimate material circumstances, determine ages, remember clothing, remember spatial arrangement, etc. Eye movement recordings showed dramatically different scan patterns for each task — despite viewing the same image.

**Scan Patterns for UI:**
- **Information-seeking:** Top-to-bottom, systematic. Users with this goal need clear structure and consistent layout.
- **Evaluative/Comparison:** Side-to-side scanning between alternatives. Place comparison targets symmetrically.
- **Navigational:** Jump to landmarks (logo, nav bar, back button) then follow scent. Clear navigation anchors are essential.
- **Task completion:** Jump to the input/action area directly. Support this with clear form labels and obvious CTAs.

**Design Implication:** You cannot design for "the average scan" because there is none. Design for the primary task. Secondary tasks should be supported but not prioritized.

## Gestalt Principles — Advanced Applications

### Proximity
- Card UIs work because content within the card boundary is proximate
- Whitespace between sections creates natural grouping without borders
- Form field grouping: use tighter spacing within related field groups and significantly larger spacing between distinct groups. Use your design system's spacing scale consistently — typically 2-3 steps within groups and 4-6 steps between groups

### Similarity
- Color-coding categories: all "warning" elements in amber, all "success" in green
- Navigation items with identical styling are perceived as a set even when spread across the page
- Inconsistent icon styles break similarity and create perceived disorganization

### Continuity
- Left-align body text and form labels — the eye follows a vertical line down
- Horizontal flow in step indicators: 1 → 2 → 3 → 4
- Break continuity intentionally to indicate separate sections or state changes

### Closure
- App icons use this: simplified outlines that the brain completes
- Dotted borders for "add item" zones
- Incomplete circular progress indicators (the brain reads them as a circle with a gap)

### Figure-Ground
- Modal overlays: darkened background (ground), modal (figure)
- Sidebar navigation: collapsed sidebar becomes figure, content becomes ground
- Ensure sufficient contrast between figure and ground — WCAG 4.5:1 for text

### Common Fate
- Animations that move elements together signal they're related
- Drag-and-drop: selected items move in unison
- DON'T animate unrelated elements together — it creates false groupings

### Symmetry
- Login forms centered on page — symmetry creates perceived order
- Two-column feature comparisons use symmetry for direct comparison
- Asymmetry draws attention — use for emphasis, not for layouts

### Past Experience
- Gear icon = settings (universally recognized despite no physical resemblance)
- Magnifying glass = search
- Hamburger menu = navigation (evolved from a literal menu metaphor)
- Cloud icon = sync/storage (modern replacement for physical storage metaphors)
- When breaking convention, ensure the new pattern is clearly taught and consistently applied

## Attention — Advanced Patterns

### Von Restorff Effect (Isolation Effect)
- In a set of similar items, the one that is visually distinct is most likely to be noticed and remembered
- Application: The primary CTA should be the most visually prominent interactive element — through contrast (filled vs outlined), color (brand vs neutral), weight (bold vs regular), or spacing (more padding). Avoid making multiple elements compete for the same level of prominence, which dilutes the effect
- Warning: If multiple elements are "different," the effect is lost. Use sparingly.

### Inattentional Blindness
- The "gorilla experiment" (Simons & Chabris, 1999): ~50% of observers counting basketball passes failed to notice a person in a gorilla suit walking through
- Application: Don't place critical actions near animated elements, video players, or busy visual areas
- Onboarding tooltips near animated transitions are often completely invisible

### Change Blindness
- Users fail to notice changes between views if the transition is gradual
- Application: Use distinct transitions for state changes (success/error)
- Tab switching with subtle changes often goes unnoticed — use clear visual diffs

### Banner Blindness
- Users have learned to ignore visual patterns associated with advertisements — horizontal bars across the top of content, pop-ups, and side panels that look promotional
- Application: Don't place critical content in positions or formats that resemble ads. If using a banner or announcement for legitimate product content, ensure it uses your product's native design language rather than ad-like styling (no flashing, no generic stock photos, no exaggerated marketing language)
- Modern layouts are often single-column and full-width, so "banner blindness" more commonly manifests as ignoring full-width announcement strips — make these feel native to your product UI

---

## Emotional Design (Norman, 2002)

**Source:** Norman, D. (2002). "Emotion & Design: Attractive Things Work Better." *Interactions*, 9(4), 36-42.

**Core Finding:** Norman proposed three levels of emotional design that directly impact cognitive performance:

| Level | Description | UX Implication |
|---|---|---|
| **Visceral** | Immediate emotional reaction to appearance (first 50ms) | First impressions are functional, not cosmetic. Attractive interfaces trigger positive affect that improves problem-solving. |
| **Behavioral** | Usability, performance, feel of use | The "doing" level — does the product perform well? Errors, lag, and friction here create frustration. |
| **Reflective** | Meaning, self-image, personal satisfaction | Brand, story, and identity. "What does using this product say about me?" |

**Key Insight:** Positive visceral reactions literally improve cognitive performance. Attractive interfaces make users more tolerant of minor usability issues and more creative in problem-solving. Visual design is not a luxury layer — it's a performance layer.

---

## Aesthetic-Usability Effect (Kurosu & Kashimura, 1995)

**Source:** Kurosu, M., & Kashimura, K. (1995). "Apparent Usability vs. Inherent Usability." *CHI '95 Conference Companion*.

**Core Finding:** Users consistently rate more aesthetically pleasing interfaces as more usable — even when actual usability is identical across variations.

**Implications:**
- Design investment has measurable ROI beyond "looking nice"
- Users perceive fewer problems and report higher satisfaction with attractive designs
- The effect persists even when users are told to evaluate usability independently of appearance
- This is one reason redesigns that "look better" often get higher satisfaction scores even when functionality hasn't changed

---

## Processing Fluency (Reber, Winkielman & Schwarz, 1998/2004)

**Sources:**
- Reber, R., Winkielman, P., & Schwarz, N. (1998). "Effects of Perceptual Fluency on Affective Judgments." *Psychological Science*, 9(1), 45-48.
- Reber, R., Schwarz, N., & Winkielman, P. (2004). "Processing Fluency and Aesthetic Pleasure: Is Beauty in the Perceiver's Processing Experience?" *Personality and Social Psychology Review*, 8(4), 364-382.

**Core Finding:** Ease of visual processing produces positive affect. People misattribute processing ease to aesthetic preference — things that are easy to perceive are experienced as beautiful and trustworthy.

**Design Implications:**
- Clean typography, familiar layouts, consistent spacing, and clear hierarchy feel "right" because they process fluently
- Consistency across a product increases fluency → increases trust and preference
- Minimalism leverages a cognitive mechanism, not just a style preference
- High fluency signals: legible fonts, predictable placement, clear grouping, low visual noise
- Low fluency signals: unusual fonts, inconsistent layouts, cluttered screens, unfamiliar patterns

**When to Use Disfluency Intentionally:**
- Important disclaimers or terms of service (slightly harder-to-read text increases attention and memory)
- Warning messages (disfluency signals "pay attention")
- Learning content where deeper processing is desired
- Not for primary UI, navigation, or CTAs — always use fluency there

---

## Color Psychology (Elliot & Maier, 2014)

**Source:** Elliot, A. J., & Maier, M. A. (2014). "Color Psychology: Effects of Perceiving Color on Psychological Functioning in Humans." *Annual Review of Psychology*, 65, 95-120.

**Core Finding:** The most comprehensive review of color-psychology research. Color carries meaning and impacts affect, cognition, and behavior. Effects are context-dependent (Color-in-Context Theory).

**Key Findings:**
- Red in achievement contexts → avoidance, danger (but attractiveness in romantic contexts)
- Blue → trust, communication, calm (highly effective for SaaS, finance, healthcare)
- Green → approach, go, nature, money (effective for positive action CTAs)
- Color effects are not universal "hacks" — they depend on the user's current task and context
- Contrast and saturation matter more than hue for visibility; hue matters for emotional tone

**Design Implications:**
- CTA color should match the emotional tone of the action (positive action = warm/positive color, warning = red)
- Don't rely on "green button converts better" myths — test in your specific context
- Use color consistently for the same semantic meaning across the product
- Ensure sufficient contrast for accessibility (WCAG AA minimum)
