# Module 5: Data & Visualization

Represent small datasets visually using Canvas or SVG. Focus on mapping values to sizes/positions and clear labelling.

## Learning Outcomes

- Maps numeric data to visual encodings (length, position, colour) with clear labels.
- Explains scaling and axis choices for simple charts.
- Pairs visualizations with tables to support accessibility and verification.

## Prerequisites

- Modules 1–4 or equivalent HTML/CSS/JS basics.

## Estimated Time

- 2 lessons (90 minutes) depending on dataset exploration.

## Materials

- Browser with Canvas/SVG support (modern browsers), text editor.

## Contents

- Units
  - [Unit 5.1 – Canvas Basics: Simple Bar Chart](./units/unit-5.1-canvas-basics.md) — Draw bars from an array of values; label clearly.
- Examples
  - [canvas-bar-chart.html](./examples/canvas-bar-chart.html) — CO₂ savings as a labelled bar chart.
- Tasks
  - [Task: Visualize a Small Dataset](./tasks/task-1-visualize-dataset.md) — Pick a dataset, choose a chart form, and explain scaling.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Accessibility tips (pair with a table), extension ideas.

## How This Module Works

1. Learn Canvas basics via Unit 5.1 and the example bar chart.
2. Choose a small dataset and decide on a chart form (bar/line/strip).
3. Implement scaling, draw marks, and label axes/values clearly.
4. Provide a companion HTML table for screen reader access.

## Student Instructions (Step‑by‑Step)

1. Open `examples/canvas-bar-chart.html`; change the `data` array and observe the result.
2. Select a meaningful dataset (5–12 values) and describe what each value represents.
3. Implement a scale function (map data range → pixel range) and draw marks.
4. Add axes and labels; ensure units are explicit.
5. Add an HTML table below the chart so values are available as text.
6. Reflect on why your encoding is appropriate and what could mislead.

## Acceptance Criteria (Module 5 Project)

- Correctness: Scale maps data to pixels consistently; axes/labels match values.
- Accessibility: Companion table lists values; chart has text description.
- Clarity: Units, titles, and legend (if needed) are present.
- Reflection: Explains encoding choice and limitations.

## Accessibility Checklist

- Table: Provide an HTML table with headers and caption near the chart.
- Text: Include a short description of what the chart shows.
- Colour: Do not rely on colour alone to differentiate.

## Differentiation & Extensions

- Scaffold: Starter Canvas/SVG code with drawing helpers.
- Extension: Add simple interactivity (hover value tooltip) or switch between datasets.

## Assessment & Evidence

- Use the visualization rubric (Teacher Toolkit) for clarity, correctness, and accessibility.
- Evidence: HTML/JS files, screenshot of chart, and reflection notes.

## Teacher Toolkit Links

- [Module overview](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/05-data-visualization/module-overview.md)
- Lesson plans:
  - [Unit 5.1 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/05-data-visualization/unit-5.1-lesson-plan.md)
- [Assessment rubric](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/05-data-visualization/assessment-rubric-05.md)

## Quick Open (macOS)

```zsh
open ./examples/canvas-bar-chart.html
```

## Try it

- Alter the `data` array in the example to see how the chart changes.
- Pair the chart with a small HTML table to improve accessibility.
