# Module 3: CSS Styling & Layout

## Unit 3.2 – Layout & Responsive Design: Flexbox, Grid, Media Queries

**Learning outcomes:**

- Student uses Flexbox or CSS Grid to create multi-column layouts.
- Student applies media queries to adapt layout to small and large screens.
- Student ensures content remains readable and accessible at all sizes.

**Teacher-notes:**

- Encourage mobile-first CSS: start from narrow screens, scale up.
- Use Grid for page layout and Flexbox for components inside sections.
- Test with keyboard navigation; ensure focus styles remain visible.

**Classroom Task:**

- Core: build a card grid that changes from one to two columns at one breakpoint. Optional extension: add a second breakpoint for three columns or make the navigation responsive.

**Code Template (excerpt):**

```html
<header class="site-header">
  <h1>My Portfolio</h1>
  <nav class="site-nav">
    <a href="#work">Work</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>
<main class="grid">
  <article class="card">Project A</article>
  <article class="card">Project B</article>
  <article class="card">Project C</article>
</main>
```

```css
:root {
  --gap: 1rem;
}
body {
  margin: 0;
  font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
}
.site-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: var(--gap);
  border-bottom: 1px solid #e5e7eb;
}
.site-nav a {
  margin-left: 0.75rem;
}
.grid {
  display: grid;
  gap: var(--gap);
  padding: var(--gap);
  grid-template-columns: 1fr;
}
.card {
  border: 1px solid #e5e7eb;
  border-radius: 8px;
  padding: var(--gap);
}
/* Core breakpoint: widen the grid from one to two columns. */
@media (min-width: 640px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
/* Optional extension: add a second breakpoint for three columns. */
@media (min-width: 1024px) {
  .grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

**Reflection prompt:**

- Which core breakpoint did you choose and why? If you tried the optional second breakpoint, what does it improve?
- Where did Grid make sense vs Flexbox?
