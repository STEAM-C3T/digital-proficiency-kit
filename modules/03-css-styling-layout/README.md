# Module 3: CSS Styling & Layout

Style content with typography and colour, then build responsive layouts with Grid and Flexbox.

## Learning Outcomes

- Applies CSS selectors and properties to control typography, colour, spacing, and hierarchy.
- Constructs responsive layouts using Flexbox and Grid with simple media queries.
- Evaluates contrast, focus, and readability for accessibility.

## Prerequisites

- Modules 1–2 or equivalent HTML fundamentals.

## Estimated Time

- 2–3 lessons (90–135 minutes) including hands‑on layout practice.

## Materials

- Modern browser with DevTools; text editor.

## Contents

- Units
  - [Unit 3.1 – Styling Basics](./units/unit-3.1-styling-basics.md) — Selectors, colour, typography, and the box model.
  - [Unit 3.2 – Layout & Responsive Design](./units/unit-3.2-layout-responsive.md) — Grid/Flexbox layouts and media queries.
- Examples
  - [style-basics.html](./examples/style-basics.html) — A styled page demonstrating hierarchy and spacing.
  - [responsive-layout.html](./examples/responsive-layout.html) — A simple, responsive card grid.
- Tasks
  - [Task: Style a Simple Portfolio Page](./tasks/task-1-style-a-portfolio.md) — Apply consistent typography and spacing.
  - [Task: Build a Responsive Grid Layout](./tasks/task-2-responsive-layout.md) — Implement adaptive columns using Grid.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Contrast, focus states, and assessment ideas.

## How This Module Works

1. Establish visual language: type scale, colours, spacing (Unit 3.1).
2. Build responsive layouts with Grid/Flexbox (Unit 3.2).
3. Explore the examples and replicate patterns in your project.
4. Complete tasks: style a portfolio; build a responsive grid.

## Student Instructions (Step‑by‑Step)

1. Choose a simple multi‑section page (from Modules 1–2 or provided example).
2. Add an external stylesheet and define a base scale (font sizes, line‑height, spacing).
3. Implement a consistent colour scheme with sufficient contrast; test focus states.
4. Use Flexbox or Grid to create a responsive layout (e.g., card grid that shifts columns).
5. Add media queries to adjust layout/typography at small/medium/large breakpoints.
6. Reflect on readability and accessibility tradeoffs.

## Acceptance Criteria (Module 3 Project)

- Consistency: Clear typographic hierarchy; consistent spacing and colours.
- Responsiveness: Layout adapts across at least two breakpoints without overflow.
- Accessibility: Contrast passes basic AA for body text; visible keyboard focus.
- Maintainability: Styles grouped logically; avoids excessive inline styling.
- Reflection: Notes on layout decisions and contrast checks.

## Accessibility Checklist

- Contrast: Check text/background contrast (WCAG AA as goal).
- Focus: Keyboard focus ring visible and not removed.
- Size: Avoid locking text sizes; allow browser zoom.

## Differentiation & Extensions

- Scaffold: Provide a style guide snippet (variables/custom properties) to use.
- Extension: Add a responsive navigation and a print style.

## Assessment & Evidence

- Use the layout-focused rubric (Teacher Toolkit) for responsiveness and readability.
- Evidence: HTML/CSS files, screenshots at multiple widths, short reflection.

## Teacher Toolkit Links

- [Module overview](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/03-css-styling-layout/module-overview.md)
- Lesson plans:
  - [Unit 3.1 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/03-css-styling-layout/unit-3.1-lesson-plan.md)
  - [Unit 3.2 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/03-css-styling-layout/unit-3.2-lesson-plan.md)
- [Assessment rubric](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/03-css-styling-layout/assessment-rubric-03.md)

## Quick Open (macOS)

```zsh
open ./examples/style-basics.html
open ./examples/responsive-layout.html
```

## Try it

- Resize the browser on the responsive example and observe the grid change.
- Check link focus states with the keyboard (Tab/Shift+Tab).
