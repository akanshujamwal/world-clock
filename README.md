# 🌍 World Clock Dashboard

A modern, feature-rich **World Clock Dashboard** built with **pure HTML, CSS, and JavaScript** — zero frameworks, zero libraries.

Designed for performance, usability, and clean frontend engineering.

---

## 🔗 Live Demo

👉 [akanshujamwal.github.io/world-clock](https://akanshujamwal.github.io/world-clock/)

---

## 📸 Preview

_Add screenshots here for better GitHub presentation._

---

## Overview

The dashboard displays:

- 🇮🇳 Live **Indian Local Time** with an animated analog clock
- 🌐 **Fully customizable global clocks** — add or remove as many as you need
- ⚡ **Real-time updates** every second using `setInterval`
- 🔍 **Searchable timezone selector** with keyboard navigation
- 🌗 **12H / 24H toggle** and **seconds visibility** toggle
- 📊 **UTC offset** and **IST difference** shown on every card
- ☀️🌙 **Day / Night detection** per timezone
- 📋 **Click to copy** any time to clipboard
- 📱 Fully responsive across all screen sizes

---

## Key Features

### 🕒 Local Time Hero (India)

- Live date & time in IST, updating every second
- Smooth **SVG analog clock** with hour, minute, and second hands
- UTC offset pill, day/night indicator, and detected local timezone
- Click the time to **copy it to clipboard** instantly

---

### 🌍 Global Time Cards (Fully Dynamic)

Default timezones:

| Card | Timezone |
|------|----------|
| 1 | Europe/London |
| 2 | America/New_York |
| 3 | Asia/Dubai |
| 4 | Asia/Tokyo |
| 5 | Australia/Sydney |

Each card shows:

- City name and region
- Live time and date (updates every second)
- UTC offset (e.g. `UTC+05:30`)
- Difference vs IST (e.g. `+5h 30m IST`, `-4h IST`)
- Day ☀️ or Night 🌙 indicator with colour-coded left border
- Click time to copy it to clipboard

**Cards are fully dynamic:**

- ➕ **Add** as many clocks as you need with the Add Clock button
- ✕ **Remove** any card with the hover-reveal remove button
- Timezone changes replace the card in place — no page reload

---

### 🔍 Searchable Timezone Selector

- Live search across 400+ IANA timezones as you type
- UTC offset displayed alongside each option in the list
- Full **keyboard navigation** — `↑ ↓` arrows to highlight, `Enter` to select, `Escape` to close
- ✕ clear button to reset the search input
- Dropdown closes automatically on outside click

---

### 🎛 Global Controls

| Control | Function |
|---------|----------|
| `12H / 24H` | Toggle 12-hour and 24-hour time formats for all clocks |
| `:SS` | Show or hide seconds across all clocks |
| `＋ Add Clock` | Append a new clock card with a random unused timezone |

---

### 🎨 Design System

- **Dark theme** with subtle blue-indigo radial gradients
- **Monospace font** (JetBrains Mono) for all time values — clean and legible
- **Syne** display font for headers — bold and distinctive
- Glassmorphism-style surfaces with `backdrop-filter: blur`
- Day/Night left-border accent: amber for day, blue for night
- Hover lift effect and smooth transitions on all interactive elements
- Custom minimal scrollbar on dropdowns

---

### ⚡ Performance

- Native **Intl.DateTimeFormat** API — no timezone library needed
- DOM updates are scoped to each card — minimal reflows
- All 400+ timezone options are rendered on-demand with search filtering (max 60 at a time)
- No external dependencies — instant load, no network requests after the font

---

## 🛠 Tech Stack

| Technology | Usage |
|-----------|-------|
| HTML5 | Structure and layout |
| CSS3 | Grid, animations, glassmorphism, transitions |
| JavaScript ES6+ | Timers, DOM, Intl API, clipboard |
| Intl.supportedValuesOf | Full timezone list |
| Intl.DateTimeFormat | Locale-aware time/date formatting |
| SVG | Analog clock rendering |
| Clipboard API | Copy-to-clipboard on click |

> **Zero frameworks. Zero libraries. Pure frontend engineering.**

---

## 📂 Project Structure

```
world-clock/
│
├── index.html      # Full dashboard — HTML, CSS, and JS in one file
└── README.md       # Documentation
```

Single-file architecture — easy to deploy anywhere, including GitHub Pages.

---

## 🎯 Concepts Demonstrated

- JavaScript `Date` and `Intl` APIs (timezone, locale formatting)
- Live DOM manipulation and real-time `setInterval` loops
- SVG drawing and animation with pure JavaScript
- Custom searchable dropdown with keyboard accessibility
- Responsive CSS Grid with `auto-fill` and `minmax`
- Clipboard API integration with user feedback (toast)
- Component-style card management (create, update, replace, remove)

---

## 🚀 Getting Started

No build step required.

```bash
git clone https://github.com/akanshujamwal/world-clock.git
cd world-clock
open index.html
```

Or deploy directly to **GitHub Pages**, **Netlify**, or **Vercel** — just push `index.html`.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push and open a Pull Request

For major changes, please open an issue first to discuss the approach.

---

## 📜 License

Released under the **MIT License** — free to use, modify, and distribute.

---

## 👨‍💻 Author

**Akanshu Jamwal**
Frontend Developer · Flutter · JavaScript · UI Engineering

---

## 🔮 Potential Enhancements

- 💾 Save card preferences in `localStorage`
- ⭐ Favourite / pin cities
- 🌗 Light mode theme
- 🔔 Alarm or reminder per timezone
- 🗺 World map with clock pins
- 📸 Add preview screenshots to this README
