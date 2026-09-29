# Module 2: HTML Foundations

Build well‑structured, accessible content using semantic HTML. Learn headings, lists, links, images, forms, and tables.

**Start here:** Check the prerequisites below, then begin with the [Unit 2.1 tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/02-html-foundations/units/2.1-building-content/tutorial/unit-2.1-tutorial.md). Follow the numbered route on this page and return here after using materials on the Learning Materials site.

## Learning Outcomes

- Structures content with appropriate semantic elements (sections, lists, figures, forms, tables).
- Writes accessible markup: associated labels, alt text, table headers, and captions.
- Evaluates a page for semantic correctness and basic accessibility concerns.

## Prerequisites

- Module 1 or equivalent familiarity with basic HTML structure.

## Estimated Time

- 2–3 lessons (90–135 minutes) based on practice time.

## Materials

- Modern browser and text editor; optional screen reader for testing (macOS VoiceOver, NVDA, etc.).

## Contents

- Units
  - [Unit 2.1 – Building Content](./units/unit-2.1-building-content.md) — Headings, paragraphs, lists, links, and images.
  - [Unit 2.2 – Structuring for Access](./units/unit-2.2-structuring-for-access.md) — Semantic tags, forms, and tables.
- Examples
  - [student-survey.html](./examples/student-survey.html) — A simple page with a form and a data table.
- Tasks
  - [Task: Build a Content Page](./tasks/task-1-content-page.md) — Create a small topic page with alt text and clear structure.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Guidance on semantics, accessibility, and assessment.

## How This Module Works

1. Deepen semantics (Unit 2.1) and structure for access (Unit 2.2).
2. Explore `examples/student-survey.html` and examine forms and tables.
3. Complete the guided then independent tasks.
4. Validate your page structure and form accessibility.

## Your Route Through This Module

1. **Unit 2.1 — Build clear content.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/02-html-foundations/units/2.1-building-content/tutorial/unit-2.1-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/02-html-foundations/units/2.1-building-content/workbook/unit-2.1-student-workbook.md), then return to this page. **Checkpoint:** your topic page has a meaningful heading structure, paragraphs, a list, a descriptive link, and an image with appropriate alt text.
2. **Practise Unit 2.1.** Complete [Build a Content Page](./tasks/task-1-content-page.md). Save the page; you will extend it after Unit 2.2.
3. **Unit 2.2 — Structure a form and data table.** Work through the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/02-html-foundations/units/2.2-structuring-for-access/tutorial/unit-2.2-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/02-html-foundations/units/2.2-structuring-for-access/workbook/unit-2.2-student-workbook.md), then return here. Use [student-survey.html](./examples/student-survey.html) as a reference. **Checkpoint:** every form control has a visible label, and the table has headers that describe its columns.
4. **Apply both units.** Complete [Build an Accessible Survey Page](./tasks/task-2-accessible-survey.md). Use fictional data only; this static practice page does not collect or store responses.
5. **Review and reflect.** Test the page in a browser, move through the controls with Tab, and write one sentence about how labels or table headers help a visitor.

**What to keep:** your content page, survey page, and short reflection. A screen reader is optional; the keyboard and browser checks are enough to complete the tasks.

### Module 2 progress check

- [ ] My content page has a clear structure, descriptive links, and useful image text.
- [ ] My form controls have visible, associated labels and my table has headers.
- [ ] I checked the page with a browser and keyboard navigation.
- [ ] I saved both pages and wrote a short reflection.

**Next:** continue to [Module 3: CSS Styling & Layout](../03-css-styling-layout/README.md), or [return to the student module list](../).

## Student Instructions (Step‑by‑Step)

1. Read Unit 2.1 and add headings, paragraphs, lists, links, and images for your topic.
2. Add a small form (e.g., feedback or survey) with `label` elements associated to each `input` via `for`/`id`.
3. Add a simple data table (2–3 columns) with `th` headers and an optional `caption`.
4. Use the inspector and, if available, a screen reader to verify the reading order and label associations.
5. Complete the reflection prompts in the task file.

## Acceptance Criteria (Module 2 Project)

- Semantics: Correct use of headings, lists, links, figures/images with `alt`.
- Forms: Every input has a programmatically associated label; submit button present.
- Tables: Uses `th` for headers; includes `caption` for clarity when appropriate.
- Accessibility: Logical tab order; descriptive link text.
- Reflection: Explains choices and areas for improvement.

## Accessibility Checklist

- Labels: Inputs have associated labels; placeholder is not the label.
- Alt text: Non‑decorative images have clear `alt` text.
- Tables: Provide headers and a caption; avoid layout tables.
- Headings: Follow a clear, hierarchical structure.

## Differentiation & Extensions

- Scaffold: Provide a partially built form/table template to complete.
- Extension: Add `fieldset`/`legend` groups, required field indicators, and validation hints.

## Assessment & Evidence

- Use the module rubric (Teacher Toolkit) to assess semantics, accessibility, and clarity.
- Evidence: HTML files with form and table components; reflection notes.

## Teacher Toolkit Links

- [Module overview](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/02-html-foundations/module-overview.md)
- Lesson plans:
  - [Unit 2.1 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/02-html-foundations/unit-2.1-lesson-plan.md)
  - [Unit 2.2 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/02-html-foundations/unit-2.2-lesson-plan.md)
- [Assessment rubric](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/02-html-foundations/assessment-rubric-02.md)

## Quick Open (macOS)

```zsh
open ./examples/student-survey.html
```

## Try it

- Open the example in your browser, then extend it with more form fields or a table.
- Validate the structure: headings in order, labels associated to inputs, alt text present.
