# Module 4: JavaScript Essentials

Add interactivity with JavaScript by handling events and updating the DOM. Build small, stateful interfaces.

## Learning Outcomes

- Writes basic JavaScript to query the DOM, register event listeners, and update content.
- Manages simple UI state and renders from state deterministically.
- Applies progressive enhancement: page remains usable without JS.

## Prerequisites

- Modules 1–3 or equivalent HTML/CSS familiarity.

## Estimated Time

- 2–3 lessons (90–135 minutes) including practice time.

## Materials

- Modern browser with DevTools console; text editor.

## Contents

- Units
  - [Unit 4.1 – JS Basics + DOM](./units/unit-4.1-js-basics-dom.md) — Variables, events, selecting elements, and updating content.
  - [Unit 4.2 – DOM Events & Dynamic UI](./units/unit-4.2-dom-events.md) — Forms, lists, state, and rendering patterns.
- Examples
  - [dom-interactions.html](./examples/dom-interactions.html) — A simple counter with accessible updates.
  - [todo-list.html](./examples/todo-list.html) — Add, toggle, and filter items with basic state management.
- Tasks
  - [Task: Add Interactivity to a Page](./tasks/task-1-interactive-elements.md) — Progressive enhancement with event listeners.
  - [Task: Build a Small Dynamic UI](./tasks/task-2-dom-events.md) — Keep state in JS and render from it.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Tips for accessibility and incremental complexity.

## How This Module Works

1. Learn JS + DOM fundamentals (Unit 4.1).
2. Handle DOM events and manage stateful UI (Unit 4.2).
3. Explore examples, then implement tasks that progressively enhance an existing page.

## Student Instructions (Step‑by‑Step)

1. Open `examples/dom-interactions.html` and observe how event listeners change the DOM.
2. Build a tiny interactive component (e.g., counter or toggler) using `addEventListener`.
3. For a small list‑based UI (e.g., to‑do), store items in an array and render from state.
4. Ensure keyboard activation works (Enter/Space on buttons/controls) and announce changes accessibly (e.g., update text).
5. Reflect on what state your app keeps and when re‑rendering occurs.

## Acceptance Criteria (Module 4 Project)

- Functionality: Interaction works reliably (add/toggle/update or similar behavior).
- State: UI derived from an internal state object/array; clear rendering function.
- Accessibility: Controls are keyboard operable with discernible text; updates visible.
- Progressive Enhancement: Page content remains usable without JS.
- Reflection: Notes on event flow and state updates.

## Accessibility Checklist

- Controls: Use semantic buttons or add proper ARIA/keyboard handlers if needed.
- Focus: Ensure focus management when adding/removing elements.
- Feedback: Provide visible text updates; avoid purely visual feedback.

## Differentiation & Extensions

- Scaffold: Starter HTML with IDs and a basic render function.
- Extension: Add filtering or simple persistence (e.g., `localStorage`).

## Assessment & Evidence

- Use the JS rubric (Teacher Toolkit) for functionality, state, and accessibility.
- Evidence: HTML/JS files, short video or notes demonstrating interaction.

## Teacher Toolkit Links

- Module overview: https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/module-overview.md
- Lesson plans:
  - https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/unit-4.1-lesson-plan.md
  - https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/unit-4.2-lesson-plan.md
- Assessment rubric: https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/assessment-rubric-04.md

## Quick Open (macOS)

```zsh
open ./examples/dom-interactions.html
open ./examples/todo-list.html
```

## Try it

- Open the examples and interact with the controls. Inspect how `addEventListener` changes the interface.
- Discuss how state is stored and what triggers re‑rendering.
