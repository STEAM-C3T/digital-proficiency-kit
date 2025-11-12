# Module 1: Introduction to the Web

## Unit 1.2 – Basic Structure of a Web Page

**Learning outcomes:**

- Student constructs a simple HTML document with correct head/body structure.
- Student uses semantic tags (header, nav, main, footer) to organise content.
  **Teacher-notes:**
- Introduce semantic tags: `<header>`, `<nav>`, `<section>`, `<footer>`.
- Emphasise accessibility and readability for machines and humans.
  **Classroom Task:**
- Students build a one-page static site (e.g., “About me” page) with: header (name), nav (links to anchors on same page), two sections (hobbies, favourite subject), footer (contact info).
- They inspect how the page appears on tablet/mobile (resize browser).
  **Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>About Me</title>
  </head>
  <body>
    <header>
      <h1>Student Name</h1>
      <nav>
        <a href="#hobbies">Hobbies</a> |
        <a href="#subject">Favourite Subject</a>
      </nav>
    </header>
    <main>
      <section id="hobbies">
        <h2>Hobbies</h2>
        <p>List or describe your hobbies here.</p>
      </section>
      <section id="subject">
        <h2>Favourite Subject</h2>
        <p>Describe why you enjoy this subject.</p>
      </section>
    </main>
    <footer>
      <p>Contact: student@example.com</p>
    </footer>
  </body>
</html>
```

**Reflection prompt:**

- Why did you choose those tags (section, nav, footer) instead of just `<div>`?
- How might screen-readers or search engines use these semantic tags?
