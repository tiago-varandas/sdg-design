---
version: alpha
name: SDG.design — 13 Climate Action
description: Design system for SDG 13 — Climate Action. Two variants: a community climate tracker and a campaign and advocacy platform. Urgent, hopeful, purposeful.

colors:
  primary: "#0D1F0F"
  secondary: "#1E4D24"
  tertiary: "#74C478"
  background: "#F4FAF4"
  surface: "#FFFFFF"
  surface-subtle: "#EAF2EB"
  accent: "#3F7E44"
  accent-light: "#56A85C"
  accent-bright: "#C8F060"
  neutral: "#3A4A3C"
  earth: "#8B6914"
  earth-soft: "#F5F0E8"
  urgent: "#C53030"
  urgent-soft: "#FDECEA"

typography:
  display:
    fontFamily: "Helvetica Neue"
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.0
    letterSpacing: -0.04em
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.035em
  title:
    fontFamily: "Helvetica Neue"
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  body:
    fontFamily: "Helvetica Neue"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: -0.01em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.05em
  data-large:
    fontFamily: "JetBrains Mono"
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.0
    letterSpacing: -0.03em
  data-small:
    fontFamily: "JetBrains Mono"
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em

rounded:
  sm: 4px
  md: 8px
  lg: 12px
  xl: 20px
  full: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  2xl: 80px
  3xl: 128px

components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: 22px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-bright:
    backgroundColor: "{colors.accent-bright}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    padding: 22px
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 22px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-earth:
    backgroundColor: "{colors.earth-soft}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-urgent:
    backgroundColor: "{colors.urgent-soft}"
    rounded: "{rounded.lg}"
    padding: 20px
  card-data:
    backgroundColor: "{colors.surface-subtle}"
    rounded: "{rounded.lg}"
    padding: 20px
  pledge-card:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.xl}"
    padding: 28px
  tag-action:
    backgroundColor: "{colors.surface-subtle}"
    textColor: "{colors.accent}"
    rounded: "{rounded.full}"
    padding: 8px
  tag-urgent:
    backgroundColor: "{colors.urgent-soft}"
    textColor: "{colors.urgent}"
    rounded: "{rounded.full}"
    padding: 8px
  nav:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.neutral}"
    padding: 16px
---

# SDG.design — 13 Climate Action

## Overview

SDG 13 calls for urgent action to combat climate change and its impacts. Design for this goal must hold two emotional registers simultaneously — the urgency of a crisis and the hope of collective action. It should never induce paralysis through despair, and never minimise the scale of the challenge through false optimism.

This system serves two builder contexts. The first is community climate trackers — apps for individuals, households, and local communities to measure, visualise, and reduce their climate impact. These prioritise personal agency and collective momentum. The second is campaign and advocacy platforms — tools for NGOs, activists, and civic organisations to communicate climate data, mobilise action, and hold institutions accountable.

The community variant keeps data human-scale — your household's impact, your neighbourhood's progress, your personal actions. Abstract global statistics cause disengagement. Concrete local data drives behaviour change.

The advocacy variant uses larger, bolder data presentation — designed to be read on shared screens, embedded in presentations, and shared on social media. Numbers must be legible at distance and in screenshot form.

The palette is rooted in deep forest — serious, grounded, alive. The bright lime accent (`accent-bright`) is used sparingly for breakthrough moments — achieved pledges, exceeded targets, decisive actions. It is the color of something happening.

## Colors

Deep forest greens with a single electric lime for breakthrough moments. Earth tones for context and warmth.

