# Module 2: HTML Foundations

## Unit 2.2 – Structuring for Access: Semantic Tags, Forms, Tables

**Learning outcomes:**

- Student uses semantic tags for structuring content.
- Student implements a basic HTML form to collect user input.
- Student creates a simple table to present data.
  **Teacher-notes:**
- Explain `<form>` elements: `<label>`, `<input>`, `<button>`, and the importance of `for` attribute linking label to input.
- Show table structure: `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<td>`, `<th>`.
  **Classroom Task:**
- Students design a “Student Survey” page: brief introduction, form with name, favourite STEAM subject, reason (textarea), submit button (does not need to send data).
- Below the form, present a table summarising hypothetical survey results of three students (columns: Name, Favourite Subject, Why).
  **Code Template:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Student Survey</title>
  </head>
  <body>
    <header>
      <h1>Student Survey – STEAM Subjects</h1>
    </header>
    <main>
      <section id="survey">
        <h2>Tell us about your favourite STEAM subject</h2>
        <form id="steamSurvey">
          <label for="stuName">Name:</label>
          <input type="text" id="stuName" name="stuName" required /><br /><br />
          <label for="favSubject">Favourite STEAM subject:</label>
          <input
            type="text"
            id="favSubject"
            name="favSubject"
            required
          /><br /><br />
          <label for="reason">Why do you like it?</label><br />
          <textarea id="reason" name="reason" rows="4" cols="40"></textarea
          ><br /><br />
          <button type="submit">Submit</button>
        </form>
      </section>
      <section id="results">
        <h2>Hypothetical Survey Results</h2>
        <table>
          <thead>
            <tr>
              <th>Name</th>
              <th>Favourite Subject</th>
              <th>Why</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Alice</td>
              <td>Physics</td>
              <td>Exploring how things move.</td>
            </tr>
            <tr>
              <td>Bob</td>
              <td>Art &amp; Design</td>
              <td>Combining creativity and tech.</td>
            </tr>
            <tr>
              <td>Charlie</td>
              <td>Biology</td>
              <td>Understanding life and data.</td>
            </tr>
          </tbody>
        </table>
      </section>
    </main>
    <footer>
      <p>© 2025 School Name</p>
    </footer>
  </body>
</html>
```

**Reflection prompt:**

- Why are `<label>` elements important in forms?
- How did you organise the table headers and content for clarity?
