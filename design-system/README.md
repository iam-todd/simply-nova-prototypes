# Simply Nova Design System

**Interactive version:** https://claude.ai/artifact/YPQa1RonD3VqdGwGPMbiJp

This folder is a snapshot of that system (synced 19 Oct 2026): the brand book below, `tokens.json` (every color, type style, spacing, radius and shadow token with its usage note), `components/bundle.css`, and a guideline README for each of the 35 components under `components/`.

---

Simply Nova is an appetizing counter at 754 Metropolitan Avenue in East Williamsburg, Brooklyn. The site should feel like standing at that counter: printed, plain-spoken, a little old New York, with the fish doing the talking. This page documents simplynovanyc.com. The master copy of every value is the theme's `tokens.css` in the snn-custom repo; when the two disagree, the theme wins.

## Content fundamentals

- Write like the person behind the counter. Short declarative sentences, first person plural, second person to the customer: "Tell us the day and how many, and we will do the arithmetic."
- Be specific over persuasive. Name the cure, the weight, the day. "Two left for Sunday", "Cut the morning it leaves", "Brined 18 hours, then cold-smoked over apple".
- Headlines say plainly what the section or page is — no opinions, no slogans — unless the wording has search value. Lead with the words people search: "Smoked fish", "Catering in Brooklyn", "How much smoked salmon per person".
- Answer sections may use the customer's own question as the H2, ending in a question mark: "What's the difference between nova and lox?", "How much lox should I order per person?". The answer sits directly under it in plain text, so search and answer engines can quote it.
- Eyebrows carry the category and place words a headline leaves out: "Appetizing & deli · six counters", "Ask us anything · nova, lox, gravlax, belly".
- Button labels are counter verbs: "Add to ticket", "Build a spread", "Ship this overnight instead". Never "Shop now" or "Learn more".
- Fractions with a slash ("1/2 lb", "1 1/2"), never glyphs. Prices always with cents ("$74.00"). In mockups, a price not yet confirmed is written "$__.__".
- No exclamation marks, no emoji, no superlatives, no invented urgency. Scarcity only when it is true and dated.
- Every page names the neighbourhood and the street at least once.

## Visual foundations

