---
name: TIP TOP Customz
description: Calm navy-and-gold bands around a mobile pressure-washing crew's own before/after photos, booked by text.
colors:
  paper: "#f4f6fb"
  light: "#e7ecf5"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0e1f3d"
  body: "#26354b"
  soft: "#4a5870"
  navy: "#17366b"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c8d4e8"
  rule-dark: "rgba(255,255,255,.14)"
  gold: "#e8b84a"
  gold-2: "#f2ca6a"
  gold-ink: "#85601a"
  focus: "#2563d9"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(44px, 12.4vw, 84px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 400
    lineHeight: 1.2
  control:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  stack: "16px"
  block: "32px"
  section: "64px"
  section-wide: "96px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    typography: "{typography.control}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.control}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    textColor: "{colors.on-dark}"
    height: "68px"
  float-text:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: TIP TOP Customz

## Overview

**Creative North Star: "Night Navy, Gold Script"**

The system takes its whole palette from the client's logo, a black-ground badge with a chrome "TIP TOP" and a gold script "Customz", and moves that night into navy so the page never goes black. Full-bleed bands alternate between off-white paper and two navies, and the photographs carry the proof. The crew's own after shot sits behind the hero under a navy veil, and four before/after pairs from their Facebook post video follow it. Gold is the one warm voice. It fills the primary action, the floating text circle and the arrow wells, and it colours only the last phrase of a heading on dark ground.

The look is Ellie's house "calm band" style (`~/.claude/skills/pitch-site/references/calm-photo-style.md`), and this build is a faithful instance of it. Density is low and phone-first: one column at 20px gutters, generous 64px bands, and a single display face at regular weight. Motion is limited to three moments: the hero H1 bounces in letter by letter once, content below the first screen rises 12px into view, and a gold text circle slides up after the hero.

Everything is soft and borderless. Cards have 24px corners, buttons and chips are full pills, inputs sit on a tinted fill, and the only shadow on the page is under the floating circle.

**Key Characteristics:**
- Paper / navy / light / deep-navy bands, each section obvious by colour change alone.
- Gold as a fill, never as text on light; a darker gold-ink stands in when gold must be read on paper.
- Cal Sans at weight 400 for every heading, button, label and phone number; system sans for running text at 16/1.7.
- Real photography only, cropped 4:5 for proof and shown under a navy gradient where text sits on it.
- Flat surfaces; depth comes from band contrast, not shadow.

## Colors

A cool paper-and-navy palette with one warm gold accent, all sampled from the logo.

### Primary
- **Customz Gold** (gold): the logo's script colour. It fills the primary button, the floating text circle, the selected state of the arrow wells, the eyebrow dot and `::selection`. On dark bands it is also the accent phrase of a heading, the phone icon and link hover colour.
- **Warm Gold Highlight** (gold-2): hover fill for the primary button only.
- **Burnished Gold Ink** (gold-ink): gold as text on light grounds (the "Customz" line of the header wordmark, the header phone icon and hover, accent phrases on paper). It clears 4.5:1 on paper and light, which bright gold cannot.

### Secondary
- **Logo Navy** (navy): the mid-navy band (services, the closing band) and the Facebook proof row.
- **Night Navy** (ink): the logo's night ground. It is the colour of headings on light, text on gold, the selected chip and the before/after frame behind the photos, and (as `--deep`) the ground of the hero and the footer, where it carries the faint diagonal texture.

### Tertiary
- **Electric Form Blue** (focus): the logo's neon blue, kept for interaction only. It is the focus ring on light grounds, the hover/focus border of inputs and chips, the hover outline of the form's submit, and the caret colour.

### Neutral
- **Paper** (paper): page ground, header and the paper bands.
- **Quote Mist** (light): the band behind the quote form.
- **Card White** (card): the form card. White is also the hero H1, the before/after labels and the selected chip's text.
- **Field Mist** (field): the fill for inputs and chips on the white card, distinct enough from white to read as a control.
- **Body Slate** (body): running text on light grounds.
- **Soft Slate** (soft): ledes, step descriptions, placeholders, hints.
- **Moonlight** (on-dark): headings, buttons and links on navy.
- **Moonlight Soft** (on-dark-soft): running text on navy.
- **Night Rule** (rule-dark): hairline dividers between service rows on navy.
- **Signal Red** (error): inline error sentences and the error border.

### Named Rules
**The Gold-Is-A-Fill Rule.** Gold is a fill colour. Text on gold is always Night Navy. Gold as text on paper or light uses Burnished Gold Ink; bright gold text appears only on navy grounds and the hero.

