---
name: HandyMax
description: A living-room wall at night whose recessed downlights the visitor switches on with a finger.
colors:
  night-wall: "#16233b"
  night-wall-raised: "#1c2c49"
  ceiling-band: "#101a2e"
  wall-rule: "#2b3d5f"
  can-trim: "#2c3c5c"
  warm-paper-text: "#f4ede2"
  cool-dusk-text: "#c3cbdb"
  downlight-amber: "#ffb238"
  downlight-amber-bright: "#ffc76b"
  lit-plaster: "#efe5d3"
  plaster-field: "#fbf7ef"
  plaster-edge: "#cfc2aa"
  switch-plate: "#e9e1d2"
  navy-ink: "#17223a"
  slate-ink: "#4a5266"
  form-blue: "#2f6bff"
  error-red: "#b3261e"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 96px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(34px, 9vw, 64px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  body-large:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "19px"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.5
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.5
rounded:
  switch: "8px"
  field: "12px"
  frame: "18px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "32px"
  container: "1160px"
  section-phone: "72px"
  section-desktop: "96px"
  stack-sm: "12px"
  stack-md: "22px"
  stack-lg: "28px"
  column-gap: "56px"
components:
  button-primary:
    backgroundColor: "{colors.downlight-amber}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
    typography: "{typography.label}"
  button-primary-hover:
    backgroundColor: "{colors.downlight-amber-bright}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.warm-paper-text}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
    typography: "{typography.label}"
  button-send:
    backgroundColor: "{colors.navy-ink}"
    textColor: "{colors.lit-plaster}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.warm-paper-text}"
    height: "62px"
    padding: "8px 0"
  service-row-arrow:
    backgroundColor: "{colors.night-wall-raised}"
    rounded: "{rounded.pill}"
    size: "40px"
  service-row-arrow-hover:
    backgroundColor: "{colors.downlight-amber}"
  chip:
    backgroundColor: "{colors.plaster-field}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.navy-ink}"
    textColor: "{colors.lit-plaster}"
  input-text:
    backgroundColor: "{colors.plaster-field}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "56px"
  photo-frame:
    backgroundColor: "{colors.night-wall-raised}"
    rounded: "{rounded.frame}"
---

# Design System: HandyMax

## Overview

**Creative North Star: "The Room When the Lights Come On"**

The whole page is one wall in a living room at night. A darker ceiling band runs across the top holding recessed can lights; each can throws a real downlight scallop (a parabola-edged wash of 2700K amber) onto deep navy plaster, with dust drifting in the beam. The visitor's finger or mouse brings the nearest cans up, a wall switch turns every light on, and when nobody touches anything the cans sweep on by themselves. Lower on the page the light-row returns as a ceiling over each major section, and at the estimate section the beams finally "reveal" the wall itself: the background turns into lit warm plaster. That turn from night wall to lit wall is the page's story (Max's before/after is literally a dim room turned bright) and it is the one place the ground changes.

Everything else stays plain and heavy so the light carries the craft: the system font stack set in 900-weight uppercase for display, sentence-case body in warm off-white, one amber accent, generous phone-first spacing, and photos framed as softly rounded, shadowed pictures hanging on the wall. The system is governed by Ellie's pitch-site house rules (`ellie-taste.md`, `finishing-rules.md`); the constraints those rules place on contact, hover and form behavior are recorded here as part of the system, not as page-local choices.

Confirmed rejections: the contractor template (toolbelt stock photography, icon cards, a blue-and-orange "pro" bar), black page grounds, thin decorative highlight lines, and any sticky bottom action bar.

**Key Characteristics:**
- Night-navy ground with a darker ceiling band; never black.
- Light is rendered, not drawn: canvas downlight scallops and dust, interactive by finger and mouse.
- Amber is the only accent and means "light"; blue exists only inside the estimate form for hover and focus.
- System sans, heavy uppercase display, sentence-case body.
- Pill-shaped controls, 18px-rounded photo frames, hairline rules between list rows.
- Phone first: 56px controls, full-width stacked CTAs on phones, contact by text message and tap-to-call.

## Colors

A two-ground palette (night wall and lit plaster) with a single warm accent standing in for the light itself.

### Primary
- **Downlight Amber** (`downlight-amber`): the color of the light. Primary button fill, the lit word in the hero headline ("Wires gone."), the "Max" half of the wordmark, phone glyphs, step numerals, the before/after divider and knob, the filled arrow circle on hover, focus rings on the night wall, and text selection. Its hue matches the canvas sprite's 2700K beam (rgb 255,196,122) so type and light read as one source.
- **Bright Amber** (`downlight-amber-bright`): the hover state of anything amber (primary button, phone links, footer links). A light turned up, never a new hue.

### Secondary
- **Form Blue** (`form-blue`): hover borders, focus borders, focus rings (22-30% alpha halo) and the caret, used only on controls inside the estimate form. It exists because the form's primary button is already a fill and amber would not stand out from plaster as a focus signal.

### Neutral
- **Night Wall** (`night-wall`): the page ground, theme color, and the darkness the estimate reveal canvas paints above the lit plaster.
- **Raised Night** (`night-wall-raised`): resting fill of the arrow circles and the photo frame's loading ground; the only "surface" on the night wall.
- **Ceiling Band** (`ceiling-band`): the 64px header strip that holds the cans.
- **Wall Rule** (`wall-rule`): 1px row dividers and the footer's top rule.
- **Can Trim** (`can-trim`): the trim ring drawn around each recessed can lens on canvas.
- **Warm Paper** (`warm-paper-text`): primary text on the night wall; warm so it sits inside the amber light.
- **Dusk Gray** (`cool-dusk-text`): secondary text on the night wall (ledes, hints, step descriptions, footer, the language toggle).
- **Lit Plaster** (`lit-plaster`): the estimate section ground, and text on navy-ink buttons and selected chips.
- **Plaster Field** (`plaster-field`): fill of text inputs and unselected chips; a step lighter than the plaster so fields read as set into the wall.
- **Plaster Edge** (`plaster-edge`): 2px resting border on inputs and chips.
- **Switch Plate** (`switch-plate`): the hero's wall-switch plate (with its rocker and screw tones derived from it).
- **Navy Ink** (`navy-ink`): text on plaster and on amber; the send button and selected chip fill.
- **Slate Ink** (`slate-ink`): secondary text on plaster (lede, notes, "(optional)").
- **Error Red** (`error-red`): inline form error text only.

### Named Rules
**The One Light Rule.** Amber is the only accent on the page and it always means light: the beam, the lit word, the knob, a filled arrow. Never introduce a second decorative hue.

**The Blue Stays In The Form Rule.** Form Blue appears only on estimate-form controls (inputs, chips, the send button) and only on hover or focus. Service rows, links and buttons on the night wall never use it.

**The No Black Rule.** The darkest value on the page is the ceiling band. No pure or near-black grounds anywhere.

**The Hover Brings The Accent Rule.** Interactive elements are neutral at rest and take amber on hover (arrow circles fill, links brighten). Amber at rest is reserved for content that represents light (the lit headline word, numerals, the divider) and the primary button.

## Typography

**Display Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same system stack

**Character:** One family at two extremes: black-weight uppercase display set tight (-0.02em, 0.95 line-height) that reads like painted signage, against plain sentence-case body. Mandated by the house style (`ellie-taste.md` section 2): fast on cellular and proven on prior builds.

### Hierarchy
- **Display** (900, clamp 40-96px, 0.95, uppercase): the hero headline only, two short stacked lines with the second in amber. The closing wordmark uses the same treatment one step larger on phones (clamp 52-96px, 16vw).
- **Headline** (900, clamp 34-64px, 0.95, uppercase, balanced wrap): section headings.
- **Title** (800, 22px, uppercase, -0.01em): step titles. Step numerals sit beside them at 900 / 44px in amber.
- **Body Large** (400-700, 19px, 1.5): section ledes, service row labels (700), Max's paragraph (max 30em), closing lines.
- **Body** (400, 17px, 1.5): default text; the hero promise scales 17-20px and stays within 34em.
- **Label** (800, 17px): buttons, form labels, the phone number (16px, tabular figures).
- **Small** (400-800, 15px): hints, notes, "(optional)", errors, the before/after tags (800, uppercase, 0.04em).

### Named Rules
**The Heavy Caps Only Rule.** Uppercase is for display, headlines, step titles and the photo tags. Body, labels, buttons and form copy stay sentence case.

**The 16px Floor Rule.** Body text never drops below 17px and nothing readable goes under 15px; inputs stay at 17px so phones never zoom.

## Layout

Phone first (designed at 360-430px). A single centered container (`container`, 1160px max) with 20px gutters on phones and 32px from 700px up. Sections breathe on a 72px (phone) / 96px (desktop) vertical rhythm; sections that carry a light-row ceiling get extra top padding so the scallops have room above the content (work 120/150px, estimate 150/180px, close 150/180px).

The hero is a full-height room (clamped 560-880px, 800px max on desktop): the 64px ceiling band holds the header, and the content is bottom-anchored (headline, promise, two CTAs) so the lit wall above it stays clear. CTAs stack full width on phones and sit side by side from 700px.

Breakpoints: 700px (wider gutters, two-column service rows, side-by-side CTAs) and 1024px (before/after beside its heading, portrait beside text, three-column steps, estimate heading beside the form). A 380px step tightens the header for small phones. Inside components, gaps step through 10, 12, 16, 22, 26 and 28px; desktop columns separate by 56-64px.

### Named Rules
**The First Screen Rule.** The first phone screen shows wordmark, language toggle and phone number in the header; the benefit headline, the owner's promise, and at most two buttons. No services list, service area, or call button in the hero.

**The Clear Wall Rule.** Nothing in the scene runs through text: scallops fall from the ceiling band and fade before the bottom-anchored copy, and the wall switch sits on the right edge away from the headline.

## Elevation & Depth

Depth comes from light, not from stacked surfaces. The ground is flat navy; the canvas downlights add the only atmosphere (additive "lighter" compositing on the night wall, scallops fading with distance, dust lit only where it is inside a beam). Physical objects hanging on the wall (the switch plate, the before/after frame, the portrait) cast soft, downward, navy-tinted shadows as if lit from the ceiling. Controls are flat; no shadows on buttons, rows or chips.

### Shadow Vocabulary
- **Hung frame** (`box-shadow: 0 30px 60px -28px rgba(5,10,20,.85)`; portrait uses `-24px` spread and `.9`): photos hanging on the wall.
- **Wall fixture** (`box-shadow: 0 10px 18px -6px rgba(5,10,20,.65), 0 2px 4px rgba(5,10,20,.35)`): the switch plate.
- **Knob** (`box-shadow: 0 6px 16px rgba(5,10,20,.45)`): the before/after drag knob.
- **Form focus halo** (`box-shadow: 0 0 0 3px rgba(47,107,255,.22)`; `.3` on the send button): focus only, inside the form.

### Named Rules
**The Lit From Above Rule.** Every shadow falls downward and is tinted with the night (rgba 5,10,20), never neutral gray and never a hard offset.

**The No Glint Rule.** No hairline highlights, sheens or films over surfaces or photos.

## Shapes

Soft and domestic. Every control is a full pill (`pill`): buttons, chips, the Facebook link, arrow circles, the drag knob. Photos sit in 18px-rounded frames (`frame`); inputs are 12px (`field`); the switch plate is 8px (`switch`). The only lines are 1px Wall Rule dividers between service rows and above the footer, and the 4px solid amber before/after divider. Circles appear only where something is pressable or a light source (arrow circles, knob, can lenses as flattened ellipses).

## Components

### Buttons
Confident, chunky pills that match in pairs.
- **Shape:** full pill (`pill`), 56px minimum height, 2px border, 800-weight 17px label.
- **Primary:** amber fill with navy ink text; hover brightens to Bright Amber (fill and border).
- **Outline (secondary):** transparent with the same 2px amber border and the same height; hover adds a 12% amber wash. Primary and outline always share outline width and height.
- **Send (on plaster):** navy ink fill with plaster text; hover and focus switch the border to Form Blue with a blue halo.
- **Press:** every button nudges down 1px on `:active`. Transitions 0.2s on color, 0.15s on transform.

### Chips
- **Style:** choice chips in the estimate form only. Plaster Field fill, 2px Plaster Edge border, 46px pill, 700 / 16px.
- **State:** hover turns the border Form Blue; selected becomes a navy-ink fill with plaster text (border stays blue on hover); keyboard focus gets a 3px blue ring. Chips are real checkboxes; non-interactive labels are never chip-shaped.

### Cards / Containers
There are no cards. Content sits directly on the wall.
- **Photo frames:** 18px corners, Raised Night loading ground, Hung frame shadow, no border.

### Inputs / Fields
- **Style:** Plaster Field fill, 2px Plaster Edge border, 12px corners, 14px 16px padding, 56px minimum (110px textarea, vertical resize), warm brown placeholder.
- **Hover / Focus:** border goes Form Blue on hover; on focus the border stays blue and a 3px 22% blue halo appears; the caret is blue.
- **Error:** 700 / 15px Error Red text under the field, announced as an alert; the field is marked invalid. Hidden when empty.

### Navigation
- **Header (the ceiling):** wordmark "Handy" + amber "Max" at 900 / 22px on the left; the language toggle (an underlined Dusk Gray text button, "Español" / "English") pushed right; the tap-to-call number with an amber phone glyph in the top-right corner. All targets 44px+. Not sticky.
- **Footer:** a single wrapped line: the bolded name, the email address, the Facebook link, all in Dusk Gray brightening to amber on hover.

### Service Rows (signature)
The whole row is the link; one arrow-in-circle per row is the only cue.
- **Layout:** full-width rows, 62px minimum, 19px / 700 label left, 40px Raised Night circle with a 2.4px-stroke arrow right, 1px Wall Rule between rows; two CSS columns (56px gap) from 700px.
- **Hover / Focus:** only the arrow changes: the circle fills amber and the arrow strokes navy ink. The row never gets an outline, border, ring or background tint; the keyboard focus ring (3px amber, 3px offset) goes around the arrow circle.
- **Behavior:** on touch devices a row opens a pre-written text to Max naming that job; on fine-pointer desktops it ticks that job's chip in the estimate form and moves focus there.

### Light-Row Canvas (signature)
The world's motion system: one shared animation loop drawing recessed cans and their wall scallops on every canvas that carries them.
- **Scallop:** a precomputed 220x420 sprite of a real downlight wash: dark above a parabolic cutoff, brightest just under it, fading downward and toward the edges, plus a hot spot at the lens. Tinted rgb(255,196,122) at up to 92% alpha.
- **Cans:** flattened ellipses (13x4 phone, 16x5 desktop) in Can Trim with a lens that warms from cool gray to near-white as intensity rises; under the hero's ceiling band each can also glows on the ceiling.
- **Placement:** cans spaced evenly (about every 105px on phones, 190px on desktop, at least two); scallop width is 1.7x the spacing (170px minimum).
- **Instances:** the hero (64px ceiling band, dust, full-height beams); a work-section ceiling (340/440px tall, with dust); the estimate "reveal" (150/180px: paints Night Wall above, then cuts it away under each beam with a gradient so the lit plaster shows through, warmed with a 55% beam overlay); the closing section ceiling (340/440px, no dust).
- **Interaction:** a finger or mouse brings up the cans nearest it and pushes and carries dust; the pointer is read against each canvas every frame so it works while the page scrolls under a finger. Idle rows sweep on, one can after another, alternating direction. The wall switch sets every row to full and back. A sent estimate sweeps the estimate wall's lights on.
- **Performance and access:** paused off screen via IntersectionObserver; device pixel ratio capped at 1.5; fewer motes on phones; `prefers-reduced-motion` gets one still frame with the lights at 75% (100% with the switch on), redrawn only on resize. Canvases never take pointer events.
- **TUNE constants (the tuning surface; keep them named at the top of the IIFE):**
  - `BASE` 0.24: resting brightness of every light (0-1).
  - `BREATH` 0.05: slow breathing amplitude around BASE (plus a faster 0.025 ripple, each can on its own phase).
  - `DECAY` 0.55: per-second rate a light dims back to BASE.
  - `RISE` 14: how fast a light comes up under a finger.
  - `REACH` 0.75: finger influence radius, in light spacings.
  - `SWEEP_STEP` 0.13: seconds between cans in a sweep (each can holds full for 0.35s).
  - `IDLE` 6: seconds without a finger before a row sweeps by itself.
  - `MOTES_PHONE` 55 / `MOTES_DESKTOP` 140: dust particle counts.
  - `PUSH` 80: finger radius (px) that shoves dust.

### Wall Switch
A real two-screw rocker plate (Switch Plate, 8px corners, Wall fixture shadow) on the right edge of the hero, 48x76 on phones and 58x92 on desktop. Pressing it toggles every light row fully on; the rocker flips and `aria-pressed` reflects state.

### Before/After Slider
Two matched photos stacked in a hung frame; the after image clips from a CSS position variable. Plain 4px solid amber divider, 48px amber knob with a navy double-chevron, uppercase white tags at the bottom corners. Drag horizontally by touch (vertical drags still scroll), drag or click by mouse, arrow keys step 4% (10% with Shift), Home/End jump. The Facebook link sits directly under it as a 60px amber-outlined pill with a filled amber icon circle.

## Do's and Don'ts

### Do:
- **Do** keep amber as the single accent and use it for things that are light or that a hover has just lit.
- **Do** confine Form Blue to hover and focus on estimate-form controls.
- **Do** make service-row hover change only the arrow circle (neutral to amber), with the keyboard ring around the circle.
- **Do** put the phone number in the header's top-right corner as a tap-to-call link and nowhere else on the first screen; it may return in the closing section.
- **Do** keep the email address in the footer only, and the Facebook link both directly under the before/after and in the footer.
- **Do** make primary and secondary buttons the same height (56px+) and border; secondary is outlined, never filled.
- **Do** tune motion through the named TUNE constants and keep one shared loop, off-screen pausing, the DPR cap, and the reduced-motion still frame.
- **Do** cast shadows downward and navy-tinted, as if lit by the cans.

### Don't:
- **Don't** add a sticky bottom action bar or any full-width banner fixed to the screen.
- **Don't** put a call button in the hero, a third button under the title, or the phone number twice on one screen.
- **Don't** add email buttons, mailto prompts, or a send-by-email option anywhere outside the footer.
- **Don't** outline, border, ring or tint a service row on hover or focus.
- **Don't** use black or near-black grounds; the darkest tone is the ceiling band.
- **Don't** add hairline highlights, glints, sheens, or moving decorations on the before/after divider.
- **Don't** style non-interactive labels or service-area towns as pills or chips.
- **Don't** let scallops, dust or the switch run through text.
- **Don't** introduce icon cards, stock photography, or a blue-and-orange "pro" contractor bar.
