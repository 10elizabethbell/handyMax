---
name: HandyMax
description: A calm, banded one-page site for a one-man New Jersey handyman; paper and navy bands, one job-site yellow, his own finished room in the hero.
colors:
  job-site-yellow: "#ffc83a"
  job-site-yellow-light: "#ffd665"
  yellow-ink: "#8a5a00"
  beanie-navy: "#1d3f73"
  deep-navy: "#0f2340"
  ink: "#12233f"
  body-slate: "#2a3a4c"
  soft-slate: "#4a5868"
  paper: "#f4f6fb"
  card-white: "#ffffff"
  field-tint: "#e6ecf5"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  rule-on-dark: "rgba(255,255,255,.12)"
  error-red: "#b3261e"
typography:
  display:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "clamp(19px, 5.2vw, 22px)"
    fontWeight: 400
    lineHeight: 1.2
  button:
    fontFamily: "\"Cal Sans\", \"Avenir Next\", \"Segoe UI\", system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.02em"
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  stack: "16px"
  section: "64px"
  section-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.job-site-yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.job-site-yellow-light}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-field:
    backgroundColor: "{colors.field-tint}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field-tint}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "44px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card-white}"
  card-form:
    backgroundColor: "{colors.card-white}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    height: "64px"
  step-number:
    backgroundColor: "{colors.job-site-yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.job-site-yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: HandyMax

## Overview

**Creative North Star: "Calm Order, Roof to Basement"**

HandyMax is a one-person handyman's site in Ellie's house calm band style (default since 2026-10-19, learned from lpmr.co.uk). It earns trust through order rather than spectacle: full-bleed bands alternate between cool off-white paper and two navies, so each new section is obvious; one job-site yellow is the only warm colour and it is used as a fill; shapes are soft and borderless. The real material is Max himself: his own finished dining room behind the promise, his face, his first-person words.

Density is low on the phone: one column, a 20px gutter, 64px between bands, and every tap target 44px or more. On desktop the same bands widen to a 1160px column with 96px band padding and simple two-column splits. Motion is limited to three things: the hero H1 letters bounce in once, content below the first screen rises 12px into place, and the floating text circle slides up after the hero.

This replaces the earlier cutaway-house world entirely (redesign, not refinement); that world survives only in git history (7c9efb4) and `demos/`.

**Key Characteristics:**
- Paper / beanie navy / paper / deep navy (lined) / paper / navy / paper / navy band rhythm, deep-navy footer.
- One warm accent, job-site yellow, as fills: primary buttons, step numbers, the slider bar and knob, arrow circles on hover, the floating circle.
- Cal Sans at weight 400 for every heading, button, row and phone number; the system stack at 16/1.7 for reading.
- Borderless soft shapes: 24px cards, 10px tinted fields, full pills.
- Flat bands; only the two yellow controls that sit over other content cast a shadow.
- Bilingual: every visible string exists in English and Spanish, toggled in the header.

### Direction contract (verbatim, top of `<body>` in index.html)

