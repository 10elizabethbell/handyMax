# HandyMax — handoff at ~60%

**Live:** https://10elizabethbell.github.io/handyMax/ · **Repo:** https://github.com/10elizabethbell/handyMax · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, Facebook group "NJ Seeking Contractors")

## What's built
- **World (redesigned 2026-10-19, Ellie's pick from three working demos):** a job-site-yellow sign with Max's house cut open like a dollhouse: roof and attic, kitchen, window wall, and the basement under the dirt line. Room names sit on painter's-tape labels (in English or Spanish, following the page). The old can-light world is gone.
- **Signature element:** every room starts tired (patched roof, brown kitchen, cracked window, raw basement). A finger or mouse over a room renovates it with a paint-roller wipe, and the label gets a tick. A string of Christmas lights on the roof swings when touched and switches on. Left alone, Max renovates the house room by room and it stays finished; it only goes back to tired while scrolled off-screen, so nobody watches the work undone. Swinging light strings run across the tops of the work, estimate and closing sections. The estimate's string stays dark until an estimate is sent, then lights up left to right. Tunables are in `TUNE` in the house script (`WIPE`, `STEP`, `IDLE`, string physics, `LIGHT_UP`).
- **Grounds:** yellow (hero, services, close), navy (before/after, Max, how it works, footer), drywall white (estimate form).
- **Sections:** header (wordmark, Español toggle, tap-to-call number top-right) → hero "Roof to basement. Inside and out." + promise + Free estimate / See my work → What I do (17 services: roofs, basements, kitchens, windows and Christmas lights first, then the 12 from his Facebook posts; each row opens a pre-written text) → Before & after slider + "Click to see more of my work." Facebook link → Hi, I'm Max (photo, his own bio, then the one-person paragraph) → How it works (3 steps) → Free estimate form (chips + details + name + town, sends a pre-written SMS; call link as backup) → closing wordmark, tagline, number → footer with name, email, Facebook.
- **Bilingual:** full English/Spanish toggle (saved per visitor; Spanish browsers start in Spanish). SMS bodies follow the language.
- **Contact:** `tel:+18622393260` (header top-right, form backup line, big number in the close); `sms:+18622393260?&body=…` (service rows on phones, and the form). On computers, where `sms:` does nothing, a service row ticks that job in the estimate form instead. Email `handymaxx27@gmail.com` in the footer only.
- **Demos:** the three candidates stay in `demos/` (`cutaway.html`, `blueprint.html`, `lights.html`, English only, not linked from the site) so you can compare or swap.

## Assumptions I made
- **Email** `handymaxx27@gmail.com` is printed on his Facebook profile picture (fetched 2026-10-17). The brief said none found. It's in the footer only.
- **Texting works:** the brief says texts are "unknown". It's his personal cell, so the form and service rows hand off by SMS, and every SMS path has a call option next to it.
- **One-person business** ("you get me… I'm the one doing the work"), inferred from "Call Max" and the personal cell.
- **Promise copy** ("careful with your walls, straight with you on price, nothing left behind but the finished job"), the step "You know the price before I start" and "I clean up after myself" are written from his "Reliable • Professional • Affordable" and "FREE ESTIMATES". They're not his words; confirm them with him.
- **"Wall Panel Installation"** (English post) is listed as "Wall panels" (decorative panels, which fit with TV mounting). The Spanish post's "Paneles Eléctricos y Subpaneles" is listed separately as "Electrical panels & subpanels". Check which he meant.
- **Area:** only "New Jersey" appears on the page. Northern NJ is inferred from the 862 area code and not shown.
- **Colors:** no logo or brand colors exist. Yellow and navy come from the world: a job-site sign. The icon is a navy roof and "H" on yellow with four bulbs.
- **Roofs, basements, kitchens, windows, Christmas lights** come from you, not his posts. Confirm he wants them leading the list (and that he does roofing).
- **Hero copy** ("Roof to basement. Inside and out." / "Del techo al sótano. Por dentro y por fuera.") and the promise are mine.
- **Before photo** looks like a real-estate listing photo, from a different angle than the after. It's his own post, so I used it.
- **Spanish copy** is mine, revised once in review. Have a native speaker read it. The tagline "Reliable • Professional • Affordable" stays in English in both languages because it's his own wording; the Spanish post has no tagline ("Confiable • Profesional • Económico" is the obvious translation if he wants one).
- **"How it works"** is kept, but one reviewer suggested cutting it as mechanical copy. Your call.
- **World choice:** the first build used recessed can lights (you found it didn't say what he does). The second roll (seed a5ee8a45) assigned blueprint-to-built; you picked the cutaway house (Impeccable's own pick) from working demos.

## Placeholders and gaps
- No logo. The wordmark is "Handy" plus "Max" on a navy block, in the site's lettering; the favicon and home-screen icon are a navy roof and "H" on yellow with four bulbs (`icon.svg`).
- Only one work photo (one before/after pair). The page timeline was blocked (403).
- No service-area towns, hours, reviews, prices, or years in business. None appear on the page.
- No licensing or insurance claim. A commenter asked "Nj Electrical License??" and none is published.

## Questions for the owner
- Which towns do you cover?
- Do you take texts at 862-239-3260? (The site sends texts.)
- More before/after photos? TV mounts with hidden wires and LED installs would suit this page best.
- Did "Wall Panel Installation" mean decorative wall panels or electrical panels?
- Hours? Licensed/insured? (Only if yes and he wants it shown.)
- Is the email on your profile picture the one to show?

## Ideas not built (yours to pick)
- **Runner-ups, built as demos:** blueprint-to-built (`demos/blueprint.html`) and Christmas-light strings (`demos/lights.html`).
- An outdoor face for the house: tapping the lawn or siding to show exterior work (gutters, outdoor lighting, cameras).
- A per-service tie-in: tapping a service row scrolls up and renovates the matching room first.
- Swap in his own photos per room (kitchen, basement) as he sends them; the slider component is reusable.
- Atkinson Hyperlegible or a self-hosted display face, if you ever lift the system-font rule.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser). Headless test only: a TouchEvent over the windows room renovates it.
- Real SMS handoff on iOS/Android (body encoding verified by decoding; `?&body=` form).
- Frame rate on old phones. The house is two pre-rendered layers composited per frame; canvas DPR is capped at 1.5, and off-screen canvases pause.
- Headless Chrome drops the canvas from direct screenshots. Captures were taken inside iframes.
