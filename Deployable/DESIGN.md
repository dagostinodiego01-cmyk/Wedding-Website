---
name: Diego & Bethany Wedding
description: A fresh spring botanical wedding site for invited guests planning the day at Southdowns Manor.
colors:
  cream: "#EFF6FA"
  cream-deep: "#DCEAF5"
  cream-warm: "#E6F0F8"
  ink: "#2E3220"
  ink-soft: "#4A4C36"
  sage: "#9AC47C"
  sage-deep: "#45703A"
  olive: "#5D9440"
  forest: "#2C5327"
  mist: "#ADBDAC"
  peach: "#80A3C2"
  gold: "#80A3C2"
  mustard: "#80A3C2"
  dusty-blue: "#80A3C2"
  terracotta: "#43627E"
  gold-deep: "#43627E"
  champagne: "#EBF3F6"
typography:
  display:
    fontFamily: "Dancing Script, 'Segoe Script', cursive"
    fontSize: "clamp(3.9rem, 11.5vw, 8rem)"
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: "0"
  headline:
    fontFamily: "Montserrat, system-ui, 'Segoe UI', Arial, sans-serif"
    fontSize: "clamp(2.35rem, 4.9vw, 3.6rem)"
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Montserrat, system-ui, 'Segoe UI', Arial, sans-serif"
    fontSize: "clamp(1.6rem, 3vw, 2.05rem)"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Montserrat, system-ui, 'Segoe UI', Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Montserrat, system-ui, 'Segoe UI', Arial, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.22em"
rounded:
  xs: "3px"
  sm: "4px"
  md: "6px"
spacing:
  xs: "8px"
  sm: "14px"
  md: "22px"
  lg: "32px"
  xl: "44px"
  section: "110px"
components:
  button-primary:
    backgroundColor: "{colors.peach}"
    textColor: "{colors.ink}"
    rounded: "{rounded.xs}"
    padding: "15px 38px"
    typography: "{typography.label}"
  button-primary-hover:
    backgroundColor: "{colors.terracotta}"
    textColor: "{colors.cream}"
    rounded: "{rounded.xs}"
    padding: "15px 38px"
  card-soft:
    backgroundColor: "{colors.cream-deep}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "44px"
  input-dark:
    backgroundColor: "#FBF6EE14"
    textColor: "{colors.cream}"
    rounded: "{rounded.xs}"
    padding: "13px 16px"
---

# Design System: Diego & Bethany Wedding

## 1. Overview

**Creative North Star: "The Manor Garden Letter"**

The system should feel like a personal invitation carried through a countryside garden: soft enough for a wedding, clear enough for guests who need practical details, and specific enough to belong to Diego and Bethany rather than to a generic wedding template. It uses botanical accents, restrained page rhythm, and a warm guest-first tone to make the site feel celebratory without losing utility.

The visual language is established in the static HTML: pale sky-blue paper surfaces, fresh spring-foliage greens for botanical structure, and a deeper spring-sky blue for accents and emphasis. Type is Montserrat throughout — headings and body — with Dancing Script reserved for the couple's names in the hero. Small botanical dividers, soft reveal motion, and ambient shadows complete the system. Preserve those choices unless a future task explicitly asks for a departure. The system rejects gray, flat, static interfaces and placeholder-heavy layouts that feel lifeless.

**Key Characteristics:**
- Warm practical pages for invited guests.
- Botanical detail used as a signature, not filler.
- Soft contrast between cream surfaces and garden-toned accents.
- Ambient depth and light motion rather than heavy decoration.
- Clear form, schedule, and travel information above pure ornament.

## 2. Colors

The palette is a fresh countryside-spring range: pale sky-blue paper grounds, new-growth spring-foliage greens for botanical structure, and a deeper spring-sky blue for accents, actions, and emphasis. It reads as a bright April garden under an open sky rather than the earlier warm cream-and-terracotta scheme.

> **Legacy token names.** The CSS custom properties keep their original warm names (`--cream`, `--cream-deep`, `--cream-warm`, `--terracotta`, `--gold`, `--peach`, `--mustard`) for continuity, but they now hold cool values — the `--cream*` grounds are pale sky-blue and the accent tokens are spring-sky blue. Read tokens by role (below), not by name.

