# Module 4: JavaScript Essentials

## Unit 4.1 – JS Basics + DOM: Variables, Events, Manipulation

**Learning outcomes:**

- Student writes basic JS (variables, functions) and logs to console.
- Student selects DOM elements and updates text/attributes/styles.
- Student handles user events (click, input) to change the page state.

**Teacher-notes:**

- Keep JavaScript in a `<script>` tag at the end of `<body>` for simplicity.
- Demonstrate `document.querySelector`, `addEventListener`, and safe defaults.
- Emphasise not blocking UI; prefer unobtrusive JS (no inline `onclick`).

**Classroom Task:**

- Build a mini interactive profile card:
  - A text input to set a name; updates `<h2>` live.
  - A button to toggle a "dark mode" class on `<body>`.

**Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>JS Basics + DOM</title>
    <style>
      body {
        font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
        margin: 1rem;
      }
      .card {
        border: 1px solid #e5e7eb;
        border-radius: 8px;
        padding: 1rem;
        max-width: 32rem;
      }
      .dark {
        background: #0b1020;
        color: #e5e7eb;
      }
      .dark .card {
        border-color: #334155;
      }
    </style>
  </head>
  <body>
    <div class="card">
      <h2 id="name">Your Name</h2>
      <label for="nameInput">Set name:</label>
      <input id="nameInput" type="text" placeholder="Type your name" />
      <button id="toggleTheme">Toggle dark mode</button>
    </div>

    <script>
      const nameEl = document.querySelector("#name");
      const inputEl = document.querySelector("#nameInput");
      const toggleBtn = document.querySelector("#toggleTheme");

      inputEl.addEventListener("input", () => {
        nameEl.textContent = inputEl.value || "Your Name";
      });

      toggleBtn.addEventListener("click", () => {
        document.body.classList.toggle("dark");
      });
    </script>
  </body>
</html>
```

**Reflection prompt:**

- What events did you handle and why?
- How did you ensure the page still works with empty input?
