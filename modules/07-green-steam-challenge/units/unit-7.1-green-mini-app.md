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

- Build a "Green Actions Tracker": users tick daily actions and see a count of selected actions.
- Offer optional local persistence; the activity must still work when storage is unavailable.
- Explain how Reset removes saved choices and why the count is not a measurement of environmental impact.

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
      <p>Actions selected: <span id="score" class="score">0</span></p>
      <label><input id="remember" type="checkbox" /> Remember choices on this device</label>
      <p id="status" role="status" aria-live="polite">Choices stay for this session unless you opt in to saving them.</p>
      <button id="reset" type="button">Reset choices and saved data</button>
      <p>This count tracks selected activities; it does not measure environmental impact.</p>
    </div>

    <script>
      const KEY = "green-actions-v1";
      const list = document.querySelectorAll('#actions input[type="checkbox"]');
      const scoreEl = document.getElementById("score");
      const rememberToggle = document.getElementById("remember");
      const status = document.getElementById("status");

      function loadSavedChoices() {
        try {
          const saved = localStorage.getItem(KEY);
          return { available: true, state: saved === null ? null : JSON.parse(saved) };
        } catch {
          return { available: false, state: null };
        }
      }
      function saveChoices(state) {
        try {
          localStorage.setItem(KEY, JSON.stringify(state));
          return true;
        } catch {
          return false;
        }
      }

      function update() {
        const state = {};
        let selectedCount = 0;
        list.forEach((cb) => {
          state[cb.value] = cb.checked;
          if (cb.checked) selectedCount++;
        });
        scoreEl.textContent = selectedCount;
        if (rememberToggle.checked && !saveChoices(state)) {
          rememberToggle.checked = false;
          status.textContent = "Browser storage is unavailable. Choices will remain only for this session.";
        }
      }

      function reset() {
        list.forEach((cb) => (cb.checked = false));
        scoreEl.textContent = "0";
        rememberToggle.checked = false;
        try {
          localStorage.removeItem(KEY);
          status.textContent = "Choices and saved data have been cleared.";
        } catch {
          status.textContent = "Choices are cleared on this page, but browser storage would not allow saved data to be removed.";
        }
      }

      function rememberChoices() {
        if (!rememberToggle.checked) {
          try {
            localStorage.removeItem(KEY);
            status.textContent = "Saved choices removed. Choices now stay only for this session.";
          } catch {
            status.textContent = "Could not remove saved data because browser storage is unavailable.";
          }
          return;
        }
        const state = loadSavedChoices();
        if (!state.available) {
          rememberToggle.checked = false;
          status.textContent = "Browser storage is unavailable. Choices will remain only for this session.";
          return;
        }
        if (state.state) {
          list.forEach((cb) => {
            cb.checked = Boolean(state.state[cb.value]);
          });
        }
        status.textContent = "Choices are saved in this browser on this device. Use Reset to clear them.";
        update();
      }

      list.forEach((cb) => {
        cb.addEventListener("change", update);
      });
      rememberToggle.addEventListener("change", rememberChoices);
      document.getElementById("reset").addEventListener("click", reset);
      scoreEl.textContent = "0";
    </script>
  </body>
</html>
```

**Reflection prompt:**

- Who is your app for and what problem does it help with?
- What feedback did you receive and how will you iterate?

The example’s count is an activity count, not a measurement of environmental impact. Saving choices is optional; if you implement persistence, keep the app usable when browser storage is unavailable and explain how Reset removes saved data.
