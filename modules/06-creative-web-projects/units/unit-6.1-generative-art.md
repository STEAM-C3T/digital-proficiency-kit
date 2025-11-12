# Module 6: Creative Web Projects

## Unit 6.1 – Generative Art with HTML/CSS/JS

**Learning outcomes:**

- Student combines CSS and JS to create a simple generative visual.
- Student iterates on parameters (colour, size, randomness) to explore design.
- Student reflects on creative process and code decisions.

**Teacher-notes:**

- Encourage playful exploration: small changes, quick iterations.
- Discuss deterministic vs random outputs; seed values for repeatability.
- Promote accessibility: provide a text caption describing the piece.

**Classroom Task:**

- Create an animated pattern (dots, lines, or shapes) that changes over time.
- Expose 2–3 controls (sliders or inputs) to tweak the artwork.

**Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Generative Dots</title>
    <style>
      body {
        margin: 0;
        background: #0b1020;
        color: #e5e7eb;
        font-family: system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
      }
      #ui {
        position: fixed;
        top: 0.5rem;
        left: 0.5rem;
        background: rgba(255, 255, 255, 0.08);
        padding: 0.5rem 0.75rem;
        border-radius: 8px;
      }
      label {
        display: inline-block;
        margin-right: 0.5rem;
      }
    </style>
  </head>
  <body>
    <div id="ui">
      <label
        >Count <input id="count" type="range" min="50" max="500" value="150"
      /></label>
      <label
        >Size <input id="size" type="range" min="2" max="12" value="5"
      /></label>
    </div>
    <canvas id="c"></canvas>
    <script>
      const canvas = document.getElementById("c");
      const ctx = canvas.getContext("2d");
      const countEl = document.getElementById("count");
      const sizeEl = document.getElementById("size");

      function resize() {
        canvas.width = innerWidth;
        canvas.height = innerHeight;
      }
      addEventListener("resize", resize);
      resize();

      function rand(n) {
        return Math.random() * n;
      }

      function draw() {
        const count = Number(countEl.value);
        const size = Number(sizeEl.value);
        ctx.clearRect(0, 0, canvas.width, canvas.height);
        for (let i = 0; i < count; i++) {
          const x = rand(canvas.width);
          const y = rand(canvas.height);
          const hue = Math.floor(rand(360));
          ctx.fillStyle = `hsl(${hue} 80% 60% / 0.5)`;
          ctx.beginPath();
          ctx.arc(x, y, size, 0, Math.PI * 2);
          ctx.fill();
        }
        requestAnimationFrame(draw);
      }
      draw();
    </script>
  </body>
</html>
```

**Reflection prompt:**

- Which parameters did you expose and why?
- How would you describe the visual outcome to someone who can’t see it?
