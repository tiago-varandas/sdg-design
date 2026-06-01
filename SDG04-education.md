---
version: alpha
name: SDG.design — 04 Quality Education
description: Design system for SDG 4 — Quality Education. Two variants: a learner-facing literacy app and an educator tools platform. Curious, hopeful, accessible.

colors:
  primary: "#2D0A0F"
  secondary: "#8B1A2A"
  tertiary: "#E8748A"
  background: "#FFF9F9"
  surface: "#FFFFFF"
  surface-subtle: "#FBEAEC"
  accent: "#C5192D"
  accent-soft: "#FDEEF0"
  neutral: "#4A4040"
  highlight: "#FFF3CD"
  highlight-border: "#F5C842"
  success: "#2E7D4F"

typography:
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.025em
  title:
    fontFamily: "Helvetica Neue"
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.015em
  body:
    fontFamily: "Helvetica Neue"
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.8
    letterSpacing: 0em
  body-reading:
    fontFamily: "Helvetica Neue"
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.9
    letterSpacing: 0.01em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.05em
  progress:
    fontFamily: "Helvetica Neue"
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.0
    letterSpacing: -0.02em

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
  button-lesson:
    backgroundColor: "{colors.highlight}"
    textColor: "{colors.primary}"
    rounded: "{rounded.lg}"
    padding: 20px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-lesson:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.xl}"
    padding: 28px
  card-highlight:
    backgroundColor: "{colors.highlight}"
    rounded: "{rounded.lg}"
    padding: 20px
  badge-level:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.accent}"
    rounded: "{rounded.full}"
    padding: 8px
  badge-complete:
    backgroundColor: "#E6F4ED"
    textColor: "{colors.success}"
    rounded: "{rounded.full}"
    padding: 8px
  progress-bar:
    backgroundColor: "{colors.surface-subtle}"
    rounded: "{rounded.full}"
    height: 8px
  nav:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.neutral}"
    padding: 16px
---

# SDG.design — 04 Quality Education

## Overview

SDG 4 calls for inclusive and equitable quality education and lifelong learning for all. Design for this goal must be curious, encouraging, and radically accessible. Learning experiences should feel like discovery, not examination.

This system serves two builder contexts. The first is learner-facing literacy and skills apps — tools used directly by students, adult learners, and self-learners across all ages and literacy levels. These must accommodate low literacy, low connectivity, and first-time smartphone users. The second is educator tools platforms — apps used by teachers, tutors, and NGO educators to create content, track progress, and manage cohorts.

The learner variant uses larger text (body-reading scale), extra generous line spacing, and high-contrast interactive elements designed for people who may be navigating a screen interface for the first time. The educator variant is more information-dense, with a dashboard sensibility and efficient navigation.

The palette draws from the bold crimson of the official SDG 4 identity — assertive, energetic, confident. Education is not passive. It is active transformation. The warm background and yellow highlight color add optimism and encouragement without being infantilising.

## Colors

Confident crimson anchored in warmth. The palette signals that learning is an act of courage and aspiration.

