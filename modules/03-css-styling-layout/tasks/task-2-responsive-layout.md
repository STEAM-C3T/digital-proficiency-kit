# Task: Build a Responsive Grid Layout

## Core task

Build a card grid that uses one column on a narrow screen and two columns above one breakpoint. Start with the provided responsive layout example or your saved Unit 3.1 page.

Suggested steps:

1. Add at least three cards inside a grid container.
2. Set the container to `display: grid` with one column and a consistent `gap`.
3. Add one media query (for example, `@media (min-width: 640px)`) that changes the grid to two columns.
4. Resize the browser across the breakpoint. Check that the cards reflow and the page does not scroll horizontally at 320px.
5. Tab through any links or buttons and confirm the focus outline remains visible. Record the breakpoint and why you chose it.

The core task needs one breakpoint. Add a second breakpoint for a three-column wide-screen layout as an optional extension.

Design goals:

- Implement a card grid that adapts from 1 column (narrow screen) to 2 columns (wide screen). A third column is optional.
- Keep spacing consistent and ensure readable typography at all sizes.

Acceptance criteria:

- Uses CSS Grid for the outer layout; optional Flexbox inside cards.
- Includes one working media query breakpoint; a second breakpoint is optional.
- No horizontal scrolling at 320px; focus outlines remain visible.

Deliverable:

- A single HTML file with embedded CSS or separate `.css` file.
- Short note: Which breakpoints did you choose and why?
