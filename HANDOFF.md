# HandyMax — handoff at ~60%

**Live:** https://10elizabethbell.github.io/handyMax/ · **Repo:** https://github.com/10elizabethbell/handyMax · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, Facebook group "NJ Seeking Contractors") · **Revamped:** 2026-10-19 in the calm band style

## Revamp, 2026-10-19: what changed
The whole page was rebuilt from the DPG reference (`dpgHomeImprovement/index.html`) under the new house default (`calm-photo-style.md`). Max hasn't been contacted, so nothing of the old look was kept.
- **Gone:** the job-site-yellow cutaway house hero (rooms renovated by a paint roller), the swinging Christmas-light strings, and the yellow, navy and drywall grounds. The house still exists as an opt-in demo in `demos/cutaway.html`, and the full build is in git history at `7c9efb4`.
- **Look:** paper `#f4f6fb` with beanie-navy `#1d3f73` and deep-navy `#0f2340` bands (the deep ones carry the faint diagonal lines). Job-site yellow `#ffc83a` is the one accent and is only ever a fill (`#8a5a00` when it has to be text on light). Headings are in Cal Sans, the body in the system font at 16/1.7. Cards are 24px, buttons are pills, and fields are tinted with no border.
- **Hero:** now a photo. It's Max's own finished dining room (the "after" half of his post: recessed lights and a new fixture) under a navy overlay. On phones it fills the band; on desktop it sits at the right 60% at close to its own size, so it isn't blown up and blurry, and the copy sits on solid navy.
  - White text measures 5.0:1 at 390px, 5.85:1 at 1024px and 6.0:1 at 1440px (pixel-sampled worst case).
  - The yellow "New Jersey." measures about 3.3:1, which passes as large text.
- **Motion:** the hero H1 bounces in letter by letter, in whichever language is showing. It waits up to 600ms for Cal Sans so the letters don't land in the fallback font, then puts the plain heading back. Below the first screen there's one 12px fade-up. Both are off under reduced motion and with JS off.
- **Floating text circle:** it opens a text to Max, in the current language. It's hidden on the hero and while the estimate form is on screen, and doesn't exist with JS off.
- **Rows no longer text Max directly.** On every device, tapping a service row ticks that job in the estimate form and flashes it with a yellow ring. Before, rows texted Max on phones. This follows the calm kit, and it means the floating circle and the form are the only ways to text.
- **Hero copy:** eyebrow "Handyman & electrical", H1 "Roof to basement in **New Jersey.**", the promise "I take care of your home like it's my own.", and two buttons: **Get a free estimate** and **Text Max** (outlined). The earlier "Roof to basement. Inside and out." and "See my work" are gone.
- **Section order:** header (wordmark, Español, number top-right) → hero → Hi, I'm Max (paper) → What I do (17 rows, deep navy) → Before & after slider + "Click to see more of my work." Facebook card (paper) → How it works (navy) → Free estimate form (paper) → close: HandyMax, his tagline, number (navy) → footer: name, number, email, Facebook (deep navy).
- **New or replaced files:** `img/hero.webp` (+ provenance `.json`), `og.jpg` (a shot of the new hero), and `icon.svg`/`apple-touch-icon.png` (roof and "H" on yellow, with the Christmas bulbs dropped). `DESIGN.md` was rewritten for the calm world.
- **Impeccable:** every mode except live (and onboard, n/a) was run, plus the finish reviewer. Fixes applied:
  - the hero eyebrow now says what he does
  - selected chips outline on hover
  - the floating circle's focus ring shows on navy
  - stale `aria-invalid` cleared
  - the Before & after column is centred beside the slider on desktop
  - the slider is labelled "Dining room…"
  - footer number is a call link
  - a no-JS call line in the form
  - "Mándale esto a Max"
  - provenance for the hero photo

## What's built
- Bilingual EN/ES toggle in the header. It's remembered per visitor, and Spanish browsers start in Spanish. Text-message bodies, labels and the page title follow the language. Without JS the page shows English.
- **Contact:**
  - `tel:+18622393260`: header top-right, form fallback line, big number in the close, footer.
  - `sms:+18622393260?&body=…`: hero "Text Max", floating circle, estimate form. The form's text carries the jobs picked, details, name and town.
  - Email `handymaxx27@gmail.com`: footer only.
- Facebook: the card under the before/after, and in the footer.

