# Module 4: JavaScript Essentials

Learn JavaScript fundamentals, then use events and DOM updates to build small, stateful interfaces.

## Learning Outcomes

- Uses variables, expressions, functions, and conditions to solve a small problem.
- Connects an event to a function and updates page content safely.
- Manages simple UI state and renders from state deterministically.
- Applies progressive enhancement: page remains usable without JS.

## Prerequisites

- Modules 1–3 or equivalent HTML/CSS familiarity.

## Estimated Time

- 2–3 lessons (90–135 minutes) including practice time.

## Materials

- Modern browser and text editor; DevTools are optional for debugging.

## Contents

- Units
  - [Unit 4.1 – JavaScript Basics and a First Interaction](./units/unit-4.1-js-basics-dom.md) — Variables, values, operators, functions, conditions, and a small event-driven calculator.
  - [Unit 4.2 – DOM Events & Dynamic UI](./units/unit-4.2-dom-events.md) — Forms, lists, state, and rendering patterns.
- Examples
  - [javascript-basics.html](./examples/javascript-basics.html) — A labeled calculator using functions, conditions, and a form event.
  - [dom-interactions.html](./examples/dom-interactions.html) — A simple counter with accessible updates.
  - [todo-list.html](./examples/todo-list.html) — Add, toggle, and filter items with basic state management.
- Tasks
  - [Task: Add Interactivity to a Page](./tasks/task-1-interactive-elements.md) — Progressive enhancement with event listeners.
  - [Task: Build a Small Dynamic UI](./tasks/task-2-dom-events.md) — Keep state in JS and render from it.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Tips for accessibility and incremental complexity.

## How This Module Works

1. Learn JavaScript fundamentals and connect one form event to a function (Unit 4.1).
2. Use DOM events and arrays to build a small list UI (Unit 4.2); completion, deletion, filtering, and persistence are optional extensions.
3. Explore examples, then implement tasks that progressively enhance an existing page.

## Your Route Through This Module

1. **Unit 4.1 — Make a first interaction.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/04-javascript-essentials/units/4.1-javascript-basics/tutorial/unit-4.1-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/04-javascript-essentials/units/4.1-javascript-basics/workbook/unit-4.1-student-workbook.md). Trace the [calculator example](./examples/javascript-basics.html), predict an answer, then try it. **Checkpoint:** explain which function calculates the answer and which event calls it. Console experiments, arrays, and loops are optional; DevTools are not required.
2. **Practise Unit 4.1.** Complete [Build a First JavaScript Calculator](./tasks/task-1-interactive-elements.md). Save the working file before moving on.
3. **Unit 4.2 — Keep a small interface in sync with state.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/04-javascript-essentials/units/4.2-dom-manipulation/tutorial/unit-4.2-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/04-javascript-essentials/units/4.2-dom-manipulation/workbook/unit-4.2-student-workbook.md). Explore the [todo example](./examples/todo-list.html). **Checkpoint:** describe what changes in the array when an item is added, and how the page is rendered from it. Toggling items is optional extension work.
4. **Build and check.** Complete [Build a Small Dynamic UI](./tasks/task-2-dom-events.md). Test valid and empty input, then check how the page responds. Native form submission also supports the keyboard.
5. **Reflect.** Describe one event, the state change it causes, and how the user sees the result.

**What to keep:** your calculator, dynamic interface, and short event/state explanation. Browser DevTools can help you read errors, but they are not required.

## Student Instructions (Step‑by‑Step)

1. Open `examples/javascript-basics.html` and trace how the inputs reach the calculation function.
2. Predict the result of a calculation, run it, and try an invalid input.
3. In Unit 4.2, use an array to store list items and render the visible items from that state.
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

- [Module overview](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/module-overview.md)
- Lesson plans:
  - [Unit 4.1 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/unit-4.1-lesson-plan.md)
  - [Unit 4.2 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/unit-4.2-lesson-plan.md)
- [Assessment rubric](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/04-javascript-essentials/assessment-rubric-04.md)

## Quick Open (macOS)

```zsh
open ./examples/javascript-basics.html
open ./examples/dom-interactions.html
open ./examples/todo-list.html
```

## Try it

- Open the examples and interact with the controls. Inspect how `addEventListener` changes the interface.
- Discuss how state is stored and what triggers re‑rendering.
