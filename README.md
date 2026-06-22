# ELA Reading Performance Dashboard

An interactive React dashboard for visualizing K–5 English Language Arts diagnostic data. Built to help educators quickly identify trends in reading performance, track student growth, and surface students who may need intervention.

## Features

- **Time point navigation** — Toggle between Fall (BOY), Winter (MOY), and Spring (EOY) to compare performance across the year
- **Overview tab** — Stat cards (avg score, percentile, growth from Fall, grade-level placement), score distribution strip chart, and gain-by-grade bar charts. Fall view shows a stacked placement breakdown instead of growth metrics
- **Growth tab** — Percentile vs. growth scatter plot, zero-growth bars by grade, and highest-growth leaderboard. Fall view explains the baseline with a placement breakdown
- **Sub-Skills tab** — Radar chart for domain performance (phonics, HFW, vocabulary, comprehension) and comprehension sub-score comparison by grade, plus a low-percentile student grid
- **Classrooms tab** — Horizontal bar charts for avg score and growth by teacher, plus a full classroom data table
- **Grade filtering** — Filter all views by grade level (K–5 or All)
- **Interactive charts** — Hover tooltips on all charts for individual student and classroom detail

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
