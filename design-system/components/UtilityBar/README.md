# UtilityBar

The teal strip above the nav carrying hours, address and the NOW SLICING ticker — the site's signature element.

**Consumer provides:** today's hours, the address, and the list of what is on the board (duplicated once so the loop is seamless).

**Rules**
- Teal fill sitting still; only the ticker moves (38s loop, stops under reduced motion).
- Mono 12px. Fixed facts in `sn-cream`, everything else `sn-cream-muted`.

**Flag:** `sn-cream-muted` on teal is 4.1:1 at 12px — below AA. Move the copy to full cream.