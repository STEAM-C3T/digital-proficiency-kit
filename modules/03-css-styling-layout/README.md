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

- Modern browser and text editor. DevTools are optional; resize the browser window to check responsive layouts.

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

## Your Route Through This Module

1. **Unit 3.1 — Style a page.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/03-css-styling-layout/units/3.1-css-fundamentals/tutorial/unit-3.1-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/03-css-styling-layout/units/3.1-css-fundamentals/workbook/unit-3.1-student-workbook.md). Change one style at a time and observe the result. **Checkpoint:** your headings, text, links, and spacing have a clear visual hierarchy.
2. **Practise Unit 3.1.** Complete [Style a Simple Portfolio Page](./tasks/task-1-style-a-portfolio.md). Save the page and stylesheet; use them as the starting point for the next unit.
3. **Unit 3.2 — Adapt the layout.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/03-css-styling-layout/units/3.2-responsive-layouts/tutorial/unit-3.2-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/03-css-styling-layout/units/3.2-responsive-layouts/workbook/unit-3.2-student-workbook.md). **Checkpoint:** resize the browser and observe the cards change from one column to two without horizontal scrolling.
4. **Apply the core layout skill.** Complete [Build a Responsive Grid Layout](./tasks/task-2-responsive-layout.md) with one breakpoint, using your saved page or the [responsive layout example](./examples/responsive-layout.html). Add a second breakpoint only if you are ready for the extension.
5. **Review and reflect.** Check the page at a narrow width and navigate links with Tab. Note one design decision that improved readability.

**What to keep:** your styled page, responsive version, and short breakpoint/design note. DevTools are useful but not required; resizing the browser is enough for the core check.

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