- **Primary (#2D0A0F):** Deep crimson-black. Headlines and primary text. Strong and warm.
- **Secondary (#8B1A2A):** Mid crimson. Section headers, active states, link text.
- **Tertiary (#E8748A):** Blush. Chart fills, decorative accents, level indicators.
- **Background (#FFF9F9):** Barely-warm white. The lightest blush tint.
- **Surface (#FFFFFF):** Card and content backgrounds.
- **Surface Subtle (#FBEAEC):** Input fields, recessed sections, progress tracks.
- **Accent (#C5192D):** Bold crimson. Primary CTAs, progress fills, active states.
- **Accent Soft (#FDEEF0):** Used for hover backgrounds and soft badge fills.
- **Neutral (#4A4040):** Warm dark grey for body text.
- **Highlight (#FFF3CD):** Warm yellow. Used exclusively for key callouts, vocabulary words, and encouragement cards. Never for errors.
- **Success (#2E7D4F):** Lesson complete, achievement unlocked. Celebratory green.

## Typography

The `body-reading` scale is unique to this system — 19px, 1.9 line height, slightly positive letter-spacing. It is designed for learners reading text-heavy content, especially those for whom the interface language may not be their first language.

Standard `body` (17px) is used for instructional UI copy — button labels, navigation, tooltips. Slightly larger than most systems to support low-vision users.

Headlines are warm and energetic — tracked tighter than body but not as compressed as data-heavy systems. Education interfaces should inspire, not intimidate.

## Layout

**Learner variant:** Single-column, mobile-first. Lesson cards are full-width with large tap targets. Progress is always visible — a persistent bar at the top of every screen. Navigation is bottom-bar only. Back button always available. No dead ends.

**Educator variant:** Desktop-first, sidebar navigation. Cohort overview as the home screen. Drill-down: cohort → student → lesson → response. Bulk actions available for common tasks (assign, grade, export).

Never show more than three active tasks or lessons on a learner's home screen — cognitive overload is the enemy of learning.

## Elevation & Depth

Lesson cards use a slightly elevated style — white surface on the warm background with a visible border. The border signals "this is interactive" without requiring a shadow.

Highlight cards (yellow fill) create visual anchors for key learning moments — vocabulary, key concepts, encouragement. They stand out from the card flow without disrupting it.

## Shapes

More rounded than civic or climate systems — `xl` at 22px for lesson cards and main learning modules. The roundedness is deliberate: learning should feel safe and exploratory, never punishing.

Progress bars are fully rounded (pill shape) — partial fills look natural and encouraging.

## Components

**Lesson Card:** Illustration area (top), lesson title (title scale), estimated time (label), difficulty badge, start button. Large, tappable, full-width on mobile.

**Progress Bar:** Accent fill on surface-subtle track. Always labeled with a fraction ("Lesson 3 of 8") and percentage. Never just a visual — always has text for screen readers.

**Achievement Badge:** Circular, accent or success color. Icon + label. Awarded on lesson completion, streak milestones, and first-time completions. Celebratory animation on unlock.

**Vocabulary Highlight:** Inline highlight card in yellow. Word in title scale, definition in body. Used within reading passages to surface key terms without leaving the screen.

**Educator Dashboard Row:** Student name, last active date, progress percentage, current lesson, quick-action button (message, assign, flag). Designed for scanning 30+ students efficiently.

## Do's and Don'ts

- Do use the body-reading scale for all learner-facing text content — legibility is a learning equity issue
- Do celebrate progress visibly — every completed lesson deserves a moment of positive feedback
- Don't use red for wrong answers in learning contexts — it triggers shame. Use neutral correction instead.
- Do design for interrupted sessions — learners are often on shared devices with limited time
- Don't require account creation to start learning — first lesson should be accessible immediately
- Do provide audio support affordances — reading icons, speaker icons, visual + text together
- Don't use jargon in UI copy — plain language throughout
- Do make progress saving explicit — "Your progress is saved" is a powerful reassurance

## The Shared Device Problem

In low-income contexts, the majority of learners do not own their device. They use a family phone, a school tablet, or a community device. This changes every design decision.

**Session design:** Every lesson must assume the session will be interrupted. Progress is saved after every single interaction — not at lesson completion. The home screen shows "Continue where you left off" as the primary action, not a menu.

**Multiple user profiles without accounts:** Many learners cannot create accounts because they lack an email address, a phone number, or parental permission. The app must support anonymous profiles identified by a PIN or a chosen avatar — no email required. Switching profiles takes one tap.

**No gamification that shames absence:** Streak counters, daily goals, and "you broke your streak" notifications assume consistent daily access. A child who missed 3 days because a sibling needed the phone does not need to feel punished. Remove all streak-based mechanics. Celebrate return, never penalise absence.

**Audio over text wherever possible:** On a shared device in a noisy household, reading is harder than listening. Every text instruction should have an audio equivalent. Reading speed assumptions in timed exercises should be adjustable. The default reading pace should be set for a Grade 3 level, not an adult.
