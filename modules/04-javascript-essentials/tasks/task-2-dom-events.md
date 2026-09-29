# Task: Build a Small Dynamic UI

Design goals:

- Build a small list interface: accept a non-empty item, store it in a JavaScript array, and render the current array on the page.
- Keep state in JS and render from state; avoid inline HTML event attributes.

Suggested steps:

1. Start with the provided HTML form and an empty list in the page.
2. Select the form, input, and list elements. Check that each selection finds the intended element.
3. Create an empty array and a `renderItems()` function. First render the empty array.
4. Listen for the form's `submit` event and prevent the page from reloading.
5. Ignore blank input. For valid text, add it to the array, clear the input, then call `renderItems()`.
6. Test with one item, several items, and blank input. Explain how the array and displayed list relate.

Optional extensions: mark items complete, delete items, add filters or counts, and save between visits.

Acceptance criteria:

- Uses `addEventListener` for event handling and `classList`/`textContent` for DOM updates.
- Prevents default form submission and handles empty input.
- Adding valid text updates both the array and rendered list; the page does not reload.
- Includes accessible labels and maintains focus order.

Deliverable:

- One HTML file with embedded JS (or a separate JS file) and a short comment explaining your state shape.