## Assumptions I made
- **Email** `handymaxx27@gmail.com` is printed on his Facebook profile picture (fetched 2026-10-17). The brief said none was found.
- **Texting works.** The brief says texts are "unknown". It's his personal cell, so the form, the hero button and the floating circle all hand off by SMS. The tap-to-call number is in the header and the close.
- **One-person business**, inferred from "Call Max" and the personal cell. Two lines on the page are my wording, not his, and need his OK:
  - "you get me… I'm the one in your home doing the work"
  - "I clean up after myself"
- **Promise copy** is written from his "Reliable • Professional • Affordable" and "FREE ESTIMATES"; these aren't his words:
  - "I take care of your home like it's my own."
  - "You know the price before I start."
  - "Not sure I cover your town? Call and ask."
- **"Hi, I'm Max" paragraph two** is his own Facebook bio, word for word. Both reviewers flagged it as generic, template-sounding copy. I kept it because it's his and you added it. Cutting it, or replacing it with a line like "I speak English and Spanish, so tell me about the job whichever way is easier", is your call.
- **Palette:** no logo or brand colours exist. The navy is from his beanie in the profile photo, and the yellow is job-site yellow (carried over from the first build).
- **Area:** only "New Jersey" appears. Northern NJ is inferred from the 862 area code and isn't shown.
- **"Wall Panel Installation"** (English post) is listed as "Wall panels". "Paneles Eléctricos y Subpaneles" (Spanish post) is listed separately as "Electrical panels & subpanels".
- **Roofs, basements, kitchens, windows and Christmas lights** come from you, not his posts. They lead the list.
- **Hero photo:** the "after" half of his own post, cropped to remove a person reflected in the glass door and the baked-in label. The same room appears again in the before/after slider. The before shot looks like a real-estate listing photo taken from a different angle.
- **Spanish copy** is mine. Have a native speaker read it.

## Placeholders and gaps
- No logo. The wordmark is "Handy" + "Max" (Max in the yellow ink shade) in Cal Sans, and the favicon is a roof and "H" on yellow.
- Only one work photo (one before/after pair). The page timeline was blocked (403).
- No service-area towns, hours, reviews, prices or years in business. None appear on the page.
- No licensing or insurance claim. A commenter asked "Nj Electrical License??" and none is published.

## Questions for the owner
- Which towns do you cover?
- Do you take texts at 862-239-3260? (The site sends texts.)
- More before/after photos? TV mounts with hidden wires and LED installs would suit this page best, and a better hero photo would help too.
- Did "Wall Panel Installation" mean decorative wall panels or electrical panels?
- Hours? Licensed or insured? (Only if yes and he wants it shown.)
- Is the email on your profile picture the one to show?
- Are the inferred promises right ("I'm the one doing the work", "I clean up after myself", "you know the price before I start")?

## Ideas not built (yours to pick)
- **Signature motion (opt-in), worlds from his trade:**
  1. **Cutaway house:** your earlier pick, a working demo in `demos/cutaway.html`. Rooms renovate under a finger. This is the best fit.
  2. Blueprint drawn into a finished room (`demos/blueprint.html`).
  3. Christmas-light strings that swing and switch on (`demos/lights.html`).
  4. A light switch that brightens the hero room.
  5. Wiring pulled through a wall and hidden.
- 17 rows plus 17 chips is a lot of choice (Impeccable's distill check). Grouped chips (Inside / Electrical & lighting / Outside) are an option.
- The Facebook card could say "See more of my work on Facebook." The current line is the finishing-rules wording.
- A sticky header (the kit's header shadows on scroll). It's left static so the number appears once per screen.
- Desktop: the empty area under the estimate heading could hold the three "How it works" steps or a second photo once he sends one.
- **Impeccable findings I kept against its advice (house style):**
  - eyebrow pills (the craft floor bans them)
  - the H1 letter bounce-in (bounce easing)
  - the floating text circle
  - Cal Sans
  - the faint diagonal band texture (suppressed in the detector with that reason)
  - the `.rise` fade-up
  - tinted borderless fields: the field fill is 1.19:1 against the white card, below WCAG 1.4.11's 3:1 for boundaries. `box-shadow: inset 0 0 0 1px #8794a6` would fix it if you want.
  - yellow step-number discs in How it works. The reviewer said they look pressable like the floating circle; they're as on DPG.
  - the hero photo is dim on phones. The overlay can't get lighter without dropping white text below 5:1.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser). Tested headless in Chromium and WebKit at 360, 390, 430, 1024 and 1440, with no overflow and all tap targets 44px or more.
- Real SMS handoff on iOS/Android. The form body was decoded and checked:

  ```
  Hi Max, I'd like a free estimate. / Job: … / Details: … / Name: … / Town: …
  ```
- The bounce-in on a slow cellular first load (the font wait is capped at 600ms).