**The Never-Black Rule.** The logo's black ground becomes Night Navy. No band, overlay or footer uses black.

**The Two Ring Rule.** Focus is Electric Form Blue on light grounds and gold on navy grounds (hero, navy bands, footer), always a 3px outline with a 2-3px offset.

## Typography

**Display Font:** Cal Sans (Google Fonts, with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** One rounded, geometric display face at a single regular weight does all the speaking. The system body face stays out of its way.

### Hierarchy
- **Display** (400, clamp 44-84px, line-height 1.02): the hero H1 only, white on the photo, max 12ch on phones and 15ch on desktop, balanced wrapping.
- **Headline** (400, clamp 30-48px, 1.08): section H2s.
- **Title** (400, 22px, 1.2): step titles. Service rows (clamp 21-26px, 1.15) and the Facebook row (clamp 19-22px, 1.2) sit at the same step.
- **Control** (400, 18px, line-height 1): buttons, form labels and legends, the header phone number. The header wordmark is 22px (26px on desktop) and the closing phone number scales to clamp 30-52px.
- **Lede** (system, clamp 17-19px, 1.7): the sentence under a section heading, max 40ch. The hero promise is a sibling at clamp 17-20px / 1.5, max 30ch on phones.
- **Body** (system, 16px, 1.7): running text, inputs and chips (16px so iOS never zooms).
- **Label** (system, 14px): hints, the line under the submit, and the eyebrow (at 500 weight, letter-spacing .02em).

### Named Rules
**The One Weight Rule.** Cal Sans is only ever set at 400. Emphasis comes from size and colour (the gold accent phrase), never from bold display type.

**The Bounce-Once Rule.** Only the hero H1 animates its letters: each slides in 50px from the right over 1s with an overshoot curve (`cubic-bezier(.34,1.56,.64,1)`), 20ms apart. Then the plain heading is restored. Nothing else animates its text, and reduced motion or no JS shows the plain heading at once.

## Layout

The page is one centred column (max 1160px) with a 20px gutter on phones that widens to 40px from 760px. Sections are full-bleed bands with 64px of vertical padding on phones and 96px from 760px. The bands run paper header, photo hero, paper (proof), navy (services), paper (care), light (quote), navy (close), then the textured deep footer.

Within a section, a heading group stacks at 16px gaps (max 640px wide) and lists start 32-36px below it. From 760px the before/after pairs and service rows go to two columns (20px and 48px gaps) and the hero actions sit side by side at a 230px minimum. From 1024px the care and quote sections split into two columns with a 64px gap, and the quote heading becomes sticky beside the form. The hero copy has 56px above and 72px below on phones, and 112px / 128px on desktop.

**The Band Alternation Rule.** Adjacent sections never share a ground; a new section is announced by a change of band, not by a divider or heading ornament.

## Elevation & Depth

The system is flat. Depth comes from band contrast, the hero's navy veil over the photograph (a vertical gradient of Night Navy from 72% to 90% opacity), and the faint 135deg line texture on deep-navy grounds (1px white lines at 3.5% opacity every 23px, never stronger than about 4%). Only one element is lifted.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,20,42,.32)`): the floating text circle only, because it sits over moving content.

### Named Rules
**The One Lift Rule.** Cards, buttons, rows and chips carry no shadow at rest or on hover. The floating circle is the only shadowed object.

## Shapes

There are three radii and one circle. Containers (the form card and before/after frames) use 24px corners; inputs use 10px; buttons, chips and the eyebrow are full pills. Icon wells are perfect circles: the 44px arrow well, the 48px step number and the 60px floating button. Borders are absent at rest. Controls use a 2px transparent border that colours on hover, focus or error. The only hairlines are the dividers between service rows. The Facebook row is a 20px-radius navy slab, a step softer than the cards. Icons are inline SVG line drawings (2.2-2.6 stroke, round caps), and the brand marks are filled.

## Components

### Buttons
Big, round and quiet until touched.
- **Shape:** full pill, 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** gold fill, Night Navy text, matching gold border. It is the only filled action in a view.
- **Hover / Focus:** hover (real pointers only) brightens to gold-2. Press scales to .98. Focus is the band's ring (see The Two Ring Rule). In the form the full-width submit also takes a blue outline on hover, matching the other controls.
- **Ghost:** transparent with a 2px Moonlight border at 70%. On hover the border goes solid white over a 10% white wash. Used on dark grounds only, as the secondary of the pair.

### Chips
- **Style:** Field Mist pill, 48px tall, system 16px Night Navy text, 2px transparent border. They are radio inputs, visually hidden behind labels.
- **State:** hover colours the border Electric Form Blue. Selected fills Night Navy with white text. Keyboard focus is a blue 3px outline with a 2px offset (never a border, which vanishes on the navy fill).

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** the form card is Card White on the light band. Before/after frames are Night Navy, showing as a 4px seam between the two photos.
- **Shadow Strategy:** none (see The One Lift Rule).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px) on the form card. Photo frames are full-bleed to their rounded edge.

