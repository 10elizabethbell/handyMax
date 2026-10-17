# HandyMax — handoff at ~60%

**Live:** https://10elizabethbell.github.io/handyMax/ · **Repo:** https://github.com/10elizabethbell/handyMax · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, Facebook group "NJ Seeking Contractors")

## What's built
- **World:** a living-room wall at night (navy `#16233b`). The header is the ceiling; recessed can lights in it throw real downlight scallops of warm amber light on the wall, with dust drifting in the beams. It ties straight to Max's own before/after: a dim room that got recessed lights.
- **Signature element:** a finger or mouse turns up the lights under it, and they dim back slowly. When nobody touches the page they sweep on by themselves. Dust gets pushed around by the finger and settles back. A real wall switch on the right turns every light on. Smaller light rows repeat as the ceiling of the work, Max and closing sections. The estimate section is the lit plaster wall showing through under the scallops. Tunables are in `TUNE` in the lights script (`BASE`, `DECAY`, `RISE`, `REACH`, `IDLE`, mote counts).
- **Sections:** header (wordmark, Español toggle, tap-to-call number top-right) → hero "Lights on. Wires gone." + promise + Free estimate / See my work → What I do (12 services from both Facebook posts; each row opens a pre-written text naming the service) → Before & after slider (his dining-room post) + "Click to see more of my work." Facebook link → Hi, I'm Max (his profile photo) → How it works (3 steps) → Free estimate form (chips + details + name + town, sends a pre-written SMS; call link as backup) → closing wordmark, tagline, number → footer with phone, email, Facebook.
- **Bilingual:** full English/Spanish toggle (saved per visitor; Spanish browsers start in Spanish). SMS bodies follow the language.
- **Contact:** `tel:+18622393260` (header top-right, form backup line, big number in the close); `sms:+18622393260?&body=…` (service rows on phones, and the form). On computers, where `sms:` does nothing, a service row ticks that job in the estimate form instead. Email `handymaxx27@gmail.com` in the footer only.
- **Footer phone:** removed. The close's big number sits on the same screen, so per the once-per-screen rule it serves as the footer phone. Footer = name, email, Facebook.
- **Rewards:** sending a valid estimate sweeps the estimate wall's lights on, and the wall switch cuts the lights instantly when turned off.

## Assumptions I made
- **Email** `handymaxx27@gmail.com` is printed on his Facebook profile picture (fetched 2026-10-17). The brief said none found. It's in the footer only.
- **Texting works:** the brief says texts are "unknown". It's his personal cell, so the form and service rows hand off by SMS, and every SMS path has a call option next to it.
- **One-person business** ("you get me… I'm the one doing the work"), inferred from "Call Max" and the personal cell.
- **Promise copy** ("careful with your walls, straight with you on price, nothing left behind but the finished job"), the step "You know the price before I start" and "I clean up after myself" are written from his "Reliable • Professional • Affordable" and "FREE ESTIMATES". They're not his words; confirm them with him.
- **"Wall Panel Installation"** (English post) is listed as "Wall panels" (decorative panels, which fit with TV mounting). The Spanish post's "Paneles Eléctricos y Subpaneles" is listed separately as "Electrical panels & subpanels". Check which he meant.
- **Area:** only "New Jersey" appears on the page. Northern NJ is inferred from the 862 area code and not shown.
- **Colors:** no logo or brand colors exist. Navy and amber come from the world: night wall and warm light. His headlamp red is unused.
- **Before photo** looks like a real-estate listing photo, from a different angle than the after. It's his own post, so I used it.
- **Spanish copy** is mine, revised once in review. Have a native speaker read it. The tagline "Reliable • Professional • Affordable" stays in English in both languages because it's his own wording; the Spanish post has no tagline ("Confiable • Profesional • Económico" is the obvious translation if he wants one).
- **"How it works"** is kept, but one reviewer suggested cutting it as mechanical copy. Your call.
- **World choice:** Impeccable's concept roll (seed 979b58ed) assigned a breaker-panel world. I overrode it with the pitch-site rule (best brand + fluid touchable motion). A breaker snaps rather than flows, and it would put panel work, and so the license question, front and centre.

## Placeholders and gaps
- No logo. The wordmark is "Handy**Max**" in the site's lettering; the favicon and home-screen icon are an amber "H" under a can light (`icon.svg`).
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
- **Runner-up world:** Max's headlamp in an open stud wall (his profile photo's backdrop). The finger is the headlamp beam, revealing Romex runs that tidy themselves into the wall ("hidden wire management").
- A mounted TV on the hero wall with no wires showing, lit by the cans. It would demonstrate his two lead services in one picture.
- A per-service light: tapping a service row turns on one can light over it.
- Atkinson Hyperlegible or a self-hosted display face, if Ellie ever lifts the system-font rule.
- More slider pairs as he sends photos. The slider component is reusable.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser). Headless tests only: a TouchEvent sweep brightens the nearest light, and vertical drags still read the finger.
- Real SMS handoff on iOS/Android (body encoding verified by decoding; `?&body=` form).
- Frame rate on old phones. Phones get 55 dust motes vs 140 on desktop, and the canvas DPR is capped at 1.5.
- Headless Chrome drops the canvas from direct screenshots. Captures were taken inside iframes.