### Grounds (Neutral)
- **Invitation Sky** `--cream` (#EFF6FA): Main page background and the light text used on deeper accent surfaces (e.g. the accent-blue button on hover).
- **Pressed Paper** `--cream-deep` (#DCEAF5): Alternating section background and soft card surface — a slightly deeper pale sky-blue.
- **Soft Paper** `--cream-warm` (#E6F0F8): Subtle pale sky-blue fill for eyebrows and small surfaces.

### Text
- **Garden Ink** `--ink` (#2E3220): Primary text, focus contrast, and the grounding color for body copy.
- **Soft Ink** `--ink-soft` (#4A4C36): Secondary text and the uppercase hero subtitle.

### Spring Foliage (Structure)
- **Spring Sage** `--sage` (#9AC47C): Soft botanical color for hero atmospherics, gradients, and supporting detail.
- **Deep Leaf** `--sage-deep` (#45703A): Darker green for readable secondary text and schedule structure.
- **Olive Stem** `--olive` (#5D9440): Botanical SVG strokes and quiet garden-line accents.
- **Forest** `--forest` (#2C5327): Deepest green for gradient ends and the RSVP success check.
- **Pastel Mist** `--mist` (#ADBDAC): Soft pastel-green surface for the RSVP panel — a calm light section (dark ink text, blue accents) that gives the RSVP its own identity without over-using the accent blue.

### Spring Sky (Accent & Emphasis)
- **Sky Accent** `--peach` / `--gold` / `--mustard` / `--dusty-blue` (#80A3C2): The single accent blue — button backgrounds, labels, botanical marks, selection highlights, and gradients.
- **Sky Emphasis** `--terracotta` / `--gold-deep` (#43627E): Deeper blue for emphasis text such as the couple's names, hover states, and prominent labels.
- **Sky Tint** `--champagne` (#EBF3F6): Pale surface and text selection.

### Named Rules
**The Guest-First Contrast Rule.** Body text stays close to Garden Ink or Invitation Sky; decorative pale text is not allowed to carry essential information.

**The Accent-with-Restraint Rule.** The spring-sky blue marks action, romance, and botanical detail; it should feel earned, not flood every component. Fresh greens carry structure; the blue carries emphasis.

## 3. Typography

**Primary Font:** Montserrat (with system-ui, Segoe UI, Arial fallback) — used for headings and body.
**Hero Script:** Dancing Script (with Segoe Script, cursive fallback) — reserved for the couple's names in the hero. It is the closest widely-available Google Font to the requested "Jimmy Script"; drop in the licensed face here if it is ever self-hosted.

**Character:** Montserrat carries the whole page in a single geometric-sans family, using weight and size for hierarchy (600 for headings, 400 for body) rather than a second text face. Dancing Script gives the couple's names their one handwritten, invitation-quality moment in the hero; everything else stays practical and legible.

### Hierarchy
- **Hero names** (Dancing Script, 600, `clamp(3.9rem, 11.5vw, 8rem)`, ~1.04): Only "Diego & Bethany" in the hero.
- **Headline** (Montserrat, 600, `clamp(2.35rem, 4.9vw, 3.6rem)`, ~1.1, -0.02em): Section titles such as story, day, travel, gallery, and RSVP.
- **Title** (Montserrat, 600, `clamp(1.6rem, 3vw, 2.05rem)`, ~1.2): Schedule names, card headings, venue title, and footer signature.
- **Body** (Montserrat, 400, 1rem, 1.6): Guest-facing explanatory copy, capped around 62ch in the current page.
- **Label** (Montserrat, 500, 0.75rem, 0.22em, uppercase): Navigation, form labels, tags, countdown labels, and the hero date/venue subtitle.

### Named Rules
**The One-Script-Moment Rule.** Dancing Script appears only on the couple's names in the hero. Everywhere else is Montserrat; don't scatter the script into section titles or accents, or it stops feeling special.

**The Invitation-Not-Broadsheet Rule.** Lead with guest clarity; do not turn sections into editorial magazine styling. Hierarchy comes from Montserrat weight and size, not decoration.

## 4. Elevation

This system uses ambient softness: most surfaces are flat or tonally separated, with a single warm shadow reserved for lifted cards, mobile navigation, and hover states. Depth should feel like paper and garden light, not glass, chrome, or app panels.

### Shadow Vocabulary
- **Ambient Paper Lift** (`0 20px 60px rgba(94,84,45,0.12)`): Use for the venue card, photo placeholders, mobile menu, and interactive card hover states.

### Named Rules
**The Soft-Lift Rule.** Shadows appear when a surface needs tactile emphasis or hierarchy; do not add shadows to every repeated item.

## 5. Components

Components should feel warm, practical, and guest-first: ceremonial enough for the occasion, but never so precious that guests have to work to find details.

### Buttons
- **Shape:** Small radius, exact current value 3px.
- **Primary:** Sky-accent blue (`--peach`, #80A3C2) background, Garden Ink text, uppercase Montserrat label, `15px 38px` padding.
- **Hover / Focus:** Hover shifts to sky-emphasis blue (`--terracotta`, #43627E) with Invitation Sky text and a small upward translate. Focus uses a visible 2px outline with 3px offset.
- **Secondary / Ghost / Tertiary:** Not currently defined. Future secondary buttons should use a full border or quiet text treatment, not side-stripe accents.

### Chips
- **Style:** Small uppercase tags use sky-emphasis blue (`--terracotta`, #43627E) text on the surrounding surface, with no filled pill by default.
- **State:** Use for "Coming soon" and similar status labels; avoid making them compete with calls to action.

### Cards / Containers
- **Corner Style:** 4px for image placeholders and gallery items, 6px for cards and venue containers.
- **Background:** Pressed Paper for large content containers; Invitation Sky for smaller cards on Pressed Paper sections.
- **Shadow Strategy:** Ambient Paper Lift only on prominent cards or hover states.
- **Border:** Use the existing `rgba(51,54,31,0.14)` line for schedule rows and travel cards.
- **Internal Padding:** 32px for small cards, 44px for the venue card.

### Inputs / Fields
- **Style:** RSVP form fields sit on the pastel-mist panel with a translucent-white fill, hairline ink border, dark ink text, 10px radius, and Montserrat body type.
- **Focus:** Border shifts to sky-emphasis blue with a soft sky-accent focus ring; the fill lightens slightly.
- **Error / Disabled:** Invalid fields use a muted rose border and icon; text stays dark ink for readability (colour is never the only signal). Disabled not yet defined.

### Navigation
- **Style:** Fixed top nav with translucent cream background, blur, spring-accent hover underline, and compact uppercase Montserrat links.
- **Mobile:** Links slide in as a right-side cream panel with Ambient Paper Lift. The menu toggle must keep its accessible label and visible focus state.

### Botanical Divider
The sprig SVG is the signature motif. Use it sparingly as a ceremonial divider or visual pause; do not repeat it above every small block of text.

## 6. Do's and Don'ts

### Do:
- **Do** preserve the existing color tokens from `diego-bethany-wedding.html` when extending the page.
- **Do** keep guest logistics easy to scan: schedule rows, travel cards, RSVP fields, and venue details should read quickly.
- **Do** use Dancing Script only for the couple's names in the hero — the site's single script moment.
- **Do** use Montserrat everywhere else: headings, navigation, forms, labels, and practical body copy.
- **Do** support reduced motion and keep reveal content visible by default or safely recoverable.

### Don't:
- **Don't** make the interface gray, flat, or static; that is an explicit anti-reference for this project.
- **Don't** use generic wedding-template styling that could belong to any couple.
- **Don't** let placeholders dominate the page once real imagery is available.
- **Don't** use side-stripe accent borders, gradient text, glassmorphism, or repeated tiny uppercase labels as default scaffolding.
- **Don't** reduce essential form, schedule, travel, or RSVP text to low-contrast decorative color.