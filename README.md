# Simply Nova — Web Prototypes

Interactive design prototypes for the rebuild of [simplynovanyc.com](https://simplynovanyc.com), the website for **Simply Nova**, a classic appetizing shop at 754 Metropolitan Ave in Williamsburg, Brooklyn. The shop sells hand-sliced smoked fish, bagels and deli at the counter, ships nationwide, and does NYC catering.

Every file here is a single self-contained HTML page — no build step, no dependencies beyond Google Fonts. Open one in a browser and it works.

**▶ Live demo:** https://USERNAME.github.io/simply-nova-prototypes/

---

## What's in here

| Prototype | What it explores |
|---|---|
| [Homepage v3](simply-nova-homepage-v3.html) | One homepage serving three businesses — counter pickup/delivery, nationwide shipping, catering. "Three doors" reorder by visitor location; the hero headline changes with the time of day; ZIP check runs *before* the cart. |
| [Local pickup module](simply-nova-local-module-concepts.html) | Three ways to surface pickup to nearby visitors on a shipping-first page: a counter-ticket stub, a scroll-triggered bar, and an in-flow menu band. |
| [Web design guidelines](simply-nova-guidelines.html) | The locked design system: four colors with four jobs, three typefaces, live component states, voice rules, and a 12-point quality floor developers check before shipping. |
| [Editorial: The Schmaltz + Fish Primer](simply-nova-editorial.html) | Blog index in three layouts (broadsheet, counter board, hybrid), an article template with product popovers and a guest-count bundle, and a Fish Primer with hand-drawn SVG specimen plates and side-by-side compare. |
| [Product page module rules](simply-nova-module-rules.html) | A rules engine deciding which modules appear on which product page — always-on, by page type, data-gated, or hand-picked — with the structured-data schema each page outputs. |

## Design system

**[Simply Nova Design System →](design-system/)** · [interactive version](https://claude.ai/artifact/YPQa1RonD3VqdGwGPMbiJp)

The production design system the prototypes grew into: a full brand book (voice, color roles, type, layout, states, accessibility), `tokens.json` with a usage note on every token, the component stylesheet, and guidelines for 35 components — from Button and Tag up to MenuBoard, BuyPanel and PortionCalculator. The theme's `tokens.css` is the master copy; this is a snapshot from 19 Oct 2026.

## How to use them

Each prototype has its own controls at the top or bottom of the page:

- **Skin / View** toggles switch between design directions.
- **Visitor / Time / Data** toggles simulate different customers and launch states.
- **Notes** reveals the design reasoning inline, next to the thing it explains. Turn it on — that's where the thinking is.

## Design system at a glance

| Role | Value |
|---|---|
| Surface | Cream `#F5F0E8` |
| Ink | Espresso `#2C2418` |
| Rest state (buttons, links) | Teal `#046049` on light · `#0FBF9A` on dark |
| Interaction (hover, focus) | Clay `#A8442A` |
| Display | Barlow Condensed |
| Body | DM Sans |
| Utility (prices, weights, times) | DM Mono |

Hard rules: solid clay never appears at rest, and teal never appears on hover.

> **A note on Homepage v3 and the local module concepts:** these predate the locked design system. They use the earlier exploratory "skins" (Bevan, Fraunces, gold accents) that were later retired. They're kept here for the structural ideas — the three-door layout and visitor states carried forward; the styling did not.

## Stack these are designed for

WordPress + WooCommerce on the Kadence theme, with a custom `snn-*` plugin suite. The prototypes are specs, not production code — the guidelines page is the contract for the build.

## Status

Prototypes and specs. Product names, prices, counts and copy are placeholders unless noted.

---

© 2026 Simply Nova LLC. Shared for portfolio purposes.
