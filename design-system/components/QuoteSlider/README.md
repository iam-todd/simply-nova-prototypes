# QuoteSlider

Press quotes, one at a time: the quote large in DM Sans, the outlet and month in mono, a "Read the story" link to the original article, then round arrow buttons either side of three dots.

- The track is a native horizontal scroll with snap, so quotes swipe on a phone with no script. A small script wires the arrows and dots, keeps the current dot filled espresso, loops from the last quote to the first, and un-hides the controls; without it the controls stay hidden.
- Never autoplays. Smooth scrolling stops under reduced motion.
- Arrows are 44px circles with a CSS chevron, teal at rest and clay on hover. Dots are 10px rings in a 44px target; the current one fills espresso.
- Quote real press only, with outlet and month, and link to the story. The quote is up to 36px — larger than the `quote` style — while that is an open decision.
