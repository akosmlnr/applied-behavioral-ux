# Mobile UX Research: Foundational Papers and Studies for the 5-Layer Behavioral UX Framework

## Purpose and Methodology

This document catalogs research papers and studies specifically about mobile UX, mobile design psychology, and mobile behavioral differences, organized by the 5-layer framework. For each entry, I distinguish between:

- **NEW principle**: A finding that is genuinely unique to mobile -- true on mobile but NOT true (or fundamentally different) on desktop
- **APPLIED principle**: An existing general principle (like Fitts's Law) applied to mobile context -- the principle itself is not mobile-specific, but the application has mobile-unique implications

The distinction matters. Many "mobile UX principles" are actually existing psychology/UX principles applied to smaller screens. True mobile-unique findings are rarer and more valuable for building a genuinely mobile-specific layer.

---

## LAYER 1 -- Perception: Visual Processing, Attention, Eye Tracking on Mobile

---

### 1. Thumb Zone Research

**Hoober, S. (2013). "How Do Users Really Hold Mobile Devices?" UXmatters.**
- **Layer:** 1 (Perception) -- specifically touch ergonomics
- **Key finding:** Observational study of 1,333 real-world mobile device interactions. Found three grip patterns: **49% one-handed (thumb only), 36% cradle (one hand holds, other finger taps), 15% two-handed (both thumbs)**. The thumb is the dominant input mechanism, and reachability varies dramatically by grip type and phone size.
- **NEW vs APPLIED:** **Partially new.** The *distribution of grip types* and the *thumb zone heat map* are mobile-unique findings -- they have no desktop analog. However, the underlying principle is an application of human biomechanics/anthropometrics to the specific form factor. The concept of "reachability zones" (natural, stretch, awkward) is genuinely mobile-specific because it depends on the physical relationship between hand, device, and screen size.

**Parhi, P., Karlson, A.K., & Bederson, B.B. (2006). "Target Size Study for One-Handed Thumb Use on Small Touchscreen Devices." MobileHCI.**
- **Layer:** 1 (Perception)
- **Key finding:** Foundational MobileHCI study determining optimal target sizes for one-handed thumb use. Showed that thumb accuracy degrades significantly toward screen edges, especially in the bottom corners. Recommended minimum target sizes of 9-10mm for reliable one-handed thumb input.
- **NEW vs APPLIED:** **Applied (Fitts's Law).** This is a direct application of Fitts's Law to thumb-based touch input. The principle itself is not new. However, the *quantitative data about thumb accuracy by screen region* is mobile-unique empirical work.

**Henning, Pohl et al. (2019). "The Influence of Hand Size on Touch Accuracy."**
- **Layer:** 1 (Perception)
- **Key finding:** Examined how physical hand dimensions (thumb length, hand breadth) influence touch accuracy. Found significant individual variation in accuracy based on hand size, suggesting that universal target size guidelines may be insufficient.
- **NEW vs APPLIED:** **Applied.** Extends Fitts's Law with anthropometric data. The individual variation finding is useful but still within the Fitts's Law framework.

**MDPI (2020). "Effects of Smartphone Size and Hand Size on Grip Posture in One-Handed Use." Applied Sciences.**
- **Layer:** 1 (Perception)
- **Key finding:** Identified user-preferred grip postures based on smartphone size and hand size for one-handed operation. Larger phones require more grip shifts and postural adjustments.
- **NEW vs APPLIED:** **Partially new.** The finding that phone size affects *grip type distribution* (not just comfort) is a mobile-specific insight without desktop analog.

---

### 2. Fitts's Law Adapted for Touch Screens

**Bi, X., Li, S., & Zhai, S. (2013). "FFitts Law: Modeling Finger Touch with Fitts' Law." CHI '13.**
- **Layer:** 1 (Perception)
- **Key finding:** Proposed "FFitts Law" -- an enhanced Fitts's Law model specifically for finger-based touchscreens. The standard Fitts's Law underestimates movement time for finger input because the finger is not a precision pointing device (it has width, it occludes the target). FFitts Law accounts for finger width and the offset between finger centroid and actual touch point.
- **NEW vs APPLIED:** **Applied but with genuine new contribution.** The core law is Fitts's. But the *correction for finger occlusion and the offset between visual target and physical contact point* is a genuinely new principle that only applies to direct-touch interfaces (no mouse cursor exists to bridge the gap). This means on mobile, users touch BELOW where they think they're touching due to finger anatomy -- a finding with no desktop equivalent.

---

### 3. Mobile Eye Tracking / Attention Patterns

**Nielsen, J. (2006/2024). "F-Shaped Pattern of Reading on the Web." NN/g.**
- **Layer:** 1 (Perception)
- **Key finding:** The F-shaped scanning pattern (horizontal scan at top, shorter horizontal scan below, then vertical scanning along left edge) persists on both desktop and mobile. On mobile, the pattern is more compressed vertically due to narrower viewport, but the fundamental scanning behavior is the same.
- **NEW vs APPLIED:** **Applied.** The F-pattern itself was originally discovered on desktop. The finding that it persists on mobile is confirmation, not a new discovery. However, the compression effect on narrow screens has practical mobile implications.

**Nielsen, J. (2018). "Scrolling and Attention." NN/g.**
- **Layer:** 1 (Perception)
- **Key finding:** Eyetracking data shows people still devote more visual attention to what's initially visible (above the fold) than below it. However, mobile users scroll more freely than desktop users -- touch interfaces make scrolling natural. The "fold" on mobile is much lower (less content visible), so more content is below the fold, and users do scroll to it.
- **NEW vs APPLIED:** **Partially new.** The finding that *mobile users scroll significantly more than desktop users* is mobile-specific, driven by the touch interface making scrolling effortless (vs. mouse wheel/scrollbar). The above-the-fold attention bias is a general finding applied to mobile.

**Google/Think with Google. "Eye Tracking Study: Comparing Mobile and Desktop."**
- **Layer:** 1 (Perception)
- **Key finding:** Direct eyetracking comparison between mobile and desktop advertising contexts. Found that mobile attention is more concentrated -- smaller screens force focus, so users spend more time per element they view, but view fewer total elements per session.
- **NEW vs APPLIED:** **Partially new.** The finding that *smaller screens create more concentrated attention per element* (fewer elements visible = more focused gaze) is a genuine mobile-specific perceptual phenomenon. On desktop, peripheral elements compete for attention; on mobile, fewer elements are visible simultaneously.

---

### 4. Dark Mode / OLED Color Perception

**Wen, Z. et al. (2021). "Study on the Effects of Display Color Mode and Luminance Contrast on Visual Fatigue."**
- **Layer:** 1 (Perception)
- **Key finding:** Analyzed dark mode effects on visual fatigue. Found that dark mode with appropriate contrast reduces visual fatigue in low ambient light, but poor contrast in dark mode increases fatigue. The relationship between ambient light and optimal color mode is significant.
- **NEW vs APPLIED:** **Partially new.** Dark mode is primarily a mobile phenomenon (OLED screens on phones). The finding that ambient light modulates the optimal mode is relevant to mobile's portability -- phones are used in varied lighting conditions in ways desktops typically are not.

**Google/Purdue University. "The Impact of Color Schemes on Device Energy Consumption."**
- **Layer:** 1 (Perception) -- indirect (affects battery, which affects behavior)
- **Key finding:** Dark mode on OLED smartphones extends battery life by up to 30-60% at full brightness. This creates an *economic incentive* to use dark mode on mobile that has no desktop equivalent (LCD desktop monitors don't benefit from dark mode in the same way).
- **NEW vs APPLIED:** **New behavioral implication.** While the physics of OLED power consumption isn't a UX principle, the *resulting behavioral implication* is mobile-unique: users on mobile have a rational reason to prefer dark mode (battery life), creating a feedback loop where dark mode adoption changes color behavior on mobile in ways that don't apply to desktop.

---

## LAYER 2 -- Cognition: Cognitive Load Differences on Mobile, Information Processing on Small Screens

---

### 5. Screen Size and Cognitive Load

**Al-Mushasha, F. et al. (2021). "The Effect of Screen Size on Students' Cognitive Load in Mobile Learning." Journal of Educational Technology and Learning (JETL).**
- **Layer:** 2 (Cognition)
- **Key finding:** Surveyed 1,570 students. Counterintuitively, **smaller screens produced lower cognitive load** than larger screens for the same learning content. The hypothesis is that smaller screens naturally limit visible content, reducing extraneous cognitive load from information overload and forcing sequential processing rather than parallel processing.
- **NEW vs APPLIED:** **Genuinely new.** This is a mobile-specific finding that contradicts the intuitive assumption that "smaller screen = harder to process." The mechanism (natural content limitation reduces extraneous load) is a genuinely new cognitive principle that only applies to constrained-viewport devices. On desktop, all content is visible simultaneously, creating potential split-attention overload. Mobile's small screen acts as a natural progressive disclosure mechanism.

**Hwang, G.J. et al. (2018). "Cognitive Load Management in Mobile Learning Systems." PMC/NIH.**
- **Layer:** 2 (Cognition)
- **Key finding:** Reviews the split-attention principle in mobile contexts. Content on small screens requires scrolling between related elements (e.g., a diagram and its label on different "pages"), increasing extraneous cognitive load through split attention. However, well-designed mobile interfaces that present related information together can actually achieve lower extraneous load than desktop by limiting distractions.
- **NEW vs APPLIED:** **Applied (Cognitive Load Theory -- Sweller).** This is Sweller's split-attention effect applied to mobile. However, the *tension between natural content limitation (reducing load) and forced scrolling (increasing split-attention)* is a genuinely mobile-specific design trade-off with no desktop parallel.

**ScienceDirect (2021). "Impact of Screen Size on Cognitive Training Task Performance."**
- **Layer:** 2 (Cognition)
- **Key finding:** Visual stimulus size significantly impacts performance on working memory tasks. Smaller visual stimuli lead to lower performance on certain memory tasks, suggesting that information that is harder to see/perceive also engages more cognitive resources.
- **NEW vs APPLIED:** **Applied.** This relates to general perceptual encoding -- smaller text/images are harder to perceive, which loads working memory more. The principle is not mobile-specific, but the application to mobile screen sizes is relevant.

---

### 6. Mobile Reading Patterns

**ACM (2022). "Characteristics of Deep and Skim Reading on Smartphones vs Desktop."**
- **Layer:** 2 (Cognition)
- **Key finding:** Mobile reading tends toward skimming with shorter fixation durations and less regression (re-reading). Desktop environments support deeper reading with longer fixations and more regressions. The difference is not just in comprehension scores but in *processing strategy* -- mobile users adopt a different cognitive approach to reading.
- **NEW vs APPLIED:** **Partially new.** The finding that users *strategically shift their reading strategy based on device* is a genuinely mobile-specific cognitive finding. Users don't just read the same way on a smaller screen -- they adopt a fundamentally different processing approach (skim vs. deep). This is not about ability but about adaptive strategy, which is mobile-unique.

**Nielsen Norman Group (2020). "Reading Content on Mobile Devices."**
- **Layer:** 2 (Cognition)
- **Key finding:** Readers can understand short, simple text on mobile devices just as well as on computers. However, they **slow down significantly when reading difficult/complex text on mobile**, suggesting that complex content creates disproportionately higher cognitive load on small screens.
- **NEW vs APPLIED:** **Partially new.** The interaction between *text complexity* and *device type* is a mobile-specific finding. Simple text processes equally well across devices; complex text creates a mobile penalty. This suggests that content simplification on mobile is not just aesthetic but cognitively necessary for complex material.

**Rello, L. et al. (2016). "Make It Big! Font Size and Line Spacing on Online Readability."**
- **Layer:** 2 (Cognition)
- **Key finding:** With 104 participants, readability (measured via mean fixation duration) increased significantly with font size. Comprehension also benefited from larger fonts and adequate line spacing. This applies to mobile where font size scaling is more critical.
- **NEW vs APPLIED:** **Applied.** This is general typographic research, not mobile-specific. However, on mobile, font size decisions matter more because the baseline is already constrained.

---

### 7. Smartphone "Mere Presence" Effect

**Ward, A.F., Duke, K., Gneezy, A., & Bos, M.W. (2017). "Brain Drain: The Mere Presence of One's Own Smartphone Reduces Available Cognitive Capacity." Journal of the Association for Consumer Research, 2(2), 140-154.**
- **Layer:** 2 (Cognition)
- **Key finding:** The mere presence of one's own smartphone reduces available cognitive capacity, even when the phone is turned off. Participants performed worse on cognitive tasks when their phone was nearby (on the desk) vs. in another room. The effect was strongest when the phone was the participant's own (not a stranger's). This is called the "brain drain" effect.
- **NEW vs APPLIED:** **Genuinely new (mobile-specific cognitive phenomenon).** This is one of the most significant mobile-unique findings. The smartphone as a cognitive "leech" -- drawing mental resources even when not in use -- has no desktop analog. A desktop computer sitting nearby does not produce the same effect. This is specific to the smartphone's role as a personal, always-connected, potentially-rewarding device. For mobile UX design, this means: the user's cognitive capacity is *already diminished* by the mere fact that they're using a smartphone, before any UI complexity is added.

**Nature Scientific Reports (2023). "The Mere Presence of a Smartphone Reduces Basal Attentional Capacity."**
- **Layer:** 2 (Cognition)
- **Key finding:** Replicated and extended the brain drain finding. The mere presence of a smartphone results in lower cognitive performance, supporting the hypothesis that smartphone presence uses limited cognitive resources even without active interaction. The effect persists across multiple task types.
- **NEW vs APPLIED:** **Genuinely new.** Further confirmation that this is a robust, replicable mobile-specific cognitive effect.

---

## LAYER 3 -- Decision Making: Choice Behavior on Mobile, Mobile Conversion Patterns

---

### 8. Mobile Conversion Differences

**Multiple industry studies (2024-2026 data):**
- DRIP (2026): 117 European brands, 486M sessions -- desktop 3.93% vs mobile 2.46% conversion
- BMG360: Desktop converts 1.9x more than mobile across 15 brands
- Shopify (2026): Desktop consistently outperforms mobile in e-commerce conversion
- **Layer:** 3 (Decision Making) / 5 (Product Behavior)
- **Key finding:** Mobile drives 54-70% of e-commerce traffic but converts at only 1.4-2.8% vs desktop's 3.2-4.0%. The mobile conversion gap persists despite responsive design and faster load times.
- **NEW vs APPLIED:** **Applied with mobile-specific causes.** Conversion optimization is a general principle. But the *specific friction points* that cause the mobile gap are mobile-unique: smaller screens make product evaluation harder, mobile checkout forms are harder to complete with thumbs, security concerns with mobile payment, and the context of mobile shopping (on-the-go, distracted) creates different decision-making conditions.

**ScienceDirect (2024). "Choose a Mobile Application or Mobile Website? Different Effects on Consumer Behavior."**
- **Layer:** 3 (Decision Making)
- **Key finding:** Despite both being optimized for mobile, apps and mobile websites offer fundamentally different user experiences that significantly influence consumer behavior and engagement. Apps create a more immersive, higher-commitment context; mobile web is more exploratory and lower-commitment.
- **NEW vs APPLIED:** **Partially new.** The finding that the *same content in an app vs mobile browser* produces different behavioral outcomes is mobile-specific. This "container effect" (the platform shapes the behavior, not just the content) has implications for mobile decision architecture.

---

### 9. Google Micro-Moments Research

**Google/Think with Google (2015). "How Micro-Moments Are Changing the Rules."**
- **Layer:** 3 (Decision Making)
- **Key finding:** Mobile has fractured the consumer decision journey into hundreds of micro-moments -- intent-rich moments where users reflexively turn to their phones to learn, do, discover, or buy. These moments are characterized by high intent, impatience, and preference for immediate relevance. Four types: I-want-to-know, I-want-to-go, I-want-to-do, I-want-to-buy.
- **NEW vs APPLIED:** **Genuinely new (mobile-specific decision-making pattern).** Micro-moments are a genuinely new consumer behavior pattern driven by mobile's always-carried, always-on nature. The decision journey on mobile is not a smaller version of desktop -- it's fundamentally fragmented into smaller, more frequent, more context-dependent decision points. This is a mobile-unique principle with no desktop equivalent.

**Google/Think with Google. "How Mobile Has Redefined the Consumer Decision Journey."**
- **Layer:** 3 (Decision Making)
- **Key finding:** Mobile has transformed the consumer journey from a linear funnel to a non-linear, looping process. Consumers loop between exploration and evaluation multiple times before purchase, and mobile is the primary device for most of these loops.
- **NEW vs APPLIED:** **Partially new.** While non-linear decision journeys exist in general, the *degree of fragmentation and looping* driven by mobile is qualitatively different. Mobile enables continuous, ambient decision-making that was impossible with desktop.

---

## LAYER 4 -- Motivation: Mobile Engagement, Push Notification Behavior, Mobile Habit Formation

---

### 10. Push Notification Behavior

**Stothart, C., Mitchum, A., & Yehnert, C. (2015). "The Attentional Cost of Receiving a Cell Phone Notification." Journal of Experimental Psychology: Human Perception and Performance, 41(5), 1193-1202.**
- **Layer:** 4 (Motivation) -- also Layer 2 (Cognition)
- **Key finding:** Just *receiving* a cell phone notification -- even without actively checking it -- significantly disrupts attention and task performance. The mere notification triggers an involuntary attentional shift. This is separate from the "mere presence" effect (finding #7); this is an *active interruption* effect.
- **NEW vs APPLIED:** **Genuinely new (mobile-specific motivational/attentional phenomenon).** Push notifications are a mobile-unique engagement channel with no desktop equivalent. The finding that a *single notification disrupts cognitive processing for approximately 7 seconds* (replicated in later studies in *Computers in Human Behavior*) is a quantified mobile-specific cost. This creates a fundamental tension: the primary engagement tool for mobile (push notifications) inherently damages the cognitive state it's trying to leverage.

**PMC (2023). "How Notifications Affect Engagement With a Behavior Change App."**
- **Layer:** 4 (Motivation)
- **Key finding:** Push notifications can increase engagement with behavior change apps, but effectiveness depends on timing, personalization, and frequency. Over-notification leads to notification fatigue and disengagement.
- **NEW vs APPLIED:** **Partially new.** While the principle of "moderate prompting works, excessive prompting fails" applies broadly, the *push notification as the primary behavioral prompt mechanism* is mobile-specific. The 7-second attentional cost creates a unique trade-off: each notification both engages AND degrades the cognitive state.

**ResearchGate (2021). "Mobile Apps in Retail: Effect of Push Notification Frequency on App User Behavior."**
- **Layer:** 4 (Motivation)
- **Key finding:** Investigates how different push notification frequencies affect behavior in retail apps. Higher frequency increases short-term engagement but decreases long-term retention and increases opt-out rates. There is an inverted-U relationship between notification frequency and lifetime engagement.
- **NEW vs APPLIED:** **Applied (inverted-U principle / habituation).** The finding is consistent with general habituation principles. However, the *push notification as the mechanism* and the specific quantitative thresholds for mobile are mobile-unique.

---

### 11. Mobile Habit Formation Specifics

**Verplanken, P. & Orbell, S. (2003). "Reflections on Self-Regulation and Habit." (applied to mobile)**
- **Layer:** 4 (Motivation)
- **Context:** While the original research is general habit theory, the application to mobile has generated mobile-specific findings. Mobile habits are typically *shorter duration, higher frequency* than desktop habits. Checking a mobile app is typically a 30-60 second behavior, compared to desktop sessions of 10+ minutes.
- **NEW vs APPLIED:** **Partially new.** The *shorter, more frequent habit pattern* is mobile-specific, driven by the device's portability and always-available nature. The habit loop (cue-routine-reward) operates the same way, but the *temporal pattern* of mobile habits is qualitatively different.

**Oulasvirta, A., Rattenbury, T., Ma, L., & Raita, E. (2012). "Habits Make Smartphone Use More Pervasive." Personal and Ubiquitous Computing, 16(1), 105-114.**
- **Layer:** 4 (Motivation)
- **Key finding:** Found that smartphone habits -- not conscious intention -- are the primary predictor of smartphone use. The more habitual the checking behavior, the less it is associated with the user's conscious goals. Habits make use more automatic and frequent, creating a "check addiction" pattern.
- **NEW vs APPLIED:** **Genuinely new (mobile-specific finding).** The finding that *habit strength overrides conscious intention specifically for smartphone use* is a mobile-unique behavioral finding. This explains why users check their phones 150+ times per day -- it's not that each check serves a goal; it's that the habit has become self-sustaining. The always-available, always-carried nature of smartphones makes them uniquely susceptible to compulsive habit formation in ways that desktop computers are not.

---

### 12. App vs Web Behavioral Differences

**ScienceDirect (2024). "Choose a Mobile Application or Mobile Website? Different Effects on Consumer Behavior."**
- **Layer:** 4 (Motivation)
- **Key finding:** Mobile apps create stronger engagement, higher conversion rates (up to 157% higher than mobile web per BYYD research), and deeper sessions. ~90% of mobile time is spent in apps. The installation barrier creates a self-selection effect: users who install an app have higher intent.
- **NEW vs APPLIED:** **Partially new.** The finding that the *same brand, same user, same content* produces different behavior based on whether it's in an app or browser is a mobile-specific "container effect." The installation friction creates a commitment/consistency effect that filters for higher-intent users, and the app environment (push notifications, home screen presence, persistent login) creates a fundamentally different engagement context than mobile web.

**ResearchGate (2020). "Advertising on Mobile Apps Versus the Mobile Web: Which Delivers Better Advertisement Recognition and Willingness to Buy."**
- **Layer:** 4 (Motivation)
- **Key finding:** Branded apps led to higher advertisement recognition and greater willingness to buy new products compared to mobile websites. Cognitive and behavioral antecedents differed between the two platforms.
- **NEW vs APPLIED:** **Partially new.** The app environment creates higher cognitive engagement and trust, leading to different behavioral outcomes. This is a mobile-specific "context" effect.

---

## LAYER 5 -- Product Behavior: Mobile Onboarding, Mobile Retention, Mobile Conversion Optimization

---

### 13. Mobile Onboarding

**Nielsen Norman Group (2020). "Mobile-App Onboarding: An Analysis of Components and Techniques."**
- **Layer:** 5 (Product Behavior)
- **Key finding:** Breaks mobile onboarding into three components: benefit communication (why to use), education (how to use), and account creation. The key mobile-specific finding is that mobile onboarding has **less screen real estate per step**, forcing more steps for the same content. Mobile users also have **lower tolerance for onboarding friction** -- up to 80% of users abandon apps during onboarding if the experience is poor (DesignerUp, 2024 study of 200+ onboarding flows).
- **NEW vs APPLIED:** **Partially new.** The general onboarding principles (reduce friction, show value fast) apply broadly. However, the *space constraint forcing more sequential steps* and the *lower friction tolerance on mobile* are mobile-specific. Mobile users have alternative apps literally one tap away (app store), making abandonment cost lower than desktop where switching is more effortful.

**Specific mobile onboarding challenge:** Permission requests on mobile are a mobile-unique onboarding barrier. Asking for camera, location, or notification permissions before the user understands why creates reflexive denial. On desktop, most permissions are granted implicitly or are less granular. This is a mobile-specific onboarding anti-pattern.

---

### 14. Mobile Retention

**App industry benchmarks (2024-2026):**
- D1 retention: 40-60% (consumer apps), 70-80% (SaaS)
- D7 retention: 20-30% (consumer), 50-60% (SaaS)
- D30 retention: 10-15% (consumer), 30-40% (SaaS)
- **Layer:** 5 (Product Behavior)
- **Context:** These benchmarks are mobile-specific because the *retention drivers* differ on mobile. Home screen presence, push notification re-engagement, and widget visibility are mobile-specific retention mechanisms with no desktop equivalent. The home screen is "free advertising space" -- every time the user sees the app icon, it's a re-engagement touchpoint that doesn't exist for desktop software.

---

### 15. Mobile Conversion Optimization

**DRIP (2026). "Mobile vs Desktop Conversion Rates: 117-Brand Data."**
- **Layer:** 5 (Product Behavior)
- **Key finding:** Across 117 European e-commerce brands and 486 million sessions, desktop converts at 3.93% median while mobile converts at 2.46%. The gap is driven by mobile-specific friction: form completion difficulty with thumbs, smaller product images, security concerns with mobile payment methods, and contextual factors (on-the-go, distracted).
- **NEW vs APPLIED:** **Applied with mobile-specific interventions.** Conversion optimization principles are general. But the *specific interventions* needed are mobile-unique: thumb-friendly form layouts, larger touch targets, simplified checkout flows, Apple Pay/Google Pay integration (which are mobile-only), and context-aware design (fewer fields when the user is likely walking/transit).

---

## CROSS-LAYER: Mobile Context of Use

---

### 16. Mobile as a Divided-Attention Context

**ResearchGate (2011). "Investigating Selection and Reading Performance on a Mobile Phone While Walking."**
- **Layer:** 2 (Cognition) / 5 (Product Behavior)
- **Key finding:** Walking while using a mobile phone significantly degrades both reading comprehension and target selection accuracy compared to stationary use. This is not a small effect -- performance drops are substantial.
- **NEW vs APPLIED:** **Genuinely new (mobile-specific).** The finding that *a significant portion of mobile use occurs in a divided-attention context* (walking, transit, social situations) and that this fundamentally degrades cognitive performance is a mobile-unique principle. Desktop use is overwhelmingly stationary and focused; mobile use is frequently not. This means mobile UIs must be designed for *degraded cognitive states* as the baseline, not as an edge case.

**Whiterose eprints. "The Effects of Simulated Interruptions on Mobile Search Tasks." JASIST.**
- **Layer:** 2 (Cognition) / 3 (Decision Making)
- **Key finding:** Investigated the ambient distraction of walking while using a mobile device combined with simulated interruptions (notifications). The two sources of divided attention (environmental + digital) compound, creating a multiplicative (not additive) degradation of task performance.
- **NEW vs APPLIED:** **Genuinely new.** The compounding effect of environmental + digital distraction is a mobile-specific phenomenon. Desktop users rarely face this combination; mobile users routinely do.

**PMC (2024). "What's That on Your Phone? Effects of Mobile Device Task Type on Pedestrian Safety."**
- **Layer:** 4 (Motivation) / Context
- **Key finding:** Multitasking with a mobile device negatively impacts pedestrian safety regardless of task type. This documents the real-world consequences of mobile divided attention.
- **NEW vs APPLIED:** **New contextual finding.** Confirms that mobile use often occurs in contexts where the user's attention is split between the device and the physical environment.

---

### 17. Understanding In-Context Mobile Interaction

**ScienceDirect (2019). "Understanding In-Context Interaction: An Investigation into On-the-Go Usage."**
- **Layer:** 1 (Perception) / 2 (Cognition)
- **Key finding:** Investigated how physical context (walking, grip shifts, environmental factors) affects mobile interaction. Found that mobile users frequently shift grip and adjust their physical relationship to the device during use, affecting both accuracy and reading behavior.
- **NEW vs APPLIED:** **Genuinely new.** Grip shifts during use are a mobile-specific physical behavior with no desktop analog. The finding that users' physical posture changes *during* an interaction session (not just between sessions) affects UI design implications -- elements must be robust to changing grip types mid-interaction.

---

## Summary: What Is Genuinely Mobile-Unique vs. Applied?

### Genuinely Mobile-Unique Principles (True on Mobile, NOT True on Desktop)

| # | Principle | Layer | Why It's Mobile-Unique |
|---|---|---|---|
| 1 | **Thumb zone heat maps** -- natural, stretch, awkward zones based on grip type | 1 | No desktop analog; depends on hand-device physical relationship |
| 2 | **Screen size as natural progressive disclosure** -- smaller screen limits content, paradoxically reducing extraneous cognitive load | 2 | Counterintuitive; only applies when viewport constrains visible content |
| 3 | **Smartphone "mere presence" brain drain** -- phone nearby reduces cognitive capacity even when off | 2 | Desktop computers nearby do not produce this effect |
| 4 | **Adaptive reading strategy shift** -- users strategically skim on mobile, deep read on desktop, even for identical content | 2 | Not about ability but about strategic adaptation to device |
| 5 | **Micro-moments** -- decision journey fragments into intent-rich, impatient micro-decisions | 3 | Driven by always-carried, always-on device; no desktop equivalent |
| 6 | **7-second notification attentional cost** -- single notification derails focus even if ignored | 4 | Push notifications are a mobile-only engagement channel |
| 7 | **Habit override** -- habit strength, not intention, predicts smartphone use; creates compulsive checking | 4 | Always-carried nature enables unique compulsive habit formation |
| 8 | **App vs web container effect** -- same content produces different behavior based on app vs browser | 4 | Installation friction + push notifications create fundamentally different engagement contexts |
| 9 | **Divided attention as baseline** -- mobile use frequently occurs while walking, in transit, or in social situations | Cross-layer | Desktop use is predominantly stationary and focused |
| 10 | **Grip shift during interaction** -- users change physical relationship to device mid-session | 1 | No desktop analog; affects accuracy and UI requirements |
| 11 | **FFitts finger occlusion correction** -- users touch below where they think they're touching due to finger anatomy | 1 | No cursor to bridge gap; only applies to direct-touch interfaces |
| 12 | **Dark mode economic incentive** -- OLED battery savings create rational reason for dark mode preference | 1 | LCD desktop monitors don't have this property |
| 13 | **Lower abandonment cost on mobile** -- alternative apps are one tap away (app store) | 5 | Desktop software switching requires more deliberate effort |

### Applied Principles (Existing General Principles Applied to Mobile)

| Principle | Original Source | Mobile Application |
|---|---|---|
| Fitts's Law | Fitts (1954) | Touch targets, thumb reachability, target sizing |
| Cognitive Load Theory (split-attention) | Sweller (1988) | Mobile UI layouts, scrolling between related content |
| F-pattern scanning | Nielsen (2006) | Compressed on mobile but persists |
| Hick's Law | Hick (1952) | Fewer visible options on mobile reduces effective choice count |
| Inverted-U (optimal stimulation) | General psychology | Push notification frequency optimization |
| Habit loop (cue-routine-reward) | Duhigg (2012) | Mobile habit formation, push notification triggers |
| Loss aversion / conversion | Kahneman & Tversky (1979) | Mobile checkout optimization |
| Onboarding best practices | General UX | Mobile onboarding with space constraints |
| Goal-gradient effect | Hull (1932) | Mobile progress indicators, setup completion |

---

## Key Gaps in the Research

Areas where mobile-unique research is thin or missing:

1. **Mobile-specific choice architecture** -- Most choice architecture research (decoy effect, compromise effect, default effects) has been tested on desktop. Very few studies replicate these on mobile with mobile-specific layouts. We don't know if the decoy effect works differently in a single-column mobile layout vs. a three-column desktop layout.

2. **Mobile color psychology on OLED** -- Color psychology research (Elliot & Maier, 2014) is device-agnostic. Very little research examines whether OLED color reproduction differences (deeper blacks, more saturated colors) change color-behavior relationships on mobile.

3. **Mobile social proof differences** -- Does social proof work differently on mobile where social information is viewed through a smaller, more personal viewport? Unknown.

4. **Mobile temporal discounting** -- Does hyperbolic discounting operate differently when the device itself enables immediate action? A user on mobile can act on impulse immediately (one tap to buy), while desktop may introduce more friction. This could amplify temporal discounting on mobile, but research is lacking.

5. **Mobile endowment effect** -- Does the intimate, always-carried relationship with a phone amplify endowment effects for mobile apps? Anecdotally, users treat "their apps" differently than "their websites," but research quantifying this is scarce.
