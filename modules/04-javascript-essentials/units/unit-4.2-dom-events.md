# Module 4: JavaScript Essentials

## Unit 4.2 – DOM Events & Dynamic UI: Forms, Lists, and State

**Learning outcomes:**

- Student handles common DOM events (`click`, `input`, `submit`).
- Student renders state safely with `textContent`; using `classList` for completion styling is an optional extension.
- Student structures small UI logic into functions.

**Teacher-notes:**

- Prevent default form submission for in-page demos (`event.preventDefault()`).
- Separate state from view: compute state, then render the UI.
- Encourage keyboard accessibility (labels, focus order).

**Core classroom task:**

- Build a small list that accepts a non-empty item, stores it in an array, and renders the array on the page. Completion toggles, deletion, filters, and persistence are optional extensions.

**Starter example:** See `examples/todo-list.html` for a complete reference. Build the core first; the example’s extra features are optional.

**Reflection prompt:**

- How did you store item state? Why that structure?
- What events did you listen to, and how do they change rendering?
