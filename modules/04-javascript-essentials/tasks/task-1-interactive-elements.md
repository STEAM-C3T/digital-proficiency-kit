# Task: Add Interactivity to a Page

Design goals:

- Add at least one interactive control (button, input) that updates the DOM.
- Use `addEventListener` (no inline `onclick`).
- Keep behaviour separate from structure (progressive enhancement friendly).

Acceptance criteria:

- Uses `querySelector`/`classList` to select/modify elements.
- Handles empty or invalid input gracefully (no errors).
- Includes accessible labelling and `aria-live` where dynamic text changes.
- JS is placed at the end of `<body>`; no blocking alerts on load.

Deliverable:

- One HTML file with embedded JS or a separate `.js` file.
- Brief comment (2–3 sentences) describing the event handled and the DOM changes performed.
