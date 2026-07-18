<div align="center">

<img src="./assets/banner.png" alt="EmployeeOS banner" width="100%" />

# EmployeeOS
### Employee Profile Generator & Analytics Dashboard

A single-file HR dashboard for managing employee profiles, auto-generating employee IDs, and visualizing workforce analytics — built with plain HTML, CSS, and JavaScript. No installs, no build step, no backend.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-38bdf8?style=flat-square)](./LICENSE)
[![Dependencies: none](https://img.shields.io/badge/Dependencies-None-22d3a5?style=flat-square)](#)

</div>

---

## What it does

Open `index.html` in a browser and you get a full HR dashboard:

- 🧑‍💼 **Manage employees** — add, edit, delete, and view detailed profiles
- 🆔 **Auto-generated employee codes** — e.g. `DEV-2026-JD-001`, built from department, year, and initials
- 🤖 **Auto-written profile summaries** for each employee
- 🔍 **Instant search & filters** by name, department, or status
- 📊 **Analytics view** — salary by department, experience distribution, headcount and diversity charts
- 📄 **Export to PDF** via the browser's print dialog
- 📱 **Responsive** — works on desktop and mobile

## Preview

<div align="center">

<img src="./assets/screenshot-dashboard.png" alt="Dashboard preview" width="100%" />

<br/><br/>

<img src="./assets/screenshot-analytics.png" alt="Analytics preview" width="100%" />

</div>

## Getting started

**1. Get the files**
```bash
git clone https://github.com/<codewithrahul18>/employee-profile-generator.git
cd employee-profile-generator
```

**2. Open it**

Just double-click `index.html` — or, for the most reliable experience, serve it locally:
```bash
python3 -m http.server 8000
```
then open `http://localhost:8000` in your browser.

That's it. No `npm install`, no build step, nothing else to configure.

## Project files

```
employee-profile-generator/
├── index.html      ← the entire app (markup + styles + logic)
├── assets/         ← images used in this README
├── LICENSE         ← MIT
└── README.md       ← this file
```

> ⚠️ **Important:** all four items above need to be in your GitHub repo together. If you only add `README.md` by itself, the preview images above won't load — GitHub needs the `assets/` folder to sit right next to `README.md` to find them, and needs `index.html` present for the app itself to work.

## How it works

State lives in one in-memory list of employees. Any action — search, filter, add, edit, delete — updates that state and re-renders whichever view (Dashboard, Employees, or Analytics) is currently active.

```
User action  →  update state  →  re-render current view  →  update the page
(search, add,    (employees list,   (Dashboard / Employees /
 edit, delete)    filters, etc.)     Analytics)
```

## Built with

Just the basics — no frameworks, no libraries, no CDN calls:
- **HTML5** for structure
- **CSS3** (custom properties, gradients, responsive grid) for styling
- **Vanilla JavaScript** for all app logic, plus the Canvas API for the background animation and inline SVG for the charts

## Customizing the starting data

Sample employees live in the `employees` array near the top of the `<script>` section in `index.html`. Edit that array to change what loads by default, or just use the **+ Add Employee** button once the app is open.

```js
let employees = [
  { id: 'DEV-2026-JD-001', firstName: 'John', lastName: 'Doe', dept: 'DEV', position: 'Data Analyst', salary: 75000 /* ... */ }
];
```

Note: since there's no backend or database, any changes you make while using the app reset when you reload the page — that's expected, not a bug.

## Ideas for extending it

- [ ] Save data with `localStorage` so it persists across reloads
- [ ] Export employee lists to CSV
- [ ] Add a light theme toggle
- [ ] Add simple login / access control

## Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes and open a Pull Request

## License

[MIT](./LICENSE) — free to use, modify, and share.

---

<div align="center"><sub>Built with plain HTML, CSS & JavaScript.</sub></div>
<div align="center">

<img src="./assets/banner.png" alt="EmployeeOS banner" width="100%" />

# EmployeeOS
### Employee Profile Generator & Analytics Dashboard

A single-file HR dashboard for managing employee profiles, auto-generating employee IDs, and visualizing workforce analytics — built with plain HTML, CSS, and JavaScript. No installs, no build step, no backend.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-38bdf8?style=flat-square)](./LICENSE)
[![Dependencies: none](https://img.shields.io/badge/Dependencies-None-22d3a5?style=flat-square)](#)

</div>

---

## What it does

Open `index.html` in a browser and you get a full HR dashboard:

- 🧑‍💼 **Manage employees** — add, edit, delete, and view detailed profiles
- 🆔 **Auto-generated employee codes** — e.g. `DEV-2026-JD-001`, built from department, year, and initials
- 🤖 **Auto-written profile summaries** for each employee
- 🔍 **Instant search & filters** by name, department, or status
- 📊 **Analytics view** — salary by department, experience distribution, headcount and diversity charts
- 📄 **Export to PDF** via the browser's print dialog
- 📱 **Responsive** — works on desktop and mobile

## Preview

<div align="center">

<img src="./assets/screenshot-dashboard.png" alt="Dashboard preview" width="100%" />

<br/><br/>

<img src="./assets/screenshot-analytics.png" alt="Analytics preview" width="100%" />

</div>

## Getting started

**1. Get the files**
```bash
git clone https://github.com/<codewithrahul18>/employee-profile-generator.git
cd employee-profile-generator
```

**2. Open it**

Just double-click `index.html` — or, for the most reliable experience, serve it locally:
```bash
python3 -m http.server 8000
```
then open `http://localhost:8000` in your browser.

That's it. No `npm install`, no build step, nothing else to configure.

## Project files

```
employee-profile-generator/
├── index.html      ← the entire app (markup + styles + logic)
├── assets/         ← images used in this README
├── LICENSE         ← MIT
└── README.md       ← this file
```

> ⚠️ **Important:** all four items above need to be in your GitHub repo together. If you only add `README.md` by itself, the preview images above won't load — GitHub needs the `assets/` folder to sit right next to `README.md` to find them, and needs `index.html` present for the app itself to work.

## How it works

State lives in one in-memory list of employees. Any action — search, filter, add, edit, delete — updates that state and re-renders whichever view (Dashboard, Employees, or Analytics) is currently active.

```
User action  →  update state  →  re-render current view  →  update the page
(search, add,    (employees list,   (Dashboard / Employees /
 edit, delete)    filters, etc.)     Analytics)
```

## Built with

Just the basics — no frameworks, no libraries, no CDN calls:
- **HTML5** for structure
- **CSS3** (custom properties, gradients, responsive grid) for styling
- **Vanilla JavaScript** for all app logic, plus the Canvas API for the background animation and inline SVG for the charts

## Customizing the starting data

Sample employees live in the `employees` array near the top of the `<script>` section in `index.html`. Edit that array to change what loads by default, or just use the **+ Add Employee** button once the app is open.

```js
let employees = [
  { id: 'DEV-2026-JD-001', firstName: 'John', lastName: 'Doe', dept: 'DEV', position: 'Data Analyst', salary: 75000 /* ... */ }
];
```

Note: since there's no backend or database, any changes you make while using the app reset when you reload the page — that's expected, not a bug.

## Ideas for extending it

- [ ] Save data with `localStorage` so it persists across reloads
- [ ] Export employee lists to CSV
- [ ] Add a light theme toggle
- [ ] Add simple login / access control

## Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes and open a Pull Request

## License

[MIT](./LICENSE) — free to use, modify, and share.

---

<div align="center"><sub>Built with plain HTML, CSS & JavaScript.</sub></div>