> THESIS: A one-man handyman's site that earns trust through calm order (after lpmr.co.uk): Max's own finished room behind the promise, his face and his words, one list of jobs, one way to ask for a free estimate, in English or Spanish.
>
> OWN-WORLD: Off-white paper, beanie navy (#1d3f73) and deep navy (#0f2340, faint diagonal lines) bands, job-site yellow (#ffc83a) as the one warm accent (fills only; #8a5a00 when it has to be text on light). Cal Sans display, system body at 16/1.7.
>
> STORY: The visitor sees who fixes homes in New Jersey, meets Max, sees the whole list of what he does, sees a room he redid, and texts or calls him for a free estimate.
>
> FIRST VIEWPORT: Paper header with the HandyMax wordmark left, Español toggle and tap-to-call number top right. Hero: his own dining room after the job (recessed lights, new fixture) under a navy overlay; eyebrow "Handyman & electrical", "Roof to basement in New Jersey.", one promise line, two pill buttons (Get a free estimate, Text Max).
>
> FORM: fixed by pitch-site calm-photo-style.md (house default since 2026-10-19), no concept roll and no seed key; one real photo in the hero; the earlier cutaway-house world is in git history (7c9efb4) and demos/.
>
> FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, DESIGN.md, and every shipping raster carrying its provenance

Divergence: the contract's FIRST VIEWPORT says the hero eyebrow reads "Free estimates"; the build ships "Handyman & electrical" / "Handyman y electricista" (changed in af11b17). The build wins.

### Imagery and provenance

There is no logo and no brand palette. The navy comes from Max's beanie in his profile photo; the yellow is job-site yellow carried over from the first build. Every photo is Max's own, sourced from his Facebook, with a `.json` provenance sidecar beside it:

- `img/hero.webp` (940x850): the "After" half of his dining-room before/after post (recessed lights, new ceiling fixture), cropped to drop a person reflected in the glass door and the baked-in label; native resolution, WebP q74. Sits under a navy overlay.
- `img/before.webp`, `img/after.webp` (980x850 each): the two halves of the same post, labels cropped off; the before/after slider.
- `img/max.webp` (580x580): his Facebook profile picture, cropped above the printed contact text.
- `og.jpg` (1200x630): a screenshot of the shipped hero (regenerated in 9a23036 without the line texture over the photo). Not generated art.
- `icon.svg` and `apple-touch-icon.png` (180x180): the site's own lettering standing in for a logo; a roof chevron and an "H" stroked in ink (#12233f) on a yellow rounded square (rx 14 of 64).

Photos are real, never stretched (`object-fit: cover` only), sized to display, and carry provenance; new rasters follow the same rule.

## Colors

Cool paper and two navies carry the page; one job-site yellow is the only warm note, and it is a fill, never text on light.

### Primary
- **Job-Site Yellow** (`job-site-yellow`): the single warm accent, fills only. Primary buttons, numbered step discs, the before/after divider bar and knob, the floating text circle, arrow circles on hover/focus, the 7px eyebrow dot, text selection, and the focus ring on dark bands. Text on it is always Ink. It also colours the last phrase of a heading on dark bands ("New Jersey.", "do.", "works.") and the phone icon in the closing band.
- **Light Yellow** (`job-site-yellow-light`): primary button hover fill only.
- **Yellow Ink** (`yellow-ink`): the accent when it must be text or an icon on a light ground: "Max" in the wordmark, the header phone icon, header phone hover. About 5.5:1 on paper.

### Secondary
- **Beanie Navy** (`beanie-navy`): the mid navy. The hero ground and overlay tint, the How-it-works and closing bands. Also the focus/hover outline colour on light grounds (form fields, chips, slider, submit button) and the field caret.
- **Deep Navy** (`deep-navy`): the darker band, always with the line texture. The services band and the footer. Its rgb (15,35,64) also tints the hero overlay gradient and the before/after tags.

### Neutral
- **Paper** (`paper`): page ground, header, and the light bands; also `theme-color`.
- **Card White** (`card-white`): the estimate form card and the Facebook card on paper; white text on the hero H1, selected chips and slider tags.
- **Field Tint** (`field-tint`): fill for inputs, textareas and chips on the white card, and the placeholder behind photos while they load. Exists because paper-on-white fields measured about 1.08:1.
- **Ink** (`ink`): headings on light, text on yellow, the selected-chip fill.
- **Body Slate** (`body-slate`): running text on light.
- **Soft Slate** (`soft-slate`): ledes, hints, notes, placeholders, "(optional)" and the desktop wordmark subtitle on light.
- **On Dark** (`on-dark`): headings, rows, step titles and buttons on navy bands.
- **On Dark Soft** (`on-dark-soft`): running text and ledes on navy bands.
- **Rule on Dark** (`rule-on-dark`): the hairline between service rows; the same 12% white is the eyebrow fill on dark.
- **Error Red** (`error-red`): inline error sentences and the invalid-field border.

### Named Rules
**The Fill-Only Yellow Rule.** Job-site yellow is a fill. On light grounds, text or icons in the accent use Yellow Ink; on yellow, text is Ink. Never white on yellow, never yellow text on paper.

**The Dark-Band Accent Rule.** A heading's closing phrase goes yellow only on the hero and navy bands. Headings on paper stay all Ink.

**The Faint Line Rule.** The diagonal texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`) lives on deep-navy bands and the footer, at 3.5% white or fainter, so it never reads as lines through text. It is never visible over the hero photo.

## Typography

**Display Font:** Cal Sans (Google Fonts, `display=swap`, preconnected), falling back to Avenir Next, Segoe UI, system-ui
**Body Font:** the system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** One friendly geometric display face at a single weight does all the talking (headings, buttons, service rows, phone numbers, form labels); the native system face does the reading. Hierarchy comes from size, not weight.

### Hierarchy
- **Display** (Cal Sans 400, clamp 42-80px, 1.02): the hero H1 only, white, max 11ch, letter-by-letter bounce-in.
- **Headline** (Cal Sans 400, clamp 30-48px, 1.08, -0.005em, balanced wrap): every section H2.
- **Title** (Cal Sans 400, clamp 19-22px, 1.2): service rows, the Facebook card, step titles (21px, 22px on desktop), form labels and legends (17px).
- **Button** (Cal Sans 400, 18px, 1): every pill button. The header phone number uses the same face at 17px (20px desktop); the closing-band phone at clamp 32-52px.
- **Lede** (system 400, clamp 17-19px, max 38ch): the one sentence under a section heading. The hero promise is the same voice at clamp 17-20px, 1.5, in On Dark.
- **Body** (system 400, 16px, 1.7): all running text, max 60ch in the About block. Inputs are 16px so iOS never zooms.
- **Label** (system 500, 14px, 0.02em): eyebrow pills and slider tags. Hints and notes are system 15px in Soft Slate.

### Named Rules
**The One Weight Rule.** Cal Sans is only ever set at 400. Emphasis comes from size and colour (the yellow closing phrase), never bold display.

**The Letters-Once Rule.** Only the hero H1 animates letter by letter. No other heading gets a reveal.

## Layout

Single 1160px centred column (`wrap`) with a 20px gutter on phones and 40px from 760px. Bands are full-bleed with 64px vertical padding, 96px from 760px. Section heads are a left-aligned stack (16px gap, max 640px wide): optional eyebrow, H2, lede.

Breakpoints: up to 370px the header tightens (smaller wordmark and phone, phone icon hidden); from 760px the header grows to 76px, the wordmark subtitle appears and hero buttons sit side by side (min 240px each); from 1024px the hero photo takes the right 60% beside solid navy copy (min-height 620px), About becomes a 300px portrait plus text, service rows go two columns (56px column gap), the before/after slider sits beside a vertically centred heading, hint and Facebook card, the form sits beside a sticky heading, the closing band puts the big phone number bottom-right, and the three steps sit in a row.

Spacing rhythm: 16px stack inside heads, 20-28px between hero and section parts, 22px between form fields, 64px column gaps on desktop splits. Hover styles live only inside `(hover: hover)` so taps never leave them stuck.

## Elevation & Depth

Flat by default. Depth comes from band colour (paper against navy against deep navy) and from white cards sitting on paper, not from shadow. Only the two yellow controls that sit on top of other content cast a soft navy shadow.

### Shadow Vocabulary
- **Slider knob** (`box-shadow: 0 6px 16px rgba(8,20,40,.35)`): the yellow knob on the before/after photo.
- **Floating circle** (`box-shadow: 0 10px 28px rgba(8,20,40,.3)`): the fixed text circle over the page.

### Named Rules
**The Flat Band Rule.** Bands, cards, rows, fields and buttons carry no shadow at rest or on hover. A shadow means the control floats over something else.

## Shapes

Soft and borderless. Cards and photo frames round at 24px, fields at 10px, and buttons, chips, eyebrow pills, slider tags, arrow circles, step discs and the floating circle are full pills or circles. Fields and chips have a 2px transparent border that only takes colour on hover, focus or error. The only drawn lines are the 1px service-row hairlines on deep navy and the 4px yellow slider bar. Photos are clipped by their rounded frame and fill it with `object-fit: cover`.

## Components

### Buttons
Pill-shaped, tall and plain; at most two side by side.
- **Shape:** full pill (999px), 56px tall, 26px side padding, optional 20px icon left of the label.
- **Primary:** yellow fill, Ink label in Cal Sans 18px. Full width on phones and in the form.
- **Hover / Focus:** primary lightens to Light Yellow; the form's submit also gains a 3px navy outline at 3px offset. Pressing scales to 0.98. Focus is a 3px outline (navy on light, yellow on dark).
- **Ghost:** transparent with a 2px 70%-white border and On Dark label, for the secondary hero action; hover turns the border solid white with a 10% white fill.

### Chips
- **Style:** Field Tint pill, 44px tall, 16px padding, Ink system 15px, 2px transparent border. Real checkboxes, visually hidden.
- **State:** selected fills Ink with white text; hover adds a 2px navy outline at 2px offset; keyboard focus a 3px navy outline. A chip ticked by tapping a service row flashes a 3px yellow outline for 1.4s.

### Cards / Containers
- **Corner Style:** 24px (form, portrait, slider, Facebook card).
- **Background:** Card White on paper; Field Tint behind photos while they load.
- **Shadow Strategy:** none (see The Flat Band Rule).
- **Border:** none.
- **Internal Padding:** clamp 20-32px for the form; 14-22px for the Facebook card.

### Inputs / Fields
- **Style:** Field Tint fill, no visible border (2px transparent), 10px radius, 13px 14px padding, 52px min height (textarea 110px, vertical resize). Labels above in Cal Sans 17px Ink; "(optional)" in system 14px Soft Slate.
- **Focus:** the border turns Beanie Navy; hover does the same.
- **Error:** border turns Error Red and stays red while focused; the error is a plain sentence in red system 16px under the field.

### Navigation
- **Header:** paper, 64px (76px desktop). Wordmark "Handy" + "Max" in Cal Sans 22-25px, "Max" in Yellow Ink, with a small uppercase subtitle on desktop. Right side: the language toggle (underlined system 15px, "Español" / "English", JS only) and the tap-to-call number in Cal Sans with a Yellow Ink phone icon. No menu.
- **Footer:** deep navy with line texture; name, area, phone, email (its only appearance) and Facebook as 44px links that turn yellow on hover.

### Service Rows
The whole list of jobs on deep navy, each row a link that ticks the matching chip in the form. Cal Sans title, 64px min height, hairline above each row, a 44px arrow circle (10% white) on the right. Only the arrow changes on hover/focus: it fills yellow with an Ink arrow. One column on phones, two on desktop.

### Before/After Slider
A 980:850 photo frame at 24px radius with the after photo clipped from a draggable point. A 4px yellow bar and a 48px yellow knob (Ink chevrons, the knob shadow) mark the split; "Before"/"After" tags are 82% deep-navy pills with white 14px text. Drag, tap or arrow keys; vertical drags still scroll. Followed by a white Facebook card whose arrow circle fills yellow on hover.

### Numbered Steps
Three steps on beanie navy, each with a 48px yellow disc holding the CSS-counter number in Cal Sans 20px Ink, a Cal Sans title in On Dark and a sentence in On Dark Soft.

### Hero
Max's dining room (`img/hero.webp`) fills the band under a deep-navy vertical gradient (62% to 88%) on phones; from 1024px the photo sits at the right 60% and a horizontal navy gradient (solid to 40%, 50% at the edge) holds the copy on solid colour. Copy: eyebrow, the Display H1 with its last phrase in yellow, the promise line, then the primary and ghost buttons. No call button in the hero; the number stays in the header.

**Bounce-in:** JS splits the visible-language H1 into letters inside no-wrap word spans; each letter goes from `opacity:0; translateX(50px)` to rest over 1s with `cubic-bezier(.34,1.56,.64,1)` (the overshoot), 20ms apart. It waits for Cal Sans (600ms cap) so letters don't land in the fallback face. The H1 carries an `aria-label` while split, and the plain heading is restored when the last letter lands or the language changes. Skipped entirely under reduced motion or without JS.

### Fade-up
Elements marked to rise are visible at rest. Only those starting below the first screen are hidden by JS, then move up 12px and fade in over 400ms ease-out when they enter. Nothing waits at opacity 0 without JS or under reduced motion.

### Floating Text Circle
One 60px yellow circle, bottom right (16px plus safe-area insets), Ink chat icon, opening a pre-written `sms:` in the current language. It slides up 120px into view (350ms, `cubic-bezier(.2,.8,.2,1)`) once the hero leaves and hides while the form is on screen; when hidden it is `tabIndex=-1` and `aria-hidden`. Focus draws a white outline plus an Ink ring.

### Eyebrow Pill (scoped exception)
A quiet 14px label pill (6% ink on light, 12% white on dark, a 7px yellow dot) shipped above three headings: the hero H1, "What I do." and the estimate form. It is a `<p>`, not a heading, with no arrow, hover or shadow. It exists because Ellie chose LPMR-style pills for the house style on 2026-10-19, against the craft floor's ban on eyebrows (the conflict is logged in HANDOFF.md). It is recorded here because it ships, not as a pattern: do not add eyebrows to new headings or new surfaces without Ellie's explicit call.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed paper and navy bands so every section change is obvious, with deep navy carrying the faint line texture.
- **Do** use job-site yellow as a fill with Ink text on it, and Yellow Ink whenever the accent has to be text or an icon on paper.
- **Do** set every heading, button, row and phone number in Cal Sans at 400, and running text in the system stack at 16px / 1.7.
- **Do** keep shapes borderless and soft: 24px cards, 10px Field Tint fields, full pills for buttons and chips.
- **Do** outline form controls in Beanie Navy on hover and focus, and keep the error border red while focused.
- **Do** keep every tap target at 44px or more, and hover styles inside `(hover: hover)`.
- **Do** write every visible string in English and Spanish and let the toggle swap them, including aria-labels, placeholders, SMS bodies and the page title.
- **Do** use only Max's own photos, cropped with `object-fit: cover`, each with a provenance `.json`.

### Don't:
- **Don't** put white text on yellow or yellow text on paper.
- **Don't** colour a heading's closing phrase yellow on a paper band.
- **Don't** add shadows to bands, cards, rows, fields or buttons; only controls floating over content get one.
- **Don't** animate any heading other than the hero H1, and don't let fade-up content sit hidden without JS or under reduced motion.
- **Don't** turn the floating circle into a bottom bar or show it while the form is in view.
- **Don't** strengthen the line texture beyond 3.5% white or show it over the hero photo.
- **Don't** change anything on a service row's hover except its arrow circle.
- **Don't** put a call button in the hero; the number lives in the header and the closing band.
