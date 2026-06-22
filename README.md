# ELA Reading Performance Dashboard

An interactive React dashboard for visualizing K–5 English Language Arts diagnostic data. Built to help educators quickly identify trends in reading performance, track student growth, and surface students who may need intervention.

## Features

- **Overview tab** — School-wide summary with stat cards (median score, percentile, diagnostic gain, zero-growth alerts), a score distribution scatter plot by grade, and a growth-vs-typical bar chart by grade
- **Skills breakdown tab** — Radar charts comparing domain performance (phonics, high-frequency words, vocabulary, comprehension) across grades, plus a detailed classroom data table with per-student metrics
- **Filtering** — Filter by grade level (K–5 or All) to drill into specific cohorts
- **Interactive charts** — Hover tooltips on scatter plots and bar charts for individual student detail
- **ACAP projections** — Projected ACAP proficiency levels for grades 2+ with color-coded indicators

## Tech Stack

- [React](https://react.dev/) 19
- [Vite](https://vite.dev/) 8
- [Recharts](https://recharts.org/) — bar charts, scatter plots, radar charts
- [Google Fonts](https://fonts.google.com/) — DM Serif Display, IBM Plex Sans, IBM Plex Mono

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Production build
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
src/
├── ela_dashboard.jsx   # Main dashboard component with embedded student data
├── App.jsx             # App wrapper that renders the dashboard
├── main.jsx            # Vite entry point
└── index.css           # Google Fonts import and CSS reset
```

## Deployment

This project is configured for deployment on [Vercel](https://vercel.com). Connect the GitHub repo and Vercel will auto-detect Vite with these defaults:

- **Build command:** `npm run build`
- **Output directory:** `dist`
