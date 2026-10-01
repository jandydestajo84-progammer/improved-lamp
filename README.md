# Hands-On Activity 2: Class Requirements To-Do List

**Objective:** Practice event handling, conditional rendering, and rendering lists with keys.
**Suggested time:** 60 minutes

## How to run
1. Open this folder in VS Code (**File → Open Folder…**).
2. Double-click `start.bat`, **or** open the terminal with **Ctrl + `** and run `npm install` then `npm run dev`.
3. The app opens at http://localhost:5173. Press **Ctrl + C** in the terminal to stop it.

> PowerShell error *"running scripts is disabled"*? Switch the VS Code terminal to **Command Prompt** (**˅** beside **+**).

## Your tasks
Search for `TODO` with **Ctrl + Shift + F**. Styling is already provided.

| # | Task | File |
|---|------|------|
| 1 | Store tasks in state as an array of `{ id, title, done }`. | `src/App.jsx` |
| 2 | Add a task with the input and **Add** button. Generate the id with `crypto.randomUUID()` or `Date.now()`. Ignore empty input. | `App.jsx`, `components/TaskForm.jsx` |
| 3 | Render the tasks with `map()` using `task.id` as the **key**. | `components/TaskList.jsx` |
| 4 | Clicking a task toggles `done`. Done tasks get a strike-through (conditional `className`). | `App.jsx`, `components/TaskItem.jsx` |
| 5 | Add a **Delete** button per task (use `filter()`). | `App.jsx`, `components/TaskItem.jsx` |
| 6 | Show **"No tasks yet!"** when the list is empty, otherwise **"X of Y completed"**. | `App.jsx` |
| Bonus | Filter buttons: All, Active, Completed. | `components/FilterBar.jsx`, `App.jsx` |

## Rubric (100 pts)
| Criterion | Points |
|---|---|
| Add, toggle, and delete work | 35 |
| Correct list rendering + keys (no index keys) | 25 |
| Conditional rendering | 25 |
| Readable code and UI | 15 |

## Submit
A screenshot showing **at least 5 tasks (some completed)** and your zipped `src` folder (no `node_modules`) or a GitHub link.
