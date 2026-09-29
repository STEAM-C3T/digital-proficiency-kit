# Module 7: Green STEAM Challenge

Apply your skills to build a small sustainability‑focused web app linked to SDG themes. Keep scope small and impactful.

## Learning Outcomes

- Plans and implements a small purpose‑driven web app with clear user flows.
- Makes persistence optional, handles storage limitations, and explains how to reset saved data.
- Communicates sustainability activity counts and impact claims accurately, with limitations.

## Prerequisites

- Modules 1–4 required; 5–6 helpful depending on idea.

## Estimated Time

- 2–4 lessons (90–180 minutes) for planning, build, and sharing.

## Materials

- Browser and text editor; optional open datasets (CSV/JSON) if applicable.

## Contents

- Units
  - [Unit 7.1 – Build a Sustainability Mini‑App](./units/unit-7.1-green-mini-app.md) — Plan–build–test a simple app; persistence is optional.
- Examples
  - [green-mini-app.html](./examples/green-mini-app.html) — Track selected green actions with optional, resettable local storage.
- Tasks
  - [Task: SDG Mini‑App](./tasks/task-1-sdg-mini-app.md) — Design and explain a small app that supports awareness or behaviour change.
- Teacher notes
  - [Notes](./teacher-notes/notes.md) — Ethics, privacy, and assessment guidance.

## How This Module Works

1. Choose an SDG‑aligned theme and define a very small, specific user goal.
2. Prototype the UI (paper or HTML) and list core interactions.
3. Build the core flow; add simple persistence if appropriate.
4. Test with a peer, refine copy and accessibility, and present impact.

## Your Route Through This Module

1. **Unit 7.1 — Choose a focused sustainability question.** Follow the [tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/tutorial/unit-7.1-tutorial.md) and [student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/workbook/unit-7.1-student-workbook.md). Start with one user, one need, and one interaction. **Checkpoint:** explain who the app helps and what the user can do.
2. **Plan before coding.** Sketch the screen and write down the input, action, and feedback. Use the [green mini-app example](./examples/green-mini-app.html) to explore how a small interaction works.
3. **Build the core version.** Complete [SDG Mini-App](./tasks/task-1-sdg-mini-app.md). Make sure it works in the current session before considering optional storage.
4. **Test and improve.** Ask a peer to try the app, then make one improvement. If you add saving, explain what is stored and how to reset it. Never use real personal or sensitive data in a classroom prototype.
5. **Present and reflect.** Show the problem, the interaction, and what you changed. Explain what your app's counts or outputs do—and do not—measure.

**What to keep:** your HTML file, a short demo or screenshot, peer feedback, and the 100–150 word write-up. Presentation and reflection are part of this project, not a separate unit.

## Student Instructions (Step‑by‑Step)

1. Pick a focus (e.g., tracking green actions, comparing CO₂ of choices, or a tips library).
2. Outline the core flow (add/view/update) and sketch screens.
3. Build a minimal interface with semantic HTML; add JS for interactions.
4. If using `localStorage`, make it optional, explain what is stored, handle storage errors, and explain how Reset removes saved data.
5. Add simple activity counts and explain what they do and do not measure.
6. Prepare a short demo highlighting the problem, solution, and impact.

## Acceptance Criteria (Module 7 Project)

- Purpose: Clear, SDG‑aligned goal and simple user flow.
- Functionality: Core interactions work; persistence (if used) is explained.
- Accessibility: Keyboard operable; clear text labels; contrast meets basics.
- Ethics/Privacy: Discloses stored data and offers a reset.
- Communication: Explains impact and limitations honestly.

## Accessibility Checklist

- Operability: All controls reachable via keyboard; visible focus.
- Text: Clear language; avoid jargon; headings structure content.
- Data: If data is shown, provide textual summaries or tables.

## Differentiation & Extensions

- Scaffold: Provide a starter mini‑app skeleton with sections and placeholder handlers.
- Extension: Import a small open dataset; add filtering and basic visualization.

## Assessment & Evidence

- Use the project rubric (Teacher Toolkit) for purpose, usability, and ethics.
- Evidence: HTML/JS files, demo notes, and reflection on impact.

## Learning Materials

Comprehensive instructional materials for teachers and students are available in the [Learning Materials repository](https://github.com/STEAM-C3T/dpk-learning-materials/tree/main/modules/07-green-steam-challenge):

- **[Module 07 Overview Deck](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/module-deck/module-07-deck.md):** Marp slides with learning outcomes, big ideas, demonstrations, and speaker notes
- **Unit 7.1 Materials:**
  - [Lesson deck](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/deck/unit-7.1-deck.md)
  - [Step-by-step tutorial](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/tutorial/unit-7.1-tutorial.md)
  - [Student workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/workbook/unit-7.1-student-workbook.md)
  - [Teacher annotated workbook](https://github.com/STEAM-C3T/dpk-learning-materials/blob/main/modules/07-green-steam-challenge/units/7.1-green-mini-app/workbook/unit-7.1-teacher-annotated.md) (with timing, differentiation, answer keys)

**For Teachers:** These materials are specifically designed for novice teachers with little or no programming experience, providing scaffolded lesson plans, common misconceptions, and classroom-ready slides.

## Teacher Toolkit Links

- [Module overview](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/07-green-steAM-challenge/module-overview.md)
- Lesson plans:
  - [Unit 7.1 – Lesson plan](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/07-green-steAM-challenge/unit-7.1-lesson-plan.md)
- [Assessment rubric](https://github.com/STEAM-C3T/teacher-toolkit/blob/main/modules/07-green-steAM-challenge/assessment-rubric-07.md)

## Quick Open (macOS)

```zsh
open ./examples/green-mini-app.html
```

## Try it

- Open the example, tick actions, and observe the selected-action count.
- Opt in to saving choices, refresh the page, then use Reset to clear saved data.
- Discuss why the count is not a measurement of environmental impact.
