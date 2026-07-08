# Applied Behavioral UX

**A research-grounded 5-layer framework for evaluating and designing user experiences using behavioral science.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Unlike style-focused UX guides, this framework applies peer-reviewed findings from psychology, behavioral economics, and neuroscience directly to product decisions.

## The Framework

```
Layer 1 — Perception (How users SEE)
  Gestalt · Yarbus · Fitts · Visual Hierarchy · Attention · Emotional Design · Processing Fluency
       ↓
Layer 2 — Cognition (How users THINK)
  Cognitive Load · Miller · Mental Models · Hick · Information Foraging · Zeigarnik · Flow
       ↓
Layer 3 — Decision Making (How users CHOOSE)
  Prospect Theory · Loss Aversion · Nudge · Choice Architecture · Cialdini · Hyperbolic Discounting
       ↓
Layer 4 — Motivation (Why users ACT)
  Self-Determination Theory · Goal Theory · Habit Formation · Peak-End Rule · Social Identity
       ↓
Layer 5 — Product Behavior (What the product DOES)
  Activation · Onboarding · Retention · Conversion · Trust · Pricing
```

## What's Inside

| File | Description |
|---|---|
| [`SKILL.md`](SKILL.md) | The complete framework — principles, checklists, evaluation & design templates |
| [`references/`](references/) | Deep-dive reference files for each layer with extended research citations |

### Reference Files

- [`references/layer-1-perception.md`](references/layer-1-perception.md) — Visual processing, eye tracking, attention, emotional design, processing fluency, aesthetic-usability effect
- [`references/layer-2-cognition.md`](references/layer-2-cognition.md) — Cognitive load, memory, mental models, information foraging, mere exposure, Zeigarnik effect, flow state
- [`references/layer-3-decisions.md`](references/layer-3-decisions.md) — Prospect theory, choice architecture, Cialdini's influence principles, endowment effect, regulatory focus, construal level theory
- [`references/layer-4-motivation.md`](references/layer-4-motivation.md) — Self-determination theory, goal-gradient hypothesis, habit formation, Fogg behavior model, peak-end rule, expectancy-value theory, social identity
- [`references/layer-5-product.md`](references/layer-5-product.md) — Activation, onboarding, retention, conversion, trust, pricing psychology

## Foundational Research

This framework synthesizes findings from 40+ peer-reviewed papers and seminal works across:

**Psychology & Neuroscience**
- Kahneman & Tversky (1979) — Prospect Theory
- Norman (2002) — Emotional Design
- Csikszentmihalyi (1975) — Flow Theory
- Reber, Winkielman & Schwarz (1998/2004) — Processing Fluency
- Zeigarnik (1927) — Incomplete Task Retention

**Behavioral Economics**
- Thaler (1980/1991) — Endowment Effect & Loss Aversion
- Ainslie (1975) — Hyperbolic Discounting
- Kahneman & Tversky (1984) — Framing Effects
- Samuelson & Zeckhauser (1988) — Status Quo Bias

**Motivation & Social Psychology**
- Deci & Ryan (1985) — Self-Determination Theory
- Tajfel & Turner (1979) — Social Identity Theory
- Cialdini (1984) — Principles of Influence
- Locke & Latham (1990) — Goal Setting Theory

**Perception & Attention**
- Fitts (1954) — Law of Target Acquisition
- Yarbus (1967) — Task-Driven Eye Movements
- Kurosu & Kashimura (1995) — Aesthetic-Usability Effect
- Treisman & Gelade (1980) — Feature Integration Theory

**Applied Frameworks**
- BJ Fogg (2009) — Behavior Model (B = MAP)
- Eyal (2014) — Hook Model
- Balfour (Reforge) — Activation Framework
- Pirolli & Card (1999) — Information Foraging Theory

## How to Use

### Evaluate an existing product or flow
Walk through each layer top-to-bottom. For each layer, identify what's working and what violates the principle. End with prioritized recommendations.

### Design a new feature or flow
Walk through each layer bottom-up (Layer 5 → Layer 1) to ground design decisions in behavioral outcomes first, then work back to visual execution.

### Diagnose a specific problem
Jump to the relevant layer:
- Conversion isn't converting? → **Layer 3 (Decision Making)**
- Users aren't finding features? → **Layer 2 (Cognition)**
- Users churn after signing up? → **Layer 5 (Product Behavior) → Activation/Onboarding**
- Engagement is declining? → **Layer 4 (Motivation) → Habit Formation**

## As a ZCode Skill

This framework is designed as a [ZCode](https://zcode.ai) skill for AI-assisted UX evaluation and design. It triggers on UX reviews, usability critiques, conversion optimization, behavioral design, and any question about *why* users behave a certain way in a product.

## Ethical Use

This framework describes how human psychology works. It includes ethical guardrails:

- **Dark patterns violate the framework itself** — They undermine Autonomy (Layer 4)
- **Nudge ≠ Manipulate** — Nudges preserve freedom of choice
- **Loss aversion is a tool, not a weapon** — Fabricating losses (false urgency, fake scarcity) is not a nudge
- **Variable rewards become addiction when users lose control** — Design for engagement, not compulsion

## Contributing

Found a missing paper? Have a UX insight backed by research? PRs welcome — especially:

- Additional peer-reviewed papers mapped to the appropriate layer
- Real-world case studies applying specific principles
- Cross-cultural considerations for any principle
- Counter-examples where a principle doesn't hold

## License

MIT
