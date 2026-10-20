# BuyPanel

The product decision block: centred header (eyebrow, teal H1, mono pricing), then one white panel holding every choice, split by hairlines.

**Blocks, in order:** claims · Cure swatches grouped by family · Amount buttons · constraint line · stock Tag + actions.

**Rules**
- H1 in `sn-heading-product` (teal), matching the add button (ratified Sep 2026).
- Swatches are grouped by cure family ("Cold-smoked · slices", "Cured, never smoked", "Hot-smoked · flakes") because the groups are facts.
- Amount buttons show amount and price only — portion guidance lives in the FAQ.
- Invalid combinations are disabled with a reason, never hidden. Never block: a change of mind rolls to the next valid amount and the constraint line says so.
- Local product pages carry no ship toggle; shipping lives at /ship/<product>.
- Ratified but not yet drawn: the double teal rule frame with the "A taste of nostalgia" corner motto, reserved for price-card elements like this panel.

**Flag:** the per-pound line and family labels use `sn-ink-faint` (2.7:1); faint is ruled for disabled controls only — move them to muted.