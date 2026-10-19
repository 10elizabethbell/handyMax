---
name: HandyMax
description: A job-site sign for a one-person handyman; a cutaway house the visitor renovates room by room.
colors:
  sign-yellow: "#ffc83a"
  sign-yellow-light: "#ffd25c"
  sign-text-2: "#4a3d12"
  navy-ink: "#15233b"
  navy-ink-2: "#22345a"
  night-line: "#2b3d5f"
  text-on-navy: "#f6f2ea"
  text-on-navy-2: "#c3cbdb"
  drywall: "#f6f2ea"
  drywall-bright: "#fffdf8"
  drywall-edge: "#d6cdbd"
  ink-soft: "#4a5266"
  painters-tape: "#2b7bbd"
  form-blue: "#2f6bff"
  error-red: "#b3261e"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(34px, 8.8vw, 92px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(34px, 9vw, 64px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "19px"
    fontWeight: 700
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.5
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "19px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.5
  tape:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 800
    letterSpacing: "0.05em"
rounded:
  wordmark: "3px"
  field: "12px"
  media: "18px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-phone: "20px"
  gutter-wide: "32px"
  container: "1160px"
  section-phone: "72px"
  section-wide: "96px"
  string-top-phone: "130px"
  string-top-wide: "160px"
components:
  button-primary:
    backgroundColor: "{colors.navy-ink}"
    textColor: "{colors.sign-yellow}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.navy-ink-2}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-send:
    backgroundColor: "{colors.navy-ink}"
    textColor: "{colors.drywall}"
    rounded: "{rounded.pill}"
    height: "56px"
  input-field:
    backgroundColor: "{colors.drywall-bright}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "56px"
  chip:
    backgroundColor: "{colors.drywall-bright}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.navy-ink}"
    textColor: "{colors.drywall}"
  service-row:
    textColor: "{colors.navy-ink}"
    typography: "{typography.title}"
    height: "62px"
  tape-label:
    backgroundColor: "{colors.painters-tape}"
    textColor: "#ffffff"
    typography: "{typography.tape}"
    padding: "3px 10px"
---

# Design System: HandyMax

## Overview

**Creative North Star: "The Job-Site Sign"**

HandyMax reads like a yellow sign staked in a front lawn: one loud field of sign yellow, navy ink set heavy and uppercase, and everything else made of the materials of the job itself. Painter's tape labels the work, a paint roller does the renovating, C9 Christmas-light strings hang on real rope physics across the tops of sections, and the estimate form sits on clean finished drywall. The hero is a dollhouse cutaway of a house (slate roof, kitchen, window wall, basement under the dirt line) that goes from tired to finished room by room, under a finger or on its own.

The page alternates three grounds in a fixed order: the sign (hero, services, close), the night (navy: work, Max, how it works), and the drywall (estimate). Each change of ground is announced by a light string hung across the section top. Density is low and phone-first: one column, big tap targets, a single display voice.

It refuses the contractor template (job-photo hero, blue-and-orange bar, icon cards) and the earlier can-light night-wall world this replaced.

**Key Characteristics:**
- One yellow field, one navy ink; navy carries every type and button on yellow.
- Heavy uppercase system-sans display (900, -0.02em, 0.95 leading).
- Job materials as UI: tape labels, roller wipe, C9 light strings, drywall form.
- Three grounds in order: sign, night, drywall, back to sign; never black.
- Pills for actions, 18px corners for photos, 12px for fields.

## Colors

A two-color sign (yellow and navy) with a warm drywall neutral and one blue borrowed from painter's tape.

### Primary
- **Job-Site Sign Yellow** (#ffc83a): the ground of the hero, services and close, the `html` background and `theme-color`. On navy it becomes the accent: step numerals, the before/after bar and knob, the Facebook ring, focus rings, footer link hover. The hero lifts it with a radial wash toward Sign Yellow Light (#ffd25c) behind the house.
- **Sign Text Brown** (#4a3d12): secondary text on yellow (promise, ledes, the "where" line), tinted from the yellow rather than a grey.

### Secondary
- **Navy Ink** (#15233b): all type and lines on yellow, the fill of primary buttons, the night-section ground, the footer, the wordmark's "Max" block, the roller frame in the hero. Navy Ink 2 (#22345a) is its hover and the photo placeholder fill.

### Tertiary
- **Painter's Tape Blue** (#2b7bbd): only on tape strips: the hero's room labels and the Before/After tags. White 800-weight uppercase text on it.
- **Form Blue** (#2f6bff): hover and focus on estimate-form controls only (inputs, textarea, chips, send button, caret).

### Neutral
- **Finished Drywall** (#f6f2ea): the estimate ground; also primary text on navy.
- **Drywall Bright** (#fffdf8): input and chip fill; the roller sleeve.
- **Drywall Edge** (#d6cdbd): 2px resting border for inputs and chips.
- **Soft Ink** (#4a5266): secondary text on drywall (lede, notes, optional tags).
- **Night Secondary** (#c3cbdb): secondary text on navy and the footer's text.
- **Hairline** (rgba(21,35,59,.22)): service-row dividers on yellow.
- **Error Red** (#b3261e): inline form errors, 700 weight.

### Named Rules
**The Two-Inks Rule.** On yellow, everything is navy; on navy, accents are yellow. No third color competes on either ground; tape blue appears only as tape.

**The Never-Black Rule.** The darkest ground is Navy Ink (#15233b). No section, footer or overlay goes black.

**The Form-Blue Rule.** Form Blue (#2f6bff) exists only for hover and focus on estimate-form controls. It never appears at rest and never outside the form.

## Typography

**Display Font:** system sans stack (-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif)
**Body Font:** the same stack

**Character:** One family doing a sign painter's job: black weight, uppercase, tight tracking for anything that announces; plain 17px reading text for anything Max says.

### Hierarchy
- **Display** (900, clamp(34px, 8.8vw, 92px), 0.95, uppercase, -0.02em): the hero headline only, balanced line by line. The close's wordmark uses the same voice larger (clamp(44px, 13.5vw, 96px)).
- **Headline** (900, clamp(34px, 9vw, 64px), 0.95, uppercase, -0.02em): every section h2.
- **Title** (700 to 800, 19 to 22px): service rows (19px/700), step titles (22px/800 uppercase, -0.01em), the Facebook link (19px/800).
- **Body** (400, 17px, 1.5): default text; Max's paragraphs run 19px at max 30em.
- **Lede** (400 to 500, 19px or clamp(17px, 4.6vw, 20px) for the hero promise): one-line section introductions in the secondary ink of the ground.
- **Label** (800, 17px): form labels, with a 600/15px "(optional)" in Soft Ink.
- **Tape** (800, 14px, 0.05em, uppercase): text on painter's tape; the canvas labels scale 10 to 15px with the house.
- **Numerals** (900, 44px, Sign Yellow): step counters on navy. Phone numbers use tabular figures.

### Named Rules
**The System-Stack Rule.** The system font stack only. No webfonts, no second family; weight and case do the work.

**The Shout-Then-Talk Rule.** Uppercase 900 is for headlines, step titles and tape. Everything Max says to the visitor is sentence case at reading weight.

## Layout

Single column on phones with a 20px gutter, widening to 32px at 700px; content caps at 1160px. Sections pad 72px vertically on phones and 96px from 700px. A section that carries a light string at its top gets 130px top padding (160px from 700px) so the string hangs in clear space; the string canvas is 96px tall on phones and 120px wide.

The hero fills the first screen (clamp(640px, 100svh, 880px)). On phones the copy is bottom-anchored and the house is sized to fill the space between header and headline. From 1024px the copy sits left (max 500px or 40vw), vertically centered, with the house on the right edge of the container.

At 700px the hero buttons go side by side and the services list breaks into two columns (56px gap). At 1024px the before/after takes the wider column with the heading and Facebook link beside it, Max's portrait sits beside his words, the three steps run in a row, and the estimate splits into intro and form (1fr / 1.3fr). Under 380px the header tightens so wordmark, language and phone fit on one line.

### Named Rules
**The Phone-Top-Right Rule.** On the first screen the phone number appears only in the header, top-right. It may return in the close. There is no call button in the hero and no sticky bottom bar.

## Elevation & Depth

Flat grounds; depth belongs only to physical things. Photos cast long, soft, navy-black shadows as if hung on the wall; tape strips carry a tight drop as if stuck on; the before/after knob floats. Buttons, rows, chips and fields never cast shadows. On navy, the light strings glow with additive radial halos; on yellow and drywall the bulbs read by color alone, and the estimate's string stays unlit until an estimate is sent.

### Shadow Vocabulary
- **Hung photo** (`box-shadow: 0 30px 60px -28px rgba(5,10,20,.85)`): the before/after frame and Max's portrait (portrait at -24px, .9).
- **Tape** (`box-shadow: 0 2px 4px rgba(5,10,20,.3)`): Before/After tags; the canvas tape uses an equivalent 3px navy blur.
- **Knob** (`box-shadow: 0 6px 16px rgba(5,10,20,.45)`): the before/after drag handle.
- **Form focus halo** (`box-shadow: 0 0 0 3px rgba(47,107,255,.22)`): focused fields; .3 on the send button.

### Named Rules
**The Only-Objects-Cast Rule.** Shadows belong to objects in the world (photos, tape, the knob). Interface controls stay flat.

## Shapes

Pills (999px) for every action: buttons, chips, the Facebook link. Circles for icon carriers: the service-row arrow (40px), the Facebook badge (40px), the before/after knob (48px). Photos round at 18px. Fields round at 12px. The wordmark's "Max" block is a 3px-rounded navy slug. Tape strips are the one deliberately crooked shape: square-ended, rotated a few degrees (±2° on tags, -3° to 34° in the hero), torn at the ends in the canvas.

## Components

### Buttons
Heavy, round, sign-painted.
- **Shape:** full pill (999px), min height 56px, 26px side padding, 2px navy border, 800 weight 17px.
- **Primary:** Navy Ink fill, Sign Yellow text. Hover to Navy Ink 2.
- **Outline:** transparent with navy border and text; hover tints with 8% navy.
- **Send (estimate):** Navy fill, Drywall text; hover and focus swap the border to Form Blue with a blue halo.
- **Press:** 1px downward nudge on all buttons.
- **Pairing:** the two hero buttons are always the same height, stacked full-width on phones and side by side from 700px.

### Chips
- **Style:** Drywall Bright pill, 2px Drywall Edge border, 46px tall, 700 weight 16px.
- **State:** hover turns the border Form Blue; checked fills Navy Ink with Drywall text; keyboard focus gets a 3px Form Blue ring.

### Inputs / Fields
- **Style:** Drywall Bright fill, 2px Drywall Edge border, 12px radius, 14px 16px padding, 56px min height (textarea 110px); caret in Form Blue.
- **Focus:** border to Form Blue plus a 3px 22% Form Blue halo; hover also turns the border Form Blue.
- **Error:** a 700-weight Error Red line under the field; the control gets `aria-invalid`.

### Navigation
The header is the hero's top 64px: wordmark left (22px, 900, "Max" in a navy slug), then the language toggle (an underlined text button, 15px/700) and the phone link (16px/800, tabular, inline phone glyph) pushed right. No menu. The footer is navy with the name in 900, then the email and Facebook links, Night Secondary text turning Sign Yellow on hover.

### Service Row
A full-width list on the yellow, 62px tall, 19px/700 job name left and a 40px circle with an arrow right, divided by navy hairlines. Hover and keyboard focus change only the arrow circle: it fills Navy Ink and the arrow turns Sign Yellow. The row itself never highlights. On touch a row opens a pre-written text; on desktop it selects that job in the estimate form.

### Painter's-Tape Label
Tape Blue strip, white 800 uppercase tracked text, tilted, small drop shadow. Used for the hero room labels and the Before/After tags. A label marks a real thing in the picture; it is never a section kicker.

### Light String
A C9 Christmas-light string drawn on canvas as a verlet rope hung from evenly spaced clips: dark green wire (#1f3a28; navy on the close), bulbs cycling red, green, blue, amber and pink, a gentle twinkle, and a finger or cursor can shove it. Strings hang across the top of each change of ground (work, estimate, close) and along both slopes of the hero roof. Under reduced motion everything renders still and fully finished.

### Signature: The Cutaway House
The hero canvas: a dollhouse cross-section with roof, kitchen, window wall and basement below a dirt line. Each room starts tired; a tap (or Max, after 5s idle, every 1.1s) sends a paint roller across it in 0.75s, wiping the finished room in. The roof's lights switch on from the ridge outward last. When the finished house scrolls out of view it resets, so it is never seen going backwards.

### Before / After
An 18px-rounded photo frame with a hung-photo shadow, a 4px Sign Yellow divider and a 48px yellow knob; drag or arrow keys move the split. Tape tags label each side. The Facebook link (a yellow-ringed pill with a yellow Facebook badge) sits directly under it.

## Do's and Don'ts

### Do:
- **Do** keep every ground yellow (#ffc83a), navy (#15233b) or drywall (#f6f2ea), in the order sign, night, drywall, sign.
- **Do** set headlines in the system stack at 900, uppercase, -0.02em, 0.95 leading.
- **Do** announce a change of ground with a light string hung across the section top, and give that section 130px (160px wide) of top padding.
- **Do** use pills (999px) at 56px height for actions, and keep paired buttons the same height.
- **Do** label things in the picture with painter's tape (#2b7bbd), tilted, white uppercase.
- **Do** put the Facebook link under the before/after and again in the footer; put the email in the footer only.
- **Do** render every animation as a finished still under `prefers-reduced-motion`.

### Don't:
- **Don't** let the ground go black, anywhere.
- **Don't** load a webfont or add a second family.
- **Don't** show the phone number on the first screen anywhere but the header's top-right, add a call button to the hero, or add a sticky bottom bar.
- **Don't** highlight a whole service row on hover; only the arrow circle changes.
- **Don't** use Form Blue (#2f6bff) at rest or outside the estimate form's hover and focus states.
- **Don't** use tape strips as section kickers or eyebrows above headings.
- **Don't** put shadows on buttons, chips, rows or fields.
- **Don't** fall back to the contractor template: job-photo hero, blue-and-orange bar, icon cards.
