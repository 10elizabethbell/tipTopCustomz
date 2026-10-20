# TIP TOP Customz — handoff at ~60%

**Live:** https://10elizabethbell.github.io/tipTopCustomz/ · **Repo:** https://github.com/10elizabethbell/tipTopCustomz · **Built:** 2026-10-20 from Muse brief (run 2026-10-20, Facebook group "Essex County Contractor Referrals" post)

## What's built
- One page in the calm band style: paper header (TIP TOP wordmark, tap-to-call number top right) → photo hero → Before and after (paper) → What we clean (navy service rows) → Your place, treated like our own + 3 steps (paper) → Reserve your spot form (light) → close with the logo and big number (navy) → footer (deep navy, texture).
- Palette from the logo: night navy `#0e1f3d`, mid navy `#17366b`, gold `#e8b84a` from the "Customz" script (fills only; `#85601a` when gold must be text on light), the logo's electric blue `#2563d9` for form hover/focus outlines.
- Hero: their own "after" frame of the cleared roof (from the post video) under a deep-navy overlay. White text measures 7.3:1 or better, gold H1 words 4.0:1 (large text, passes 3:1) by pixel sampling at 390 and 1440.
- Proof: four before/after pairs pulled from the 11-second post video (roof debris, gutter, roof edge gutter, gutter line over a window), side by side, labelled Before/After only. Then "Click to see more of our work." → their Facebook page.
- Contact: everything goes to (828) 246-2273. Hero "Reserve your spot" jumps to the form; "Text us" opens a pre-written text. Service rows pre-select the matching chip. The form (job chips, name, where, optional notes) composes a text; if Messages doesn't open, it shows the number. Floating gold text circle appears after the hero and hides over the form.
- Motion: hero H1 letter bounce-in, `.rise` fade-up below the first screen. Both off under reduced motion and without JS (verified).
- Favicon/touch icon: a "TT" in gold on navy, drawn from the site lettering (the logo is a busy illustrated badge that can't be read at 16px). `og.jpg` 1200×630 with the headline and logo.

## Assumptions I made
- **The business does more than pressure washing.** The logo says "DETAILING & MORE! · ENHANCE YOUR LUXURY" with a car, a boat ("CAMZZ") and an RV; the brief's post is pressure washing. I listed "Cars, boats & RVs" as a service from the logo. Confirm or cut.
- **"Gutters & roofs"** is a service row because their own video is entirely gutter/roof debris clean-outs, though the post's text doesn't list it. Confirm.
- **"We", not "I":** "WE COME TO YOU" in their post. Owner name unknown.
- **No place in the H1** (the calm style wants one): the brief says the area is mismatched (828 western NC number, ad in an Essex County NJ group) and not to publish a location. The H1 is their own line, "Make it look brand new again." Add the town when known: e.g. "Make it look brand new again in <town>."
- "Homes and businesses" in the hero promise comes from "Residential & Commercial".
- The care paragraph ("take our time on it, and don't call it done until it looks tip top") is my wording in their voice, not a quote. Owner should approve.
- The video frames are the "before" and "after" of the same jobs in the order the video shows them; the framing differs between each pair, so they're side-by-side pairs, not sliders.

## Placeholders and gaps
- Service area: unknown. Close says "Not sure we cover your area? Text and ask."
- Real business name: page reads "TIP TOP Customz" (as on Facebook). Confirm before delivery.
- No email (so none in the footer), hours, owner name, prices, reviews, years in business.
- Photos are video frames (1080×1918, compressed); they hold up at phone size but aren't as sharp as real photos would be. The trailer-deck wash from the end of the video isn't used (no matching before frame).
- The Facebook page timeline wasn't readable; there may be more photos there.

## Questions for the owner
- Which towns do you cover? (Puts the place in the headline.)
- Is detailing (cars, boats, RVs) still part of the business? Want it on the page?
- Your first name, so the page can speak as you?
- Any reviews from customers we can quote word for word?
- Real photos (not video frames) of a driveway, siding or deck before and after?
- Do you give free quotes? (Then the button can say so.)
- Email for the footer?

## Ideas not built (yours to pick)
- **Signature motion, opt-in:** runner-up worlds from the trade: (1) a pressure-wash wand you drag across a grimy driveway in the hero to reveal clean concrete (best fit, T&J/Above All style), (2) water sheeting down the siding, (3) leaves blowing off the gutter line, (4) foam/suds for the detailing side, (5) a gold wet-sheen sweep across the logo's chrome.
- Before/after sliders: needs pairs shot from the same spot; ask for some.
- A detailing section of its own if the owner wants it (car, boat, RV), with photos.
- **Impeccable findings left standing (they'd remove your calm-style choices):** the craft floor bans eyebrow pills, and the detector flags the diagonal band texture as "repeating-gradient stripes". Both stay. I also suppressed two other detector flags for `index.html`, in `.impeccable/config.json`: "cramped padding" (the photo pairs are meant to run to the card edge) and "flat type hierarchy" (it only counts the 11–20px sizes and misses the 30–84px Cal Sans headings, which use clamp()).
- From the finish review, not built: let the logo's neon blue/purple glow into the page somewhere (only the form focus colour uses it now); before/after drag sliders once pairs are shot from the same spot.
- Small delights from the sweep: a water splash when a job chip is ticked; a soft "rinse" wipe revealing each after photo as it scrolls in (motion, so opt-in).

## Review passes done
- All Impeccable modes except live (critique, audit, polish, harden, clarify, adapt, optimize, typeset, layout, colorize, animate, delight, distill, quieter, bolder, overdrive, extract) and the finish reviewer. Applied: the chip error is now tied to its group for screen readers; the close-band H2 is hidden visually under the logo; repeated lines are trimmed; "brand new" stays on one line in the phone H1; step numbers are a quiet navy tint; the gold accent was taken off the light-band heading; the H1 split waits up to 600ms for Cal Sans so the font doesn't swap mid-bounce; near-duplicate type sizes are merged.
- Checked in Chromium and WebKit at 360/390/414/430/1440: no sideways overflow, inputs ≥16px, the hero's primary button sits within the first screen (bottom at 460–495px of 800 on phones), the bounce-in runs and restores the plain H1, reduced motion and no-JS show everything, the floating circle is hidden on the hero, shown at services and hidden at the form, and the composed text decodes correctly.

## Not verified
- Real-device touch and the real SMS handoff on iOS/Android (sms: body tested by decoding the composed URL in Chromium and WebKit).
- Facebook in-app browser behaviour.
- Frame rate of the bounce-in on old phones.
