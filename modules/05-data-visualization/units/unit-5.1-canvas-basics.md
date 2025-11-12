# Module 5: Data & Visualization

## Unit 5.1 – Canvas Basics: Drawing a Simple Bar Chart

**Learning outcomes:**

- Student stores small datasets in arrays/objects.
- Student draws simple shapes on `<canvas>` using 2D context.
- Student maps data values to pixel heights with a linear scale.

**Teacher-notes:**

- Keep data inline (no external fetch) to focus on fundamentals.
- Show axes-free charts first; discuss labelling afterwards.
- Emphasise readability: colours, bar spacing, value labels.

**Classroom Task:**

- Visualise 5 data points (e.g., monthly recycling rates) as vertical bars.
- Add value labels above each bar; ensure contrast against background.

**Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Canvas Bar Chart</title>
    <style>
      body {
        font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
        margin: 1rem;
      }
      #wrap {
        max-width: 640px;
      }
    </style>
  </head>
  <body>
    <div id="wrap">
      <h1>Recycling Rates</h1>
      <canvas
        id="chart"
        width="600"
        height="360"
        aria-label="Bar chart"
      ></canvas>
    </div>
    <script>
      const data = [35, 48, 42, 55, 60]; // example values
      const labels = ["Jan", "Feb", "Mar", "Apr", "May"];

      const canvas = document.getElementById("chart");
      const ctx = canvas.getContext("2d");

      const padding = 40;
      const w = canvas.width - padding * 2;
      const h = canvas.height - padding * 2;
      const max = Math.max(...data) * 1.1;
      const barW = (w / data.length) * 0.7;
      const gap = (w / data.length) * 0.3;

      ctx.font = "14px system-ui";
      ctx.textAlign = "center";

      data.forEach((v, i) => {
        const x = padding + i * (barW + gap) + gap / 2;
        const y = padding + h - (v / max) * h;
        const barH = (v / max) * h;

        // bar
        ctx.fillStyle = "#60a5fa";
        ctx.fillRect(x, y, barW, barH);

        // value label
        ctx.fillStyle = "#111827";
        ctx.fillText(String(v), x + barW / 2, y - 8);

        // x label
        ctx.fillStyle = "#374151";
        ctx.fillText(labels[i], x + barW / 2, padding + h + 20);
      });
    </script>
  </body>
</html>
```

**Reflection prompt:**

- How did you convert data values into bar heights?
- What would you change to make this chart more accessible?
