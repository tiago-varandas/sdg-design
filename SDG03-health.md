---
version: alpha
name: SDG.design — 03 Good Health
description: Design system for SDG 3 — Good Health and Wellbeing. Two variants: a community health worker tool and a patient-facing wellness platform. Warm, trustworthy, calm.

colors:
  primary: "#1A3A2A"
  secondary: "#2D6A4F"
  tertiary: "#74C69D"
  background: "#F4FAF6"
  surface: "#FFFFFF"
  surface-subtle: "#EAF5EF"
  accent: "#4C9B47"
  accent-warm: "#E8F5E2"
  neutral: "#4A5568"
  warm: "#F9F3EE"
  success: "#2E9E6B"
  warning: "#D4860A"
  error: "#C53030"

typography:
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.025em
  title:
    fontFamily: "Helvetica Neue"
    fontSize: 19px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.015em
  body:
    fontFamily: "Helvetica Neue"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
    letterSpacing: -0.01em
  body-small:
    fontFamily: "Helvetica Neue"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: -0.01em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.04em
  metric:
    fontFamily: "Helvetica Neue"
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.0
    letterSpacing: -0.03em

rounded:
  sm: 6px
  md: 10px
  lg: 16px
  xl: 24px
  full: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  2xl: 80px

components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: 20px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-soft:
    backgroundColor: "{colors.accent-warm}"
    textColor: "{colors.accent}"
    rounded: "{rounded.full}"
    padding: 20px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-warm:
    backgroundColor: "{colors.warm}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-metric:
    backgroundColor: "{colors.surface-subtle}"
    rounded: "{rounded.lg}"
    padding: 20px
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.md}"
    padding: 16px
  tag-category:
    backgroundColor: "{colors.surface-subtle}"
    textColor: "{colors.secondary}"
    rounded: "{rounded.full}"
    padding: 8px
  nav:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.neutral}"
    padding: 16px
---

# SDG.design — 03 Good Health

## Overview

SDG 3 calls for healthy lives and wellbeing for all ages. Design for this goal must be warm, human, and deeply trustworthy. Healthcare experiences are often anxious — the design system's primary job is to reduce that anxiety and create calm confidence.

This system serves two builder contexts. The first is community health worker tools — apps used by frontline health workers in clinics, homes, and community settings. These prioritise speed, clarity, and offline reliability. The second is patient-facing wellness platforms — consumer-facing apps for individuals managing their own health, seeking support, or accessing services.

Both variants share the same foundational warmth but differ in information density and interaction style. Health worker tools are task-oriented and efficient — a worker needs to log a visit, record vitals, and flag a referral in under three minutes. Patient platforms are more nurturing and conversational — they meet people in moments of vulnerability and must feel like a trusted friend.

The palette is grounded in forest green — natural, living, growing. This is health as vitality, not health as clinical sterility. The warm background and generous spacing create breathing room. Nothing should feel rushed or crowded.

## Colors

Forest greens anchored in warmth, deliberately avoiding the cold clinical blues of traditional healthcare.