- **Primary (#0D1F0F):** Near-black forest. Headlines and primary text. The weight of the problem.
- **Secondary (#1E4D24):** Deep forest. Section headers, active states.
- **Tertiary (#74C478):** Mid green. Chart fills, decorative accents.
- **Background (#F4FAF4):** Living white. The lightest possible green tint.
- **Surface (#FFFFFF):** Cards and panels.
- **Surface Subtle (#EAF2EB):** Data card backgrounds, input fields.
- **Accent (#3F7E44):** Forest green. Primary CTAs, active states, progress fills.
- **Accent Light (#56A85C):** Hover state for primary accent.
- **Accent Bright (#C8F060):** Electric lime. Used only for achieved states, completed pledges, breakthrough data moments. Maximum two appearances per screen.
- **Neutral (#3A4A3C):** Warm forest grey. Body text.
- **Earth (#8B6914):** Warm ochre. Used for land and soil data contexts, historical comparisons.
- **Earth Soft (#F5F0E8):** Background for earth/land content cards.
- **Urgent (#C53030):** Used only for genuinely critical thresholds — 1.5°C breach indicators, emergency alerts. Never decoratively.

## Typography

The `display` scale (72px) is unique to SDG 13 in this kit — climate advocacy requires headline numbers that command attention at scale. "1.5°C" or "2030" set at display size with tight tracking has genuine visual power.

`data-large` (48px Inter Mono) is for the primary metric on any screen — tonnes of CO₂, percentage above target, days until deadline. Monospace ensures alignment across changing values.

`data-small` (20px Inter Mono) handles supporting data — comparison values, trend figures, secondary metrics.

## Layout

**Community tracker variant:** Personal home screen with a single primary metric (your estimated monthly carbon footprint), one suggested action, and a neighbourhood progress bar. Depth available through exploration — never forced upfront.

**Advocacy variant:** Full-bleed data sections. Each section leads with a large number or chart, supported by two to three sentences of context. Designed for scrolling narratives — the layout tells a story, not just displays data. Social share built into every section.

The `3xl` spacing value (128px) is used between major sections in the advocacy variant — breathing room gives data weight.

## Elevation & Depth

The dark pledge card (primary background, white text) is the single moment of high contrast in an otherwise light layout. It creates a visual anchor — this is where commitment is made. Use once per screen maximum.

Data cards use surface-subtle fills. Urgent cards use urgent-soft fill — visible but not alarming.

## Shapes

Standard 12px for most elements. Pledge and commitment cards use `xl` (20px) — the softness of the shape counterbalances the weight of the commitment. Full radius for all buttons, tags, and pills.

## Components

**Impact Meter:** The central component of the community variant. A circular or bar visualisation of personal/household carbon footprint vs. the 2030 target. Color transitions from accent-bright (below target) through accent (at target) to urgent (above target).

**Action Card:** Single climate action. Title, estimated CO₂ saving (data-small), difficulty indicator, "Take action" button. Designed to be dismissible — users should never feel guilted, only invited.

**Pledge Card:** Dark background (primary). Pledge text in white title scale. Signatory count. Accent-bright CTA button. The single highest-contrast element in the system.

**Data Story Section:** Advocacy variant. Full-width. Large number (display or data-large scale), two-line context, source label (label scale), share button. Repeatable pattern for scrolling advocacy pages.

**Progress Collective:** Neighbourhood or cohort progress bar. Shows individual contribution within a larger group bar. Accent fill for the user's contribution, tertiary for others. Label shows total collective impact.

**Alert Threshold:** Used only for genuinely critical data points. Urgent-soft background, urgent text, exclamation icon. Reserved for threshold breaches — never for routine data.

## Do's and Don'ts

- Do lead with agency and action — every screen should offer something the user can do right now
- Do use accent-bright only for achieved states and positive breakthroughs — it must feel earned
- Don't show global catastrophe statistics without an immediately actionable response
- Do make data shareable by design — social spread of climate facts is a core campaign mechanic
- Don't use urgent red for anything other than genuine critical threshold alerts
- Do show collective impact alongside individual — "You + 847 neighbours have saved 12 tonnes this month"
- Don't use the display typography scale for anything other than the single most important number on screen
- Do design for emotional sustainability — users who feel despair disengage. Hope is a design requirement.
- Don't hide the data source — credibility is everything in climate advocacy

## The Despair Trap

Climate communication has a design problem that kills engagement: it tells people the truth about the scale of the crisis and then offers them actions that feel laughably insufficient. "The planet is heating catastrophically. You can save it by using a reusable bag." This mismatch is a design failure that produces paralysis, not action.

**Scale actions to match the emotional weight of the data.** If you show a user that global emissions are 37 billion tonnes, the suggested action cannot be "turn off the lights." Either contextualise the data at a human scale ("your city's share") or contextualise the action at a systems scale ("join 847 people pushing your city council for a clean energy mandate"). The data scale and the action scale must match.

**The 57% rule:** Research on climate communication shows that 57% of people believe they are more concerned about climate change than their neighbours. This means most people self-censor their climate concern to avoid seeming abnormal. Design should make collective concern visible: show how many people in a user's neighbourhood have taken the same action. Social normalisation of climate action is more effective than individual guilt.

**Never show a countdown to catastrophe without a pathway.** Doomsday clocks, "days until 1.5°C" counters, and catastrophe timers increase anxiety and decrease action in most user segments. If you show urgency data, it must be immediately followed by a specific, achievable action with a visible impact number. Urgency without agency is paralysis by design.

**Celebrate systemic wins as loudly as personal ones.** A user who convinced their employer to switch to renewable energy has done more than a user who stopped eating meat for a month. Design the achievement system to recognise advocacy, collective action, and systemic change — not just personal consumption changes. Individual behaviour change without systemic change is insufficient; the design system should reflect this.
