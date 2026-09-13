# Airpods Animation

An animated product carousel for Airpods built with pure HTML, CSS, and vanilla JavaScript. Products slide through a 3D-style depth-tracking layout, and each item expands into a detailed spec/checkout view.

## Features

- **Animated carousel** – 6 Airpod slides with smooth depth/blur transitions between positions (prev/next navigation).
- **Detail view** – "See More" expands the active slide into a full product view with specifications and checkout buttons.
- **Rapid-click protection** – next/prev controls are temporarily disabled during transitions to keep the animation clean.
- **Responsive layout** – dedicated breakpoints for tablets (`max-width: 991px`) and mobile (`max-width: 767px`).
- **No dependencies** – runs entirely in the browser with no build step, frameworks, or package installs.

## Technologies

- HTML5
- CSS3 (custom properties / CSS variables, keyframe animations, flexbox, media queries)
- Vanilla JavaScript (DOM manipulation, `setTimeout` transition locking)
- Google Fonts – Poppins (loaded via CSS `@import`; requires internet access)

## Project Structure

```
├── index.html    # Page markup and carousel slides
├── style.css     # Layout, animations, responsive breakpoints
├── script.js     # Carousel navigation and detail-view logic
├── images/       # Product images (img1.png ... img6.png)
└── README.md
```

## Setup / Installation

No installation is required. The project is a static website with no external dependencies other than the Google Fonts stylesheet.

Requirements:

- A modern web browser (Chrome, Edge, Firefox, Safari).

## How to Run

You can open `index.html` directly in a browser by double-clicking it, or serve the folder locally:

**Option 1 – Open directly**

1. Open `index.html` in your browser.

**Option 2 – Local server (recommended)**

With any simple static server from the project root, e.g. Python:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

Or with Node:

```bash
npx serve .
```

## Usage

- Press the **`<`** and **`>`** buttons to move between products.
- Press **SEE MORE ↗** on the active slide to expand its detail view.
- Press **SEE ALL ↗** in the center to collapse back to the carousel.