---
version: alpha
name: PloverCRM Website Visual System
description: A calm, trustworthy, WordPress-first marketing design system aligned with the shadcn-based PloverCRM app.
colors:
  background: "#ffffff"
  foreground: "#171717"
  card: "#ffffff"
  cardForeground: "#171717"
  popover: "#ffffff"
  popoverForeground: "#171717"
  primary: "#0b8b49"
  primaryForeground: "#fafafa"
  secondary: "#eff8f2"
  secondaryForeground: "#24553a"
  muted: "#f7f7f7"
  mutedForeground: "#737373"
  accent: "#edf9f1"
  accentForeground: "#27613f"
  destructive: "#dc2626"
  border: "#e5e5e5"
  input: "#e5e5e5"
  ring: "#0b8b49"
  chart1: "#0b8b49"
  chart2: "#38a6a5"
  chart3: "#315070"
  chart4: "#e7bd29"
  chart5: "#df9b20"
  sidebar: "#fafafa"
  sidebarForeground: "#171717"
  sidebarPrimary: "#0b8b49"
  sidebarPrimaryForeground: "#fafafa"
  sidebarAccent: "#edf9f1"
  sidebarAccentForeground: "#27613f"
  sidebarBorder: "#e5e5e5"
  sidebarRing: "#0b8b49"
  marketingInk: "#0d1511"
  marketingMuted: "#63746b"
  marketingMint: "#eaf8ef"
  marketingCream: "#fff9ef"
  marketingBlueSoft: "#edf6ff"
  marketingPurpleSoft: "#f4efff"
  marketingOrangeSoft: "#fff3e4"
  marketingSurface: "rgba(255,255,255,.94)"
typography:
  heading:
    family: "Geist Sans, Poppins, Inter, ui-sans-serif, system-ui, sans-serif"
    weight: 700
    lineHeight: 1.05
    letterSpacing: "-0.04em"
  body:
    family: "Geist Sans, Poppins, Inter, ui-sans-serif, system-ui, sans-serif"
    weight: 400
    lineHeight: 1.65
    letterSpacing: "-0.01em"
  label:
    family: "Geist Sans, Poppins, Inter, ui-sans-serif, system-ui, sans-serif"
    weight: 500
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  mono:
    family: "Geist Mono, ui-monospace, SFMono-Regular, Menlo, monospace"
    weight: 500
    lineHeight: 1.45
rounded:
  base: "0.625rem"
  sm: "calc(0.625rem - 4px)"
  md: "calc(0.625rem - 2px)"
  lg: "0.625rem"
  xl: "calc(0.625rem + 4px)"
  "2xl": "calc(0.625rem + 8px)"
  "3xl": "calc(0.625rem + 12px)"
  "4xl": "calc(0.625rem + 16px)"
  marketingCard: "26px"
  marketingPanel: "34px"
  pill: "999px"
spacing:
  xs: "0.375rem"
  sm: "0.625rem"
  md: "1rem"
  lg: "1.5rem"
  xl: "2.25rem"
  xxl: "3.5rem"
  section: "6rem"
components:
  appButton:
    background: "{colors.primary}"
    color: "{colors.primaryForeground}"
    radius: "{rounded.md}"
    height: "2.25rem"
    padding: "0.5rem 1rem"
    typography: "{typography.label}"
    focusRing: "3px {colors.ring}/50"
  marketingPrimaryButton:
    background: "{colors.primary}"
    color: "{colors.primaryForeground}"
    radius: "{rounded.pill}"
    padding: "14px 22px"
    typography: "{typography.label}"
  marketingSecondaryButton:
    background: "{colors.background}"
    color: "{colors.foreground}"
    border: "1px solid {colors.border}"
    radius: "{rounded.pill}"
    padding: "14px 22px"
    typography: "{typography.label}"
  appCard:
    background: "{colors.card}"
    color: "{colors.cardForeground}"
    border: "1px solid {colors.border}"
    radius: "{rounded.xl}"
    paddingY: "1.5rem"
    shadow: "shadow-sm"
  marketingCard:
    background: "{colors.marketingSurface}"
    color: "{colors.marketingInk}"
    border: "1px solid {colors.border}"
    radius: "{rounded.marketingCard}"
    shadow: "0 22px 60px rgba(4,27,18,.08)"
  input:
    background: "transparent"
    color: "{colors.foreground}"
    border: "1px solid {colors.input}"
    radius: "{rounded.md}"
    height: "2.25rem"
    padding: "0.25rem 0.75rem"
    focusRing: "3px {colors.ring}/50"
  badge:
    background: "{colors.primary}"
    color: "{colors.primaryForeground}"
    radius: "{rounded.pill}"
    padding: "0.125rem 0.5rem"
    typography: "{typography.label}"
---

## Overview

PloverCRM’s website should feel like the public-facing extension of the shadcn-based product app: clean, calm, trustworthy, operational, and conversion-focused.

The visual identity should communicate one main idea:

> A polished WordPress lead-management system that helps businesses stop losing leads after capture.

The website should not feel like a generic SaaS page. It should show the workflow visitors care about: leads arrive from WordPress forms, ads, webhooks, and other sources; PloverCRM turns them into organized records with source data, owners, statuses, reminders, and next actions.

The design should reduce fear of “another complicated CRM” by making the product feel structured, simple, and fast to adopt.

## Colors

The website should preserve the app’s shadcn semantic color model: background, foreground, card, popover, primary, secondary, muted, accent, destructive, border, input, ring, chart, and sidebar tokens.

Use green as the main brand signal. Green should communicate control, trust, growth, and operational clarity.

- `{colors.primary}` maps to the app’s primary green token, originally `oklch(0.482 0.158 141)`.
- `{colors.primaryForeground}` maps to the app’s near-white foreground on green.
- `{colors.secondary}` and `{colors.accent}` carry the app’s soft green surfaces.
- `{colors.muted}` and `{colors.mutedForeground}` preserve the shadcn muted text/background relationship.
- `{colors.border}`, `{colors.input}`, and `{colors.ring}` should be used for borders, fields, and focus states.
- `{colors.marketingInk}`, `{colors.marketingMuted}`, and `{colors.marketingSurface}` are marketing aliases for larger editorial sections, but they should not replace shadcn semantic tokens inside app-like components.
- `{colors.marketingCream}`, `{colors.marketingBlueSoft}`, `{colors.marketingPurpleSoft}`, and `{colors.marketingOrangeSoft}` may be used for soft supporting icon backgrounds, but green must remain dominant.

Use soft radial glows in the page background when they add depth. Avoid loud gradients, aggressive dark enterprise styling, and purple-heavy AI/SaaS clichés.

## Typography

Use Geist Sans as the primary font to stay aligned with the product app. Poppins may remain as a marketing fallback only when an existing static page already depends on it.

Headings should be bold, tight, confident, and easy to scan. Use negative letter spacing and short, outcome-focused lines.

Good heading examples:

- Stop Losing WordPress Leads After They Submit the Form
- Works with the tools your leads already come from.
- Every lead has a source, owner, status, and next step.

Body copy should be calm, short, and specific. Use 15–18px body text for most content, with muted gray-green color and generous line height.

Avoid long technical explanations in the hero and top sections.

## Layout

Layouts should feel structured like the product app but more editorial and spacious for marketing.

Use:

- Wide containers for visual sections.
- Card-based layouts to organize ideas.
- Clear vertical rhythm between sections.
- Alternating section types: problem, proof, workflow, benefit, objection, CTA.
- Product visuals and diagrams to explain how PloverCRM works.

Recommended widths:

- Text-heavy sections: 1120–1240px.
- Visual diagram sections: 1400–1660px.
- Hero/dashboard visuals: 920–1200px.
- Conversion sections: `calc(100% - 40px)` up to 1160–1400px.

The homepage journey should follow:

> Promise → Pain → Mechanism → Value → Compatibility → Features → Product Tangibility → Differentiator → Relevance → Proof → Objections → Decision → FAQ → Action

## Elevation & Depth

Use soft depth, not heavy shadows.

Cards should generally use:

```css
background: rgba(255,255,255,.94);
border: 1px solid var(--line);
border-radius: 26px;
box-shadow: 0 22px 60px rgba(4,27,18,.08);
```

Use stronger elevation only for hero visuals, featured cards, review highlights, and central workflow hubs. Hover lift should be subtle and only used when the element is interactive.

## Shapes

The system should inherit the app’s shadcn radius scale from `--radius: 0.625rem`.

Use:

- `{rounded.md}` for app-like controls such as buttons and inputs.
- `{rounded.xl}` for app-like cards, matching `rounded-xl`.
- `{rounded.marketingCard}` for larger editorial website cards.
- `{rounded.marketingPanel}` for hero visuals, conversion panels, and large diagrams.
- `{rounded.pill}` for badges and compact source labels.

