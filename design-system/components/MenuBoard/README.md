# MenuBoard

The six counters as a menu board: big display names stacked down the left, the selected counter filling the right with its headline, a short description, a 5:3 photo well, four item cards and one primary button.

- Selected row is espresso with cream text and a right chevron, like a selected tab. Rows at rest are teal; hover is clay.
- Under 940px the same markup becomes an accordion: each row opens in place with a down/up chevron, one open at a time. Under 600px the photo moves above the copy (4:3) and items go two by two.
- No JavaScript. Each counter is a hidden radio, its label (the row) and its panel, in that order. Keyboard arrows move between counters. All panels are in the HTML, so crawlers read every counter.
- Item cards: name, price in mono with its unit ("$74.00 / 1/4 lb"), and an "Add to ticket" link whose accessible label names the product. Variable-weight items link to their product page rather than adding to the cart.
- The grid reserves one row per counter (`grid-template-rows: repeat(6, auto) 1fr`); change the count there if the counters change.
