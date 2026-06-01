---
version: alpha
name: SDG.design — 05 Gender Equality
description: Design system for SDG 5 — Gender Equality. Two variants: a safety and support tool and an economic empowerment platform. Bold, safe, empowering.

colors:
  primary: "#1A0508"
  secondary: "#7A0E1E"
  tertiary: "#F4859A"
  background: "#FFF8F8"
  surface: "#FFFFFF"
  surface-subtle: "#FFF0F2"
  accent: "#FF3A21"
  accent-soft: "#FFE8E5"
  neutral: "#4A3A3C"
  trust: "#C44569"
  trust-soft: "#FDEEF3"
  success: "#2E7D4F"
  safe: "#E8F5EE"

typography:
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.03em
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
    letterSpacing: -0.005em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.05em
  strong:
    fontFamily: "Helvetica Neue"
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em

rounded:
  sm: 6px
  md: 10px
  lg: 14px
  xl: 22px
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
  button-trust:
    backgroundColor: "{colors.trust}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: 20px
  button-safe:
    backgroundColor: "{colors.safe}"
    textColor: "{colors.success}"
    rounded: "{rounded.full}"
    padding: 20px
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 20px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-trust:
    backgroundColor: "{colors.trust-soft}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-safe:
    backgroundColor: "{colors.safe}"
    rounded: "{rounded.lg}"
    padding: 24px
  emergency-button:
    backgroundColor: "{colors.accent}"
    textColor: "#FFFFFF"
    rounded: "{rounded.xl}"
    padding: 24px
  nav:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.neutral}"
    padding: 16px
---

# SDG.design — 05 Gender Equality

## Overview

SDG 5 calls for gender equality and the empowerment of all women and girls. Design for this goal carries heightened responsibility — tools in this space are often used in sensitive, high-stakes contexts. The design system must be both bold in its visual confidence and deeply safe in its interaction design.

This system serves two builder contexts. The first is safety and support tools — apps for domestic violence survivors, legal aid access, safe reporting, and crisis navigation. These require discreet exit mechanisms, trauma-informed interaction patterns, and nothing that could endanger a user if their device is checked by an abuser. The second is economic empowerment platforms — tools for skills training, micro-financing, job access, and entrepreneurship support for women and girls in low-income contexts.

Safety tools must prioritise dignity and control above all else. The user has likely already experienced a loss of control — every interaction should return agency. Economic empowerment tools should feel aspirational, energising, and peer-connected.

The palette draws from the official SDG 5 coral-red — bold, assertive, unapologetic. This is not a soft or apologetic design system. Gender equality is a fundamental right, and the design should communicate that confidence.

## Colors

Bold coral-red anchored in warmth, with a distinct trust palette for sensitive contexts.

- **Primary (#1A0508):** Deep warm black. Headlines and primary text.
- **Secondary (#7A0E1E):** Deep crimson. Section headers, active states.
- **Tertiary (#F4859A):** Blush rose. Decorative fills, chart elements, secondary labels.
- **Background (#FFF8F8):** Barely-warm white. The softest blush.
- **Surface (#FFFFFF):** Card backgrounds.
- **Surface Subtle (#FFF0F2):** Recessed panels, input backgrounds.
- **Accent (#FF3A21):** Bold coral-red. Primary CTAs, active states. Confident and unapologetic.
- **Accent Soft (#FFE8E5):** Used for hover states and soft pill backgrounds.
- **Neutral (#4A3A3C):** Body text. Warm dark.
- **Trust (#C44569):** A deeper rose used for sensitive support contexts — calmer than accent but still strong.
- **Trust Soft (#FDEEF3):** Background for trust/support card contexts.
- **Safe (#E8F5EE):** Used exclusively for confirmed safe states and positive outcomes.

## Typography

Body at 16px, 1.75 line height — readable under stress. The `strong` variant (same size, weight 500) is used for key information that must be retained — rights statements, safety instructions, emergency numbers.

Headlines are confident and tight — this is not a shy design system. The typography communicates that the user is in a space that takes their situation seriously.

## Layout

**Safety tool variant:** Always shows an emergency exit button — one tap returns to a neutral screen (e.g., a recipe website or news page). This is a hard requirement. No personal data shown on the home screen — privacy by default. All sensitive content is behind authentication. Navigation is minimal to reduce visible usage history.

**Empowerment platform variant:** Community-forward home screen — peer stories, active challenges, group progress. Bottom navigation. Profile is prominent but private by default. Achievement and progress systems are social-opt-in only.

## Elevation & Depth

Trust cards use the soft rose fill to create a visually distinct "safe space" within the UI — content in these cards should feel like a protected, private area. No shadows — flat fills create enclosure without visual weight.

The emergency button is the only component that breaks the card grid — it sits outside the normal layout rhythm, always accessible.

## Shapes

`xl` (22px) for primary action cards and support modules — generous radius signals safety. Full radius for all buttons and pills. No sharp corners anywhere in the safety variant.

## Components

**Emergency Exit Button:** Full-width or fixed-position. Accent red background. Single tap exits to a pre-configured safe page. Available on every screen of the safety variant. Cannot be disabled.

**Support Card:** Trust-soft background. Hotline number in `strong` scale. Opening hours, language options. Always static — works without network connection.

**Rights Statement Card:** Key legal right or resource, stated plainly. Strong typography. Safe-green left border to signal verified information.

**Peer Story Card:** Avatar (initials only, no photo), first name only, short quote. Community connection without privacy risk.

**Skills Badge:** Achievement in the empowerment variant. Earned through course completion. Shareable to LinkedIn or PDF — designed as a portable credential.

**Progress Module:** Course completion ring, next step prompt, peer cohort progress. Motivating without being competitive.

## Do's and Don'ts

- Do include a quick-exit mechanism on every screen of the safety variant — this is non-negotiable
- Do default all profiles to private — users opt in to visibility, never opt out
- Don't use location services without explicit, revocable, per-session consent
- Do write legal and rights content in plain language — complex legal text is inaccessible in crisis
- Don't store sensitive data locally without encryption
- Do design for one-handed use — safety situations often involve physical constraint
- Don't use shame-adjacent language anywhere — never "failed", "missed", "behind"
- Do test with actual community members — this system should never be shipped without lived-experience review
- Don't make the app visually identifiable as a safety app from the home screen icon or preview

## Designing Against Coercive Control

Domestic abuse is partly a technology problem now. Abusers use phones to monitor, track, and control. A safety app that does not account for this actively endangers its users.

**Disguise mode is not optional:** The app icon, app preview in the task switcher, and notification previews must all be configurable to show neutral content. A user whose phone is checked by an abuser must be able to make the app invisible or appear to be something harmless (a recipe app, a news reader). This is a survival feature, not a UX nicety.

**Screenshot-safe screens:** Sensitive content (shelter addresses, legal resources, safety plans) must not appear in screenshots or screen recordings. Use CSS techniques to prevent capture of specific elements. Test this before shipping.

**No cloud backup of sensitive data by default:** Many phones automatically back up to a shared family account. Any sensitive data (messages, safety plan, contacts) must be stored locally only, with encryption, and excluded from iCloud/Google Photos/automatic backups. Make this the default — not an opt-in setting.

**Coercive account sharing:** Abusers sometimes demand to see app accounts. The app must support a "safe view" — a secondary state that shows only neutral content even when logged in. This is sometimes called a duress PIN: entering a specific PIN shows a sanitised version of the app. This is a known pattern in safety technology and should be implemented from day one.
