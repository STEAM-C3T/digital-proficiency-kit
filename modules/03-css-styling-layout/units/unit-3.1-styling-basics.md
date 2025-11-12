# Module 3: CSS Styling & Layout

## Unit 3.1 – Styling Basics: Selectors, Colour, Typography, Box Model

**Learning outcomes:**

- Student applies CSS selectors (element, class, id) to style HTML.
- Student adjusts colour, font, spacing while maintaining accessible contrast.
- Student explains the CSS box model (content, padding, border, margin).

**Teacher-notes:**

- Start from a plain HTML page (from Module 2). Add a `<style>` block.
- Demonstrate element vs class vs id selectors and when to prefer classes.
- Use a contrast checker (or visual judgement) to ensure readable colours.

**Classroom Task:**

- Style a one-page "About me" document:
  - Set base font, size, and line-height.
  - Give headings distinct font-size/weight.
  - Add spacing with margin/padding.
  - Ensure links have clear hover/focus states.

**Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Styling Basics</title>
    <style>
      :root {
        --bg: #ffffff;
        --text: #1f2937; /* slate-800 */
        --accent: #0ea5e9; /* sky-500 */
      }
      html {
        box-sizing: border-box;
      }
      *,
      *::before,
      *::after {
        box-sizing: inherit;
      }
      body {
        margin: 0;
        font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
        color: var(--text);
        background: var(--bg);
        line-height: 1.6;
        padding: 1rem;
      }
      h1,
      h2,
      h3 {
        line-height: 1.25;
        margin: 0 0 0.5rem;
      }
      h1 {
        font-size: 2rem;
      }
      h2 {
        font-size: 1.5rem;
        margin-top: 1.25rem;
      }
      p {
        margin: 0 0 1rem;
      }
      a {
        color: var(--accent);
        text-decoration: underline;
      }
      a:focus,
      a:hover {
        outline: 2px solid var(--accent);
        outline-offset: 2px;
      }
      .card {
        border: 1px solid #e5e7eb; /* gray-200 */
        border-radius: 8px;
        padding: 1rem;
        max-width: 42rem;
        box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
      }
    </style>
  </head>
  <body>
    <main class="card">
      <h1>About Me</h1>
      <p>Short intro paragraph goes here.</p>
      <h2>Links</h2>
      <p>Visit my <a href="#">portfolio</a> or <a href="#">contact</a> page.</p>
    </main>
  </body>
</html>
```

**Reflection prompt:**

- Where did you use classes vs element selectors and why?
- How did you check visual contrast for text and links?
