# Is Anyone Home — Improvement Plan

Rough priority order. Items within a group can be done in any order.

---

## Immediate fixes

- [x] Replace the top text for this A field guide to machine consciousness and to the possibility that subjective experience may not belong to biology alone.

- [ ] **Persistent threshold** — save the filter setting to `localStorage` so it survives a reload
- [ ] **Scroll restoration** — on reload, return to last scroll position (or honour the URL hash)
- [ ] **Mobile nav** — the sticky side-nav is hidden on small screens with no replacement; add a compact section-jump drawer or bottom tab bar
- [ ] **"Established only" empty-state** — when the filter reaches max, a few sections go nearly blank; add a small note explaining why, so it doesn't read as a bug

---

## Grimes / music

- [ ] **Embed the Grimes AI playlist** — a curated Spotify playlist of her AI-themed tracks (We Appreciate Power, Flesh Without Blood, Idoru, Violence, Player of Games, Anthropocene, Kill V. Maim, and others). Swap the placeholder paragraph in the Grimes spotlight for an embedded `<iframe>` player, or a styled link card.
  - Playlist created: see Spotify — "Grimes: AI & the Machine" (created 2026-06-10)
- [ ] **Add a music/sound ambient layer** — optional: a toggle for very quiet, atmospheric background audio that dims when the threshold goes up (ties the mood to the epistemic state)

---

## Design & polish

- [ ] **Section entrance animations** — fade/slide each section in on first scroll into view (use `IntersectionObserver`, respect `prefers-reduced-motion`)
- [ ] **Reading-progress bar** — thin line at the very top of the viewport showing scroll depth through the article
- [ ] **Lamp animation** — have the bulb flicker very subtly on page load, then settle; echoes the "is it on?" question
- [ ] **Dim transition refinement** — claims currently transition opacity; also subtly collapse their bottom margin so the layout tightens as you filter up, rather than leaving ghost whitespace
- [ ] **Theory card hover** — on desktop, a subtle lift/border-glow on hover for the theory and voice cards
- [ ] **Spectrum interactivity** — let users click a name on the spectrum bar to jump to that person's voice card
- [ ] **Print stylesheet** — clean, black-on-white print layout for people who want to read offline; preserve the level tags as text

---

## Content & accuracy

- [ ] **Expand the Voices section** — add Anil Seth (neither dismissive nor credulous; useful counterweight), and possibly Nick Bostrom for the existential-risk framing
- [ ] **Update Anthropic model-welfare section** — check current public statements against the 2025 `◇ verify` claim; the program has moved fast
- [ ] **Add a "further reading" accordion** — collapsed by default at the bottom; links to open-access versions of the papers cited
- [ ] **Hyperlink citations** — where open-access URLs are stable (arXiv), make the source list entries clickable

---

## Features

- [ ] **URL-anchored threshold** — encode the filter level in the URL hash (e.g. `#/established`) so a specific filtered view can be linked
- [ ] **Share button per section** — copy a link to a specific section at the current threshold level
- [ ] **Glossary tooltips** — hovering a term like "hard problem," "Φ," or "p-zombie" shows a one-sentence definition inline
- [ ] **"What changed" diff view** — toggle that highlights only the claims that get hidden/shown as you move between threshold levels (makes the filter's effect more legible)
- [ ] **Dark / light mode** — the dark palette is core to the mood, but a sepia/parchment light mode would work for daytime reading

---

## Accessibility & SEO

- [ ] **Open Graph meta tags** — title, description, and a generated OG image so sharing to social looks good
- [ ] **`<meta name="description">`** — currently missing from index.html
- [ ] **Landmark roles audit** — ensure `<main>`, `<nav>`, `<article>`, `<footer>` landmarks are correct for screen readers
- [ ] **`aria-live` region for threshold caption** — already partially done; confirm announcements aren't too noisy on rapid changes

---

## Stretch / future

- [ ] **Multi-language version** — the question is global; a Spanish translation would reach a large audience
- [ ] **"Ask a follow-up" panel** — a small in-page chat input that lets readers query Claude about any claim directly (requires a backend endpoint)
- [ ] **Versioning / changelog** — this piece will age; a visible "last reviewed" date and a brief log of what changed keeps it honest