- **Primary (#1A3A2A):** Deep forest. Headlines, primary text. Signals depth and calm authority.
- **Secondary (#2D6A4F):** Mid forest. Section headers, active navigation, link text.
- **Tertiary (#74C69D):** Sage. Chart fills, decorative accents, secondary data.
- **Background (#F4FAF6):** Barely-green white. The page breathes with subtle life.
- **Surface (#FFFFFF):** Card backgrounds. Clean, clinical-free white.
- **Surface Subtle (#EAF5EF):** Input backgrounds, recessed panels, metric cards.
- **Accent (#4C9B47):** Forest green. Primary CTAs and interactive highlights.
- **Accent Warm (#E8F5E2):** Soft green tint. Button hover backgrounds, success states.
- **Neutral (#4A5568):** Body text. Warm grey — never cold.
- **Warm (#F9F3EE):** Cream. Used for supportive, conversational card contexts.
- **Success/Warning/Error:** Standard semantic colors. Used sparingly.

## Typography

Body text at 16px with 1.75 line height — unusually generous, but essential for health contexts where comprehension is critical and stress reduces reading ability.

Headlines are warmer and less tightly tracked than SDG 13 or SDG 16 — this is not urgency, it is reassurance. The rounded `lg` and `xl` radius scales reinforce this emotional direction.

The `metric` scale (32px, weight 500) is used for health indicators — step counts, medication adherence rates, visit completion — displayed prominently on dashboards.

## Layout

**Health worker variant:** Compact, task-focused. Every screen has one primary action. Patient list → patient record → action flow. Navigation is top-bar, minimal. Forms are single-column, one question at a time where possible to reduce cognitive load under pressure.

**Patient platform variant:** Generous whitespace, card-based. Home screen shows today's focus — one health goal, one pending action, one supportive message. Bottom navigation with five items max. Onboarding is conversational, not form-based.

Both variants must support text scaling up to 200% for accessibility without breaking layout.

## Elevation & Depth

Warmth comes from background tint contrast and card fills, not shadows. The `warm` cream surface is used for content that should feel nurturing — peer support messages, encouraging progress notes, wellbeing check-ins.

Metric cards use `surface-subtle` to distinguish data from narrative content. No drop shadows.

## Shapes

More rounded than most SDG systems — `lg` at 16px, `xl` at 24px. The roundedness signals safety and approachability. This matters especially for patient-facing tools where sharp corners can trigger subtle associations with clinical environments.

## Components

**Health Card:** Patient name (title), last visit date (label), status pill, quick-action button. The most-used component in the health worker variant.

**Metric Card:** Large number (metric scale), unit and label below, trend indicator, comparison text. Used for vitals, appointment completion rates, medication adherence.

**Check-In Module:** The signature component of the patient variant. A single question, large text, three to five response options as large tap targets. No keyboard required. Accessible to low-literacy users.

**Referral Badge:** Status pill indicating referral urgency. Three states — routine (neutral), soon (warning), urgent (error). Always visible on patient records.

**Progress Ring:** Circular progress indicator for health goals. Accent green fill on surface-subtle track. Percentage in metric scale at center.

## Do's and Don'ts

- Do use warm cream backgrounds for any content involving emotional support or sensitive health topics
- Do maintain 48px minimum touch targets throughout — health workers often use phones with gloves
- Don't use red decoratively — it triggers alarm responses. Reserve strictly for urgent clinical alerts
- Do write all UI copy in plain language — aim for Grade 6 reading level
- Don't crowd screens with multiple metrics — one primary metric per card
- Do provide clear empty states — "No visits recorded yet" is better than a blank screen
- Don't use Inter Mono for body text — it reads as clinical and cold in health contexts
- Do design every screen assuming the user may be anxious — calm, clear, never rushed

## Anxiety-Responsive Design

Healthcare is the highest-anxiety UI context that exists. Users arriving at a health app are often scared, in pain, or overwhelmed. These are not edge cases — they are the primary use case.

**Cognitive load under stress drops by 40%.** Design for someone who is frightened, not for someone browsing calmly. This means: one action per screen, no more than 5 words per button label, no modal dialogs that require reading before acting.

**Never use red for anything except a genuine emergency.** A user who has been told their test result is "in the red zone" on a decorative red background has just experienced preventable panic. Red is for emergencies. Use neutral grey for errors, amber for attention, never red for UI decoration.

**The 3am test:** This interface will be used by someone alone at 3am who is frightened about a symptom. Every screen must pass this test: does it reduce fear or increase it? Does it give the user a clear next action or leave them more confused? If a screen fails the 3am test, redesign it.

**Shame is a design failure.** Overdue appointments, missed medications, incomplete health records — never use language or visual design that implies failure or judgment. Progress indicators should show what is done, never what is missing. "3 of 5 complete" not "2 remaining."
