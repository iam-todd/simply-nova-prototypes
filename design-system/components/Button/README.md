# Button

Two buttons only: `.btn` (primary, teal fill) and `.btn-2` (secondary, espresso outline, never filled).

**Consumer provides:** an `<a>` or `<button>` with the class and a verb label. Add `.wide` for full width inside the buy panel. Disabled primary is `aria-disabled="true"` and reads "Sold out" or "Choose an available amount".

**Rules**
- Rest is teal (`sn-teal`; `sn-teal-onink` on espresso). Hover, focus and active go solid clay with cream text. Never clay at rest.
- One filled button per view. Repeated product actions ("Add to ticket" on three spread tickets) are `.btn-2`. Open ruling: three product cards each want a primary.
- Minimum height 44px, always. Repeated buttons carry the product name in their accessible label.
- Labels are counter language: "Add to ticket", "Build a spread", "Ship this overnight instead". No "Shop now", no "Learn more".

**Flag:** `sn-btn2-border` is 1.6:1 against cream, below the 3:1 floor for control borders.