# Module 1: Introduction to the Web

## Unit 1.1 – What is the Web & How Does It Work?

**Learning outcomes:**

- Student describes basic components of a webpage (HTML, CSS, JavaScript).
- Student explains how a web browser requests and displays a web page.
  **Teacher-notes:**
- Begin with discussion: “What happens when you type a URL and hit Enter?”
- Use simple diagram: browser → server → response → browser render.
  **Classroom Task:**
- Task A: Students open their browser’s “View Source” for a simple webpage and identify `<html>`, `<head>`, `<body>` tags.
- Task B: In pairs, students draw a flow-diagram of request-response cycle between browser and server.
  **Code Template (minimal):**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Your First Webpage</title>
  </head>
  <body>
    <h1>Hello Web!</h1>
    <p>This is my first webpage.</p>
  </body>
</html>
```

**Reflection prompt:**

- What parts of the page change when you edit the `<title>` or `<h1>`?
- Why might the `<body>` tag matter for screen-readers or mobile devices?
