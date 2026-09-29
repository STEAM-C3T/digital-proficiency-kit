# Module 5: Data & Visualization

Represent a small dataset as a labelled Canvas bar chart. Focus on mapping values to bar heights and making the chart understandable without relying on the visual alone. SVG and other chart types are optional extensions.

## Learning Outcomes

- Maps numeric data to visual encodings (length, position, colour) with clear labels.
- Explains scaling and axis choices for simple charts.
- Pairs visualizations with tables to support accessibility and verification.

## Prerequisites

- Modules 1–4 or equivalent HTML/CSS/JS basics.

## Estimated Time

- 2 lessons (about 90 minutes for the core chart and table); allow another 30–60 minutes for optional chart types or interaction.

## Materials

- Browser with Canvas support (modern browsers), text editor.

## Contents

- Units
  - [Unit 5.1 – Canvas Basics: Simple Bar Chart](./units/unit-5.1-canvas-basics.md) — Draw bars from an array of values; label clearly.
- Examples
  - [canvas-bar-chart.html](./examples/canvas-bar-chart.html) — CO₂ savings as a labelled bar chart.
- Tasks
  - [Task: Visualize a Small Dataset](./tasks/task-1-visualize-dataset.md) — Build a Canvas bar chart, add a companion table, and explain the scale.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Accessibility tips (pair with a table), extension ideas.

## How This Module Works

1. Learn Canvas basics via Unit 5.1 and the example bar chart.
2. Choose 4–8 data values with clear labels and units.
3. Implement a scale, draw bars, and label the chart clearly. Other chart forms are optional extensions.
4. Provide a companion HTML table for screen reader access.

## Your Route Through This Module

1. **Unit 5.1 — Turn data into a chart.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/tutorial/unit-5.1-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/workbook/unit-5.1-student-workbook.md). Start by changing one value in the [bar chart example](./examples/canvas-bar-chart.html). **Checkpoint:** explain how a larger value changes a bar's height.
2. **Practise with a small dataset.** Choose 4–8 values and identify their labels and units before drawing. Use the tutorial's scale example to map values to pixels.
3. **Make and check your chart.** Complete [Visualize a Small Dataset](./tasks/task-1-visualize-dataset.md). Add a title, readable labels, and a companion HTML table so the values are available as text.
4. **Reflect.** Explain why you chose this chart and name one way the scale or labels could affect how a reader interprets it.

**What to keep:** your HTML file, chart screenshot, companion table, and short reflection. Use a small local or invented dataset; external data is optional.

## Student Instructions (Step‑by‑Step)

1. Open `examples/canvas-bar-chart.html`; change the `data` array and observe the result.
2. Select a meaningful dataset (4–8 values) and describe what each value represents.
3. Implement a scale function (map data range → pixel range) and draw marks.
4. Add axes and labels; ensure units are explicit.
5. Add an HTML table below the chart so values are available as text.
6. Reflect on why your encoding is appropriate and what could mislead.

## Acceptance Criteria (Module 5 Project)

- Correctness: Scale maps each data value to bar height consistently; labels match values.
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

## Learning Materials

Comprehensive instructional materials for teachers and students are available in the [Learning Materials repository](https://github.com/STEAM-C3T/dpk-learning-materials/tree/main/modules/05-data-visualization):

- **[Module 05 Overview Deck](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/module-deck/module-05-deck.md):** Marp slides with learning outcomes, big ideas, demonstrations, and speaker notes
- **Unit 5.1 Materials:**
  - [Lesson deck](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/deck/unit-5.1-deck.md)
  - [Step-by-step tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/tutorial/unit-5.1-tutorial.md)
  - [Student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/workbook/unit-5.1-student-workbook.md)
  - [Teacher annotated workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/05-data-visualization/units/5.1-canvas-basics/workbook/unit-5.1-teacher-annotated.md) (with timing, differentiation, answer keys)

**For Teachers:** These materials are specifically designed for novice teachers with little or no programming experience, providing scaffolded lesson plans, common misconceptions, and classroom-ready slides.

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
