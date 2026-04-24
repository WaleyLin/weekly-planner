# Weekly Planner

A personal weekly planner built with vanilla HTML, CSS, and JavaScript. Designed for tracking work schedules, gym routines, and daily tasks — all saved locally in the browser with no backend required.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## Features

- **4-week calendar view** — navigate forward and backward through weeks with smooth transitions
- **Edit / View mode** — toggle between viewing your schedule and editing it
- **Per-day tracking** — log locations and shift times for two people, plus a gym workout type
- **Task management** — add, delete, and drag tasks between days
- **Action items panel** — a global checklist with drag-to-reorder and completion tracking
- **Copy Week** — pick any week and copy its shifts to another week
- **Clear Weeks** — clear one or multiple weeks at once, or wipe everything from a certain week forward
- **Export to PNG** — export 1–4 weeks as a clean image with day headers and week labels
- **Live weather widget** — pulls real-time weather for Mesa, AZ via Open-Meteo (no API key needed)
- **Live clock** — updates every second in the top bar
- **Persistent storage** — all data saved to `localStorage`, survives page refreshes and browser restarts
- **Task indicator** — date numbers glow when a day has tasks

---

## Built With

| Technology | Usage |
|---|---|
| HTML5 | Structure and layout |
| CSS3 | Styling, CSS variables, animations, grid layout |
| Vanilla JavaScript | All interactivity, data management, DOM manipulation |
| localStorage API | Persistent client-side data storage |
| html2canvas | PNG export of the calendar |
| Open-Meteo API | Free weather data, no API key required |
| Google Fonts | DM Sans + JetBrains Mono typography |

---

## How to Use

1. Clone or download the repo
2. Open `index.html` in any modern browser — no build step, no dependencies to install
3. Use **Edit mode** to fill in your schedule
4. Navigate weeks with the `←` and `→` buttons
5. Access **Copy Week**, **Clear Week**, and **Export** from the `···` menu

---

## Project Structure

```
planner/
├── index.html      # Entire app — HTML, CSS, and JS in one file
└── README.md
```

Everything lives in a single `index.html` file. Styles are written in a `<style>` block using CSS custom properties for theming, and all logic is handled in a `<script>` block at the bottom with no frameworks or build tools.

---

## What I Learned

- Structuring a full single-page app in plain HTML/CSS/JS without any framework
- Using CSS Grid for dynamic calendar layouts
- Managing application state with `localStorage`
- Implementing drag-and-drop natively with the HTML5 Drag and Drop API
- Working with external APIs (weather) using `fetch` and async/await
- Building reusable modal patterns and dropdown menus from scratch
- Capturing and exporting DOM elements as images with html2canvas