**Colour is a four-role system.** Cream (`sn-cream`) is the ground. Espresso (`sn-espresso`) is ink and structure. Teal (`sn-teal`) is the rest state of anything you can press. Clay (`sn-clay`) is interaction only: hover, focus, active.
- Set text in `sn-espresso` on `sn-cream` and `sn-raised`. Secondary text is `sn-ink-muted`. `sn-ink-faint` is for disabled controls only.
- Links and primary buttons are `sn-teal` on light grounds and `sn-teal-onink` on espresso. Never cross the two.
- Clay never appears at rest. The one exception is its pale form: `sn-clay-tint` with `sn-clay-ink` marks scarcity on a Tag, never on anything clickable. Absence uses `sn-status-bg` with `sn-status-ink`.
- Espresso as a surface is budgeted: the footer, selected toggles and tabs — including the open row of the counter accordion, which is the MenuBoard's tab at narrow widths. The header and hero stay cream.
- White (`sn-raised`) is the only raised surface: tickets, primer terms, the buy panel, reviews, pair cards.
- Bone (`sn-alt`) is a cream tint for alternating rows only, with full espresso ink on it.
- Headings (H1–H3) are `sn-heading`, which points to `sn-teal-deep` (#04503F). The product-page H1 is `sn-heading-product` (teal), matching its Add to ticket button. On espresso, headings are cream.
- Navigation colors live in one place, the `sn-nav-*` tokens: items, current page, hover, kicker, mega menu, footer and breadcrumb. Nav items and their script kickers rest in teal like every other link.
- Gold and the print teal (#069B7D) are print-only and not part of the web system.

**Type is four faces and no more.** Barlow Condensed 700, uppercase, for display (`display-*`, `wordmark`). DM Sans for everything read (`body`, `lede`, `quote`). DM Mono for shop data (`price`, `label`, `eyebrow`, `address`): prices, weights, cure methods, dates, addresses. Caveat script (`kicker`), by ruling, for kickers above nav items and single-line asides only — never body copy, headings or buttons. Inside a display headline, change voice with DM Sans italic lowercase (see CateringHeadline). Body copy is 16px minimum.

**Space and layout.** Content width `wrap` (1180px, 92vw). Homepage sections `space-88` top and bottom, product modules `space-76`, 56px on mobile. One breakpoint at 940px. Card grids may take one more step at 600px (MenuBoard item cards to two columns, Primer to one), and the wrap narrows to 16px gutters at 400px. No others. Sections, and the nav from the page, are divided by a 1px `sn-rule` hairline. There is no heavier rule. Mobile-first and responsive only — no per-device layouts.

**Shape.** Radii step with size: `radius-chip` 4, `radius-button` 8, `radius-control` 10, `radius-card` 12, `radius-card-lg` 14, `radius-panel` 16. Borders do the work, not shadows: `sn-border` hairlines on everything, `shadow-panel` on the buy panel only.

**States.** Hover, focus and active all resolve to clay: fills go solid clay with cream text, outlines and text go clay. Focus-visible is a 3px `sn-clay-focus` outline offset 2px. Selected (a toggle, a tab, a chosen swatch) is espresso: a fill or a 2px border. Disabled is 34% opacity or the faint-espresso fill, with a reason in the title. Nothing depends on hover to be understood.

**Imagery.** Real product, real hands, real counter. Stills are shot to fixed ratios (4:5 tiles and mega-menu features at 400×520, 4:3 cards, 5:3 rail, 1:1 gallery, 16:9 hero). Motion is short silent loops (hand-slicing, 6s) with a visible pause. Until a photo exists, a Well names the shot in mono.

**Motion.** Colour transitions at .15s. The ticker is the only thing that moves on its own; QuoteSlider moves only when asked and never autoplays. Everything stops under reduced motion.

**Accessibility.** Every interactive element, links included, is at least 44px tall on touch. Repeated buttons carry the product name in their accessible label. Production CSS uses rem.

## Scripts

No JavaScript by default. Tabs and accordions are CSS-only — a hidden radio per option (MenuBoard) or native `<details>` (FAQ) — so every panel is in the HTML for crawlers and works with JavaScript off. The one scripted exception is QuoteSlider's arrows and dots (about 20 lines); without it the quotes still swipe and scroll, and the controls stay hidden.

## The counters

Six counters, in this order. The name is set in display type; the line after it is its mono label.

- Appetizing · Smoked & cured fish
- Caviar · Sturgeon & roe
- Salads · Salads & spreads
- Deli · Carved meats & pickles
- Bakery · Sweets & bagels
- Provisions · Pantry & bread

They appear on the homepage as the MenuBoard. The nav and mega menu do not reflect them yet (see Open decisions).

## Iconography

No icon set. The system uses typographic marks: a middle dot as separator and list bullet, a slash in breadcrumbs, ✓ and ✕ in comparisons, ★ for ratings, and a CSS chevron for disclosure. The brand's three-fish "S" logo mark has no web file in this system yet; the wordmark is set in Barlow Condensed.

## Open decisions

- One filled button per view versus three product cards each wanting a primary.
- Nav items: the mockup's set versus the decisions-log set with a seasonal right-side button.
- Nav and mega menu: frozen while being redesigned (Oct 2026). Don't change the `sn-nav-*` tokens or the mega-menu structure from here; the six counters are not reflected there yet.
- Counter overlaps: bagels and bialys sit in both Bakery and Provisions; pickles in both Deli and Provisions.
- QuoteSlider sets its quote at up to 36px, larger than the `quote` style (21–28px), because it stands alone. Ratify, or bring it back to `quote`.

## Known contrast gaps (kept exact from the mockups)

- `sn-ink-faint` (2.7:1) used as text for per-pound price, cure family labels, review bylines and dt labels: move to `sn-ink-muted`.
- `sn-cream-muted` on the teal utility bar is 4.1:1 at 12px: use `sn-cream`.
- `sn-btn2-border` is 1.6:1, under 3:1 for control borders.
- `sn-ink-muted` on bone is 4.0:1.
- Several secondary lines are 13.5–15px, under the 16px body floor.