Avoid sharp enterprise boxes unless a table or data-grid style specifically requires it.

## Components

### Buttons

App-like buttons should follow the shadcn `Button` primitive: inline-flex, `rounded-md`, `text-sm`, `font-medium`, `h-9`, `px-4`, `gap-2`, transition states, disabled opacity, and visible `ring/50` focus states.

Marketing CTAs may use larger pill buttons, but their color hierarchy should still map back to shadcn variants: default, outline, secondary, ghost, and link.

Primary buttons use solid green with white text. They should be reserved for important conversion actions.

Primary CTA:

- Download Plugin

Secondary buttons use white or translucent backgrounds with a light border.

Secondary CTA:

- Try a Demo

Supporting reassurance should stay short and distributed across the page. Use phrases such as **No credit card required**, **30-day free trial**, **Works with your existing WordPress forms**, and **Set up your first source in minutes** only where they support conversion without adding clutter.

Every major section does not need a CTA. Hero, integrations, pricing, and final CTA sections should usually include one.

### Cards

App-like cards should follow the shadcn card primitive: `bg-card`, `text-card-foreground`, `rounded-xl`, `border`, `py-6`, `shadow-sm`, and internal `px-6` content spacing.

Marketing cards can be more expressive, but they should still feel like larger versions of the same primitive: white or translucent white surfaces, light borders, soft shadows, and clear internal spacing.

Use cards to make lead-management concepts tangible.

Common card types:

1. Feature cards — icon, heading, short description.
2. Metric cards — number, label, icon.
3. Workflow cards — step number, icon, process description.
4. Review cards — avatar, name, role, quote, outcome badge.
5. Integration cards — logo, tool name, connector line when used in maps.
6. Objection cards — objection, response, proof or benefit.

### Icons

Use Lucide-style line icons for product and UI concepts. Avoid Unicode symbols for production visuals.

Icon rules:

- Use line icons with consistent stroke width.
- Match app sizing: `size-4` inside buttons, `size-5` inside 40px icon containers, and smaller `size-3` icons inside badges.
- Place icons inside soft rounded containers such as `size-10 rounded-lg bg-primary/10 text-primary`.
- Keep each section visually consistent.
- Use real image/SVG assets for brand logos where possible.
- Do not mix filled emoji-like glyphs with clean line icons.

Recommended icon concepts:

- Lead capture: inbox, form, download, link.
- Source tracking: target, radar, map-pin, crosshair.
- Assignment: user-check, users.
- Reminders: clock, bell.
- Pipeline: columns, chart, list-filter.
- Automation: workflow, zap, settings.
- Mobile CRM: smartphone.
- Trust/security: shield-check.

### Forms and Inputs

Forms should feel close to the app UI:

- `h-9` fields.
- `rounded-md` corners.
- `border-input` borders.
- Transparent or card-matched backgrounds.
- `px-3 py-1` compact padding.
- Clear labels.
- Helpful placeholder text using muted foreground.
- Green `focus-visible:border-ring` and `focus-visible:ring-ring/50` states.
- Inline validation using destructive border/ring states where needed.

Avoid overly stylized fields that feel disconnected from the product.

### Navigation

The public header should be marketing-friendly but clean:

- White translucent background with blur.
- Rounded container.
- Logo left.
- Navigation center or left.
- CTA right.
- Avoid overcrowding.

Recommended nav items:

- Features
- Solution
- How it Works
- Integrations
- Pricing
- FAQs

### Tables and Data UI

Use table-like UI only when it helps conversion clarity, such as feature comparison, before/after transformation, plan comparison, or integration matrices.

Keep public-facing tables lighter and less dense than product-app tables.

### Charts and Metrics

Use chart-like visuals sparingly. They should communicate outcomes, not analytics complexity.

Good metric themes:

- Faster follow-up.
- Fewer missed leads.
- More visible lead sources.
- Clear owner on every lead.
- Web and mobile access.

Use green as the main data color, soft area fills, light grid patterns, muted labels, and rounded tooltip/card styling.

## Visual Motifs

Reuse these motifs across pages:

### Lead flow lines

Use dotted or subtle connector lines to show movement from source to CRM to follow-up.

### Soft radial glows

Use green and blue glows in the background for depth.

### Source badges

Use small pills for WordPress, Google Ads, Meta Ads, Webhooks, forms, reminders, and mobile.

### Pipeline cards

Use card sequences to show lead stages, next actions, or follow-up status.

### Hub-and-spoke maps

Use for integrations and lead-source sections. Keep the center uncluttered; a favicon or compact brand mark is enough when space is tight.

### Outcome badges

Use small green badges inside cards to show results such as “Faster follow-up” or “Clear ownership.”

## Homepage Sections

Use this approved flow as the default homepage structure:

1. Hero — clear WordPress-first promise.
2. Broken Funnel vs Lead-Control Funnel — show what breaks after capture.
3. Connected Lead System — explain the source-to-CRM-to-outcome mechanism.
4. Metric Benefits — number-led value from industry research.
5. Integrations — grouped by capture, follow-up, and outcomes.
6. Product Pillars Tabs — progressive disclosure for core capabilities.
7. Live Lead Record Anatomy — show the finished follow-up-ready record.
8. Mobile CRM Access — dedicated web/iPhone/Android differentiator.
9. Use Cases — role and business relevance.
10. Customer Reviews / Outcomes — human proof.
11. Objection Handling — persuasive objection cards.
12. Practical Buying Comparison — final decision recap.
13. FAQ — factual accordions.
14. Final CTA — focused conversion panel.

Each major section should define:

- Section name.
- Awareness stage.
- Visitor question it answers.
- Main message.
- Key visual.
- CTA, if any.
- Reason for inclusion.

## Responsive Behavior

Desktop:

- Use asymmetrical layouts.
- Use large visuals and generous spacing.
- Complex diagrams are allowed.

Tablet:

- Collapse major two-column sections into one column.
- Convert diagrams into clean grids.
- Keep cards readable and balanced.

Mobile:

- Use one-column layouts.
- Make CTAs full-width when useful.
- Hide complex connector lines.
- Reduce large heading sizes.
- Keep important content above the fold.

## Accessibility

Follow these rules:

- Buttons and links must have clear labels.
- Decorative images should use empty alt text.
- Meaningful images and logos need descriptive alt text.
- Focus states must be visible.
- Do not rely on color alone for meaning.
- Hover effects should not be required to understand content.
- Motion should be smooth and restrained.
- Review carousels and animated sections should not make text hard to read.

## Do’s and Don’ts

### Do

- Lead with the problem of losing leads after form submission.
- Make the workflow visible through diagrams, cards, timelines, and source maps.
- Use calm green accents and soft card surfaces.
- Use specific WordPress lead-management copy.
- Show source, owner, status, reminder, and next-step concepts repeatedly.
- Keep sections visually distinct but part of one system.
- Use proof and objections before the final CTA.

### Don’t

- Do not position PloverCRM as a generic CRM.
- Do not use vague SaaS claims like “grow faster with smarter tools.”
- Do not overuse loud gradients or decorative visuals without conversion purpose.
- Do not use random Unicode symbols as icons.
- Do not overcrowd integration hubs with unnecessary logos.
- Do not make the public site feel disconnected from the product app.
- Do not add heavy technical explanations in the hero.

## App Alignment Checklist

Before confirming a website pattern, verify it still harmonizes with the shadcn app:

- Does it use Geist Sans or intentionally preserve a marketing fallback?
- Does it map colors to semantic shadcn roles before using marketing aliases?
- Do app-like controls keep `h-9`, `rounded-md`, `text-sm`, and visible focus rings?
- Do cards feel like larger versions of `bg-card rounded-xl border py-6 shadow-sm`?
- Do icons match Lucide line style, sizing, and stroke behavior?
- Do data sections borrow the app’s compact table, chart, and muted-label patterns without becoming too dense for marketing?
- Are dark-mode assumptions avoided unless the website explicitly implements matching tokens?

## Design Quality Checklist

Before a section is approved, check:

- Does it support the lead-control positioning?
- Is the headline specific and understandable?
- Is the visual useful, not just decorative?
- Does the section have enough spacing?
- Are icons consistent?
- Are cards aligned and balanced?
- Does it work on mobile?
- Does the copy match the buyer awareness stage?
- Does it reduce doubt or increase desire?
- Is the CTA clear if the section needs one?

## Maintenance

This file is the living visual source of truth for the PloverCRM website. Update it when a user-approved pattern becomes reusable, when a design decision changes, or when a section creates a new standard.

When updating this file:

- Keep tokens machine-readable in the YAML front matter.
- Keep rationale human-readable in the markdown body.
- Preserve clear section headings.
- Remove stale guidance instead of keeping outdated compatibility notes.
- Use this file during future website redesigns, homepage section work, and landing-page implementation.
