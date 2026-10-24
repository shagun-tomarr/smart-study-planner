# Smart Study Planner: a beginner's guide

This app is made with regular HTML, CSS, and JavaScript. It does not need an
account or a server to keep your study plan.

## The three main parts

- `index.html` is the page's starting point. It provides an empty container for
  the app and loads the JavaScript file.
- `src/index.css` controls how the page looks, including its colors, spacing,
  and phone-sized layout.
- `src/main.js` builds the page, responds to button presses, and saves changes.

## How saving works

The app keeps two lists in JavaScript: study tasks and timetable blocks. When
you add, complete, or remove an item, the `persist()` function turns those lists
into text with `JSON.stringify()` and saves them in the browser's
`localStorage`. When the page opens, `readSaved()` loads that text again with
`JSON.parse()`. This is saved in this device and browser, not in an online
account.

## A few JavaScript ideas in this app

- A **variable** such as `tasks` holds information while the page is open.
- An **array** is a list. `tasks.map()` updates a task, and `tasks.filter()`
  keeps only the tasks you want.
- A **function** such as `render()` draws the page again after something changes.
- An **event listener** waits for an action such as submitting a form or pressing
  a button.
- `localStorage` remembers the lists when you close or refresh the page.

To learn by changing the app, try editing a heading in `src/main.js`, then
change a color near the top of `src/index.css`. Refresh the preview to see what
changed.
