# Generation Prompts Reference

Output formats and domain guidance for each pipeline stage.

## Table of Contents
- [Stage 1: Idea Generation](#stage-1-idea-generation)
- [Stage 2: Personas](#stage-2-personas)
- [Stage 3: Pitch](#stage-3-pitch)
- [Stage 4: Avatar](#stage-4-avatar)
- [Stage 5: Diary](#stage-5-diary)
- [Stage 6: Features](#stage-6-features)
- [Stage 7: Pricing](#stage-7-pricing)
- [Stage 8: Landing Page Outline](#stage-8-landing-page-outline)

---

## Stage 1: Idea Generation

Act as an innovation strategist and lean startup expert. Generate **4 business concepts** feasible for a small team or single founder.

### Constraints per idea
- **Single Founder Feasibility:** Achievable end-to-end by one skilled founder using AI tools, APIs, and lightweight frameworks.
- **Problem Profile:** A thorn-in-the-side problem -- simple, frequent, annoying enough that users will pay to eliminate it.
- **Solution Form:** A focused tool (web or mobile) that does one thing extremely well. Minimal feature creep.
- **Revenue Model:** Match the user's preference. If none stated, default to transactional/pay-per-value (each interaction = one payment for a clear deliverable). Subscriptions, freemium, and ad models are valid if the user prefers them.
- **Target Market:** Prefer underserved niches -- professionals, artisans, freelancers, creators, micro-businesses.

### Adapting to user input
- If the user specifies a domain/focus, all 4 ideas must target that space.
- If the user says "surprise me" or gives no focus, generate diverse ideas across different niches.
- If the user specifies a business model (subscription, marketplace, etc.), honor it.

### Output format per idea

```
**Idea #X: [Creative Tool Name]**
- **Target Vertical:** [Niche audience segment]
- **Specific Problem:** [What annoying issue they face regularly]
- **Solution and Value Proposition:** [How the tool solves it]
- **Proposed Transaction:** [Revenue action + suggested price point]
```

### Calibration example

**Idea #1: KDP NicheFinder**
- **Target Vertical:** Independent authors on Amazon KDP
- **Specific Problem:** Choosing the best categories and keywords for book discoverability is confusing and time-consuming.
- **Solution and Value Proposition:** Author pastes their book description; the tool uses AI to suggest top categories and high-potential keywords.
- **Proposed Transaction:** Pay $25 for one optimized category + keyword set.

---

## Stage 2: Personas

Define exactly 2 target-audience personas for the selected idea: Primary and Secondary.

### Output format per persona

```
**[Primary/Secondary] Persona: [Name] ("[Nickname]")**
- **Age:** [integer]
- **Role/Segment:** [job title or segment description]
- **Income/Budget:** [with currency, /yr where relevant]
- **Adoption & Engagement:**
  - Tier: [New | Exploring | Active | Power | Champion]
  - Metrics: [domain-appropriate metrics, e.g. sessions/wk, transactions/mo]
- **Pain Points:**
  - [pain 1]
  - [pain 2]
  - [pain 3]
- **Goals:**
  - [goal 1]
  - [goal 2]
  - [goal 3]
- **Tech/Data Comfort:**
  - Level: [Very Low | Low | Medium | High | Very High]
  - Tools: [tools they use]
- **Currency:** [preferred currency]
```

### Guidelines
- Infer plausible specifics from context. Avoid hedging ("about," "maybe," "~").
- Adoption tiers: New, Exploring, Active, Power, Champion.
- Metrics must fit the domain (DAU/sessions for consumer; seats/WAU for B2B SaaS; transactions/mo for fintech; patients/day for HCLS).
- Make the two personas meaningfully different (different needs, budgets, tech comfort).

---

## Stage 3: Pitch

Create 4 components from the idea + personas:

### Output format

```
**Elevator Pitch**
[1-2 sentences summarizing the product and its value]

**Problem Statement**
[2-3 sentences describing the pain the target personas face]

**Target Audience**
- Primary: [persona name and segment]
- Secondary: [persona name and segment]

**Unique Selling Proposition**
[1-2 sentences on what makes this solution uniquely compelling]
```

---

## Stage 4: Avatar (A-H Framework)

Build one detailed problem-aware customer avatar based on Eugene Schwartz's Problem Aware stage. The avatar clearly recognizes their problem but does not yet connect to solutions.

### Output format

Present each section with its letter prefix:

```
**A -- Who Are They**
- Name:
- Gender:
- Job:
- Household Income:
- Marital Status:
- Education Level:

**B -- What They Do & Like**
- Top 3 Brands they wear:
- 1-2 Hobbies:
- Top 5 Favorite movies:
- Top 5 Favorite books:
- Top 5 Visited websites:
- Top 5 Relevant social media influencers:

**C -- Why Are They**
- Main Personality Traits:
- 5 Major Values:
- 2 Major Life Victories:
- 2 Major Life Failures:

**D -- Smart Market Questions**
- What keeps them awake at night:
- What are they secretly afraid of:
- What are they angry about, and who at:
- Top 3 daily frustrations:
- Biggest secret desire:
- Built-in decision bias:
- Common words/language unique to them:
- Top 3 complaints about existing solutions:

**E -- Going Deep**
- Top 3 Dominant Negative Emotions:
- Top 3 Dominant Positive Emotions From Solving This Problem:
- Top 3 Beliefs About The World:
- Biggest Lifestyle Desire:

**F -- Purchasing Habits**
- Top 3 Decision Triggers:
- Prior Purchases For This Pain:
- Price Tolerance:
- Time Horizon Of Solution:

**G -- Primary Wants**
- Wants to gain:
- Wants to be:
- Wants to do:
- Wants to save:
- Wants to avoid:

**H -- Empathy Map**
- Seeing:
- Thinking:
- Hearing:
- Feeling:
- Saying:
- Doing:
```

### Guidelines
- Draw from the personas and idea context. Make details concrete and plausible.
- Don't take the avatar's job too literally -- it illustrates the type of person.
- Populate every field. No blanks, no "N/A."

---

## Stage 5: Diary

Transform the avatar into a short first-person diary entry.

### Constraints
- **Length:** 140-220 words
- **POV:** First-person, present tense (default)
- **Emotional intensity:** High (4/5 default)
- **Voice:** Natural, avatar-true; allow slang/code-switching

### Required texture (include all)
- A time + place opener ("11:38 p.m., kitchen light humming")
- One social friction moment (terse chat, ignored text)
- One body sensation tied to stress ("jaw clicking," "cold palms")
- One coping habit (doomscroll, spreadsheets, late-night cleaning)
- One concrete object in the scene (receipt, cracked mug, train ad)

### Mapping guide (avatar section -> diary content)
- A (Who): Voice, register, micro-details (workday rhythm, living space)
- B (Do/Like): Texture only (brands/sites as passing scenery, not endorsements)
- C (Why): Moral tone and self-talk patterns
- D (Market Qs): Rumination content; include short quoted inner thoughts
- E (Deep): Dominant negative emotions lead; small "hope flicker" allowed
- F (Purchases): Decision bias as inner rules ("if it's not proven...")
- G (Wants): Subtext and ache beneath the rant
- H (Empathy Map): Sensory field -- what they see/hear/feel right now

### Hard rules
- No solutions, products, advice, or brand pitching
- No headings, labels, analysis, or commentary
- Output only the diary text

---

## Stage 6: Features

Produce avatar-aligned features from the idea + avatar.

### Process
1. Identify core jobs-to-be-done, user flows, and constraints from the idea
2. Map avatar sections to feature hooks:
   - A (Who) -> access/onboarding needs
   - C (Why) -> control, simplicity, mastery features
   - D (Frustrations) -> friction-killers, clarity, feedback loops
   - E (Emotions) -> privacy, reversibility, low-stakes preview
   - F (Purchasing) -> trials, transparent limits, milestones
   - G (Wants) -> progress signals, quick wins, checkpoints
   - H (Empathy Map) -> timely nudges, offline modes, noise-proof UX

### Output format
Markdown bullet list only. Each bullet:
```
- **[Feature Name]** -- [benefit-focused clause, max 12 words]
```

No headings, numbers, emojis, or extra commentary. Just the list.

### Quality checks
- Every feature is avatar-relevant and application-faithful
- Mix covers friction reduction, confidence building, and quick wins
- No duplicate ideas; each bullet is concrete and shippable

---

## Stage 7: Pricing

### KISS rules
- **One pricing model only.** Subscription OR Transactional OR Pay-per-value.
- **One value metric only.** Obvious and measurable.
- **Max 3 tiers** (recommend 2). Plain names. Rounded prices.
- **No add-ons.** One simple overage rule if needed.
- **No jargon, no hidden fees, no complex fences.**
- **Model consistency:** Honor the idea's stated or implied model. If the idea favors transactional, use transactional. Only use subscription when it clearly fits.

### Output format

```
## Pricing Model
[Subscription | Transactional | Pay-per-value] -- [one-line reason]

## Value Metric
[Single metric] -- [how it scales with value]

## Packages & Prices

- **[Tier Name]**
  - Price: [amount] (billing period)
  - Includes:
    - [quota/feature 1]
    - [quota/feature 2]
    - [quota/feature 3]
  - Limit/Overage: [single clear rule]

- **[Tier Name]**
  - Price: [amount] (billing period)
  - Includes:
    - [quota/feature 1]
    - [quota/feature 2]
    - [quota/feature 3]
  - Limit/Overage: [single clear rule]

## Terms
- Trial/Guarantee: [e.g., 14-day trial or 30-day refund]
- Billing: [card/invoice] | Annual discount: [e.g., -15%] (optional)
```

### Guidelines
- Prices must match avatar's price tolerance and time horizon (from section F)
- Clear upgrade path without complexity

---

## Stage 8: Landing Page Outline

CRO-focused, benefit-first landing page outline using all prior context.

### Operating principles
- Benefit-first: lead with pains/outcomes; features follow as proof
- Plain language; max 12-word bullets where possible
- One primary action per section

### Output format per section

```
## [Section Name] -- Component: [UI component type]

- **Headline:** [benefit-first promise in avatar language]
- **Subhead:** [concise outcome expansion]
- **Avatar Pains -> Outcomes:**
  - [Pain] -> [Tangible outcome]
  - [Pain] -> [Tangible outcome]
  - [Pain] -> [Tangible outcome]
- **Feature Proof (2-3):**
  - [Feature] -- [specific proof/metric]
  - [Feature] -- [specific proof/metric]
- **Social Proof / Risk Reducer:**
  - [logo/testimonial/stat or trial/refund note]
- **Primary CTA:** [verb + outcome]
- **Secondary CTA (optional):** [lower-commitment action]
```

### Required sections
1. Hero
2. Problem Agitation
3. Outcome / Value Pillars
4. Feature Proof
5. Social Proof
6. How It Works
7. Pricing (KISS)
8. FAQ / Objections
9. CTA Finale
10. Footer
