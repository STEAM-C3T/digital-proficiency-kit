# Module 7: Green STEAM Challenge

## Unit 7.1 – Build a Sustainability Mini‑App

**Learning outcomes:**

- Student scopes a small web app addressing an SDG‑related question.
- Student integrates HTML, CSS, and JS for a functional prototype.
- Student collects feedback and plans improvements.

**Teacher-notes:**

- Encourage concrete, local problems (e.g., school energy saving, recycling).
- Keep scope small: 1–2 screens, a clear interaction, and meaningful output.
- Plan–Build–Test cycle; capture feedback from at least one peer.

**Classroom Task:**

- Build a "Green Actions Tracker": users tick daily actions and see a simple score.
- Persist state locally so progress remains on refresh (localStorage).

**Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Green Actions Tracker</title>
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
      .score {
        font-weight: 700;
      }
    </style>
  </head>
  <body>
    <div class="card">
      <h1>Green Actions</h1>
      <ul id="actions">
        <li>
          <label
            ><input type="checkbox" value="cycle" /> Cycled or walked</label
          >
        </li>
        <li>
          <label
            ><input type="checkbox" value="recycle" /> Recycled waste</label
          >
        </li>
        <li>
          <label><input type="checkbox" value="water" /> Saved water</label>
        </li>
      </ul>
      <p>Score: <span id="score" class="score">0</span></p>
    </div>

    <script>
      const KEY = "green-actions-v1";
      const list = document.querySelectorAll('#actions input[type="checkbox"]');
      const scoreEl = document.getElementById("score");

      function load() {
        try {
          return JSON.parse(localStorage.getItem(KEY)) || {};
        } catch {
          return {};
        }
      }
      function save(state) {
        localStorage.setItem(KEY, JSON.stringify(state));
      }

      function update() {
        const state = {};
        let score = 0;
        list.forEach((cb) => {
          state[cb.value] = cb.checked;
          if (cb.checked) score++;
        });
        scoreEl.textContent = score;
        save(state);
      }

      // init
      const state = load();
      list.forEach((cb) => {
        cb.checked = !!state[cb.value];
        cb.addEventListener("change", update);
      });
      update();
    </script>
  </body>
</html>
```

**Reflection prompt:**

- Who is your app for and what problem does it help with?
- What feedback did you receive and how will you iterate?
