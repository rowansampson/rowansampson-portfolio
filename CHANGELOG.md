# Changelog

All notable changes to the portfolio, in public.

---

## v3.5.8 — 2026-08-20
### Mobile header fit — verified across a 14-width device matrix
- Header controls now sit tight beside the brand on mobile (10px gap; was ~470px dead space with 24px right-edge clipping)
- Compact mobile metrics: 58px header, 28px mark, tightened control padding, CTA and dropdown at 30px
- Narrow devices (≤360px) get a compact CTA label ("LIVE ↗"); full label returns at 375px+
- Verified in headless Chromium: 320–1440px matrix, 14/14 widths pass (zero overflow, zero overlap, cy-spread 0)
- Touch-verified at 390px: dropdown opens in-viewport, trilingual tap switching works, no overflow
- Full interaction regression: 15/15 green, zero console errors

## v3.5.7 — 2026-08-20
### Header fit, collaborative framing, i18n round-trip fix
- Header: nav links now sit beside the brand (dead gap reduced from ~264px to 24px), controls tightened to a uniform 32px height
- Framing: "sole developer" replaced with "lead developer" across the site, CVs, bios and GitHub profile; production claims reframed to Digital Origin
- i18n engine: English now fully restores after switching back from isiXhosa / Afrikaans (snapshot-based restore for all data-i18n elements, status label, map hint and document title)
- Verified in headless Chromium at 5 viewports: zero overflow/overlap, uniform controls; 14 interaction checks green; map hover verified on both nodes

## v3.5.6 — 2026-08-20
### Story section removed per directive
- "The story, in short" narrative block removed (HTML, CSS, and both i18n dictionaries)
- All v3.5.5 engagement work retained: live links on every mock CTA, clickable contact cards, WhatsApp card, 56px bridge gap
- Footer build line corrected (silent version-bump gap since v3.5.3 fixed with an asserted replace)

## v3.5.5 — 2026-08-20
### Story, engagement, zero dead buttons
- **The Story**: first-person narrative block in the Track Record section (Gelvandale → SRC committees → field years → national office → Digital Origin), benchmark-grounded (who + proof + human touch), localized EN / isiXhosa / Afrikaans
- **Zero dead buttons**: every mock CTA is now a real link — email sample CTA, landing mock CTAs, three ad variants, and the journal cover all link to live destinations
- **Contact cards fully clickable**: each card is a link (mailto / tel / WhatsApp / LinkedIn), plus a dedicated WhatsApp card (4-card grid), copy buttons kept valid outside anchors
- **Spacing**: bridge-to-contact gap fixed at 56px (deterministic margin on the grid, verified post-reveal in Chromium)
- Regression: 5 viewports clean (zero overflow/overlap, aligned header controls), 16/16 interactions, zero console errors

## v3.5.4 — 2026-08-19
### Polish layer (measured, non-breaking)
- Anchor landing fixed: scroll-margin-top 80px — sections now land below the sticky header (verified: hash nav 80px, bridge click 116px)
- Native dark color-scheme: form controls, scrollbars and autofill render dark system-wide
- Typography craft: text-wrap balance + optimizeLegibility on all headings
- Register point: gold full stop after the hero name, echoing the mark's diamond
- Staggered reveal delays via data-d (80/160/240ms) — reduced-motion aware
- Custom thin scrollbar (green on hover) · ticker pauses on hover · press states on buttons
- Focus ring on accordion summaries · print @page margin 14mm · tap-highlight off on mobile
- Hover affordance unified on contact, ad and mock cards · image drag disabled
- Regression verified in headless Chromium: 5 viewports zero overlap/overflow, 15/15 interactions, zero console errors

## v3.5.3 — 2026-08-19
### Header rebuild, signal bridges, footer connection
- Header rebuilt as a single control system: 60px height, single-line brand, all elements on one vertical center (measured spread: 0px), dropdown and CTA at identical 34px control height, stale CSS removed
- Verified at 5 viewports in headless Chromium: zero overlap, zero overflow, progressive disclosure (9 → 6 → 3 items)
- Two signal bridges added (gold rule, distinct from navigation bridges):
  · Craft check — live print discipline: "Export this page" triggers the print stylesheet (clean A4 brief, no chrome, no trackers)
  · Keyboard check — live a11y: "Open commands ⌘K" opens the command palette
- Both bridges localized in EN / isiXhosa / Afrikaans
- GitHub added to the footer Connect column
- 15/15 interaction tests pass in real Chromium, zero console errors

## v3.5.2 — 2026-08-19
### Layout coherence pass (browser-verified)
- Section rhythm tightened: clamp(64px, 7.5vw, 80px) padding, tuned sec-head margins
- Navigation now persists at tablet widths (Case Study, Automation, Track Record visible to 760px)
- Section-tracker chip relocated to bottom-right, clear of the header
- Verified in headless Chromium at 5 viewports: no horizontal overflow, no off-screen nav items, zero console errors
- Verified interactively: dropdown, trilingual switch, command palette, bridges, accordions, copy, map, terminal, ticker, clock, FAB

## v3.5.1 — 2026-08-19
### Canonical deployment
- Canonical URL set: rowan-sampson-portfolio.vercel.app (link rel=canonical + og:url)
- GitHub Pages kept as a mirror; repo homepages and profile link to the primary deployment
- Footer carries the build number and canonical host

---

## v3.4 — 2026-08-19
### The RS Register Mark
- Custom brand identity designed and approved: woven RS monogram + gold register point
- Live in favicon, nav and footer; full suite (primary, duotone, light, lockup)
- Deployed and claimed to a permanent Vercel project

## v3.3 — 2026-08-19
### Identity, overflow fixes, copy samples
- Horizontal overflow root-caused and fixed (nav collapse, language switcher cycling on mobile)
- ⌘K launcher relocated to a floating bottom-left button
- Writing section rebuilt: 5 contemporary copy formats (technical ×2, essay, email, ads, landing)
- Command palette numbering corrected

## v3.2 — 2026-08-19
### High-tech presentation pass
- Spacing token system (`--sect` clamp) across all sections
- Header: scroll-state, active underline, responsive collapse
- Retention bridges between sections + spec chips + section tracker
- Footer rebuild: capability ticker, live clock, "Powered by Digital Origin"

## v3.0 — 2026-08-19
### The dynamic pack
- Live platform status beacon · live Core Web Vitals · ⌘K command palette
- Terminal deploy log · reading progress · scrollspy · copy-to-clipboard
- Trilingual engine (EN / isiXhosa / Afrikaans) · interactive six-cluster map
- Writing & Thinking section

## v2.1 — 2026-08-19
- Newsletter & email automation sequences presented as an active project
- Bloemfontein relocation · reference set updated

## v2.0 — 2026-08-19
- Rebuild from design reconnaissance: conversion-first architecture
- Build-led case study with verified-on-live-site audit rail
- Campaign statistics archived (policy: metrics must belong to the builder)

## v1.x — 2026-08
- Initial editorial build, hero, impact pillars, case study, endorsements
- Portrait enhancement and aspect-correct framing

## v3.5 — 2026-08-19
### Audit round: structure, voice, precision
- Language switch converted to a proper dropdown (mobile-safe, keyboard accessible)
- Retention bridges relocated to section ends, each pointing to the next section
- Copy pass across the site: em-dash density reduced, AI-voice patterns removed, concrete detail added
- Writing samples rewritten for human voice across all five formats
- YCLSA title corrected to "Office of the National Secretary"
