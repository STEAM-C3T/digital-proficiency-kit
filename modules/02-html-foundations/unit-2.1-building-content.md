# Module 2: HTML Foundations

## Unit 2.1 – Building Content: Headings, Paragraphs, Lists, Links, Images

**Learning outcomes:**

- Student creates content using headings (`<h1>`-`<h3>`), paragraphs, ordered/unordered lists, links and images.
- Student recognises when to use lists vs paragraphs vs headings for accessibility.
  **Teacher-notes:**
- Show example: difference between `<ul>`, `<ol>`, `<dl>`.
- Demonstrate how alt text for images improves accessibility.
  **Classroom Task:**
- Create a small webpage about a STEAM topic (e.g., “Climate Data”), include: heading, subheading, paragraph, unordered list of 3 key facts, image with alt text, link to a reliable external resource.
  **Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Climate Data Facts</title>
  </head>
  <body>
    <header>
      <h1>Climate Data Facts</h1>
    </header>
    <main>
      <h2>Key Facts</h2>
      <p>Here are some important facts about climate change:</p>
      <ul>
        <li>Fact 1 – description.</li>
        <li>Fact 2 – description.</li>
        <li>Fact 3 – description.</li>
      </ul>
      <figure>
        <img
          src="images/climate-chart.png"
          alt="Chart showing global temperature rise"
        />
        <figcaption>Global temperature rise since 1880.</figcaption>
      </figure>
      <p>
        Read more at
        <a href="https://www.ipcc.ch" target="_blank" rel="noopener"
          >IPCC Official Website</a
        >.
      </p>
    </main>
    <footer>
      <p>© 2025 Student Name</p>
    </footer>
  </body>
</html>
```

**Reflection prompt:**

- How did you decide which tag to use for each part of your page?
- What alt text did you provide for the image and why?