### Inputs / Fields
- **Style:** Field Mist fill, no visible border, 10px radius, 52px minimum height (110px for the textarea), system 16px Night Navy text, Soft Slate placeholder. Labels sit above in Cal Sans 18px, and the optional hint is a 14px Soft Slate aside.
- **Focus:** the 2px border turns Electric Form Blue, and hover does the same on real pointers.
- **Error:** the border turns Signal Red and stays red while focused. A plain-sentence error line appears below in Signal Red.

### Navigation
- **Header:** slim paper bar (64px, 76px on desktop). The two-line wordmark (Cal Sans "TIP TOP" over an 11px uppercase gold-ink "Customz") is on the left and the tap-to-call number with a gold-ink phone icon is on the right. There is no menu.
- **Footer:** Night Navy with the line texture. Moonlight Soft text, Moonlight links at 44px tap height that turn gold on hover.

### Service Rows (signature)
Each row on the navy band is one link: Cal Sans clamp 21-26px Moonlight text, at least 68px tall, separated by Night Rule hairlines, with a 44px arrow well (white at 12%) at the right edge. They are one column on phones and two from 760px.

**The Arrow-Only Hover Rule.** On hover or focus a row or the Facebook slab changes nothing but its arrow well, which fills gold with a Night Navy arrow. Keyboard focus adds a gold ring around the well.

### Before / After Pair (signature)
Two 4:5 photographs side by side in a 24px-radius Night Navy frame with a 4px seam. Each has a white Cal Sans 16px "Before" / "After" label on a bottom gradient to Night Navy at 85%. The photographs are the client's own (frames from their Facebook post video), and nothing is captioned below.

### Floating Text Circle (signature)
A 60px gold circle with a Night Navy chat icon, fixed 16px from the bottom-right safe area. It slides up (`.35s cubic-bezier(.2,.8,.2,1)`) once the hero has left the screen, and slides away while the quote form is visible, so the two text actions are never on screen together. When hidden it is removed from the tab order.

### Eyebrow (house exception, not an Impeccable rule)
A quiet 14px pill label with a 7px gold dot, on a 6% Night Navy tint (12% white on dark grounds). It sits above the hero H1 and two section headings. It is included because Ellie chose it for the house style (calm-photo-style.md item 5, 2026-10-19) against Impeccable's anti-eyebrow rule. It is not a rule this system creates. If used, it keeps the house limits: a `<p>`, never a heading; no hover, arrow, shadow or solid gold fill; and on a few key headings only.

### Motion
Content that starts below the first screen rises 12px and fades in over 400ms (ease-out) as it enters. Everything is visible at rest, without JS and under reduced motion. Reduced motion also removes button, float and scroll transitions.

## Do's and Don'ts

### Do:
- **Do** take the navies and the accent from the client's logo, and keep the page ground paper (#f4f6fb), never black.
- **Do** put Night Navy text on every gold fill, and switch to gold-ink (#85601a) whenever gold must be read on paper or light.
- **Do** set every heading, button, label and phone number in Cal Sans at 400; keep running text in the system stack at 16px / 1.7.
- **Do** alternate full-bleed bands (paper, navy, light, deep navy with the 135deg texture at about 3.5% white) so each section is announced by its ground.
- **Do** use only the three radii (10px field, 24px card, pill) plus perfect circles for icon wells.
- **Do** show the client's own photographs, `object-fit: cover`, under a Night Navy gradient wherever text sits on them.
- **Do** keep every tap target at 44px or more (buttons 56px, chips 48px, rows 68px).

### Don't:
- **Don't** put white text on gold or bright gold text on paper; both fail contrast.
- **Don't** add shadows to cards, buttons, chips or rows; the floating circle is the only lifted object.
- **Don't** give inputs a visible border at rest; the field fill is the affordance, and the border appears on hover, focus or error.
- **Don't** use bold Cal Sans or a second display face.
- **Don't** animate letters on any heading but the hero H1, and don't hide content at opacity 0 for anyone who has not scrolled to it.
- **Don't** change a service row's background, underline or text on hover; only the arrow well fills.
- **Don't** replace the floating circle with a sticky bottom bar.
- **Don't** fill with Electric Form Blue; it is an outline and caret colour for controls only.
