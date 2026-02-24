# Stress-Free Tracker

A Progressive Web App (PWA) to track your stress-free days. Log the days you felt stressed, visualize them on a calendar, and monitor streaks and monthly stats — all stored locally in your browser.

## Features

- 📅 Interactive calendar to visualize stressed days
- 🔥 Tracks your current stress-free streak and longest streak
- 📊 Monthly stress count stats
- 💾 Data persisted in `localStorage` (no account required)
- 📲 Installable as a PWA on desktop and mobile devices

## Live Demo

The app is deployed to GitHub Pages and available at:

**https://rmcampos.github.io/stress-free-tracker/**

## Tech Stack

| Technology | Purpose |
|---|---|
| [Vite](https://vitejs.dev/) | Build tool and development server |
| [vite-plugin-pwa](https://vite-pwa-org.netlify.app/) | PWA support (service worker, web app manifest, offline caching) |
| Vanilla JavaScript | Application logic |
| CSS | Styling |

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v20 or later
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/RMCampos/stress-free-tracker.git
cd stress-free-tracker

# Install dependencies
npm install

# Start the development server
npm run dev
```

Open http://localhost:5173/stress-free-tracker/ in your browser.

### Build for Production

```bash
npm run build
```

The production-ready files will be output to the `dist/` directory.

## Deployment

This project is automatically deployed to **GitHub Pages** on every push to the `main` branch using a GitHub Actions workflow (`.github/workflows/deploy.yml`).

The workflow performs the following steps:

1. Checks out the repository
2. Sets up Node.js 20
3. Installs dependencies with `npm ci`
4. Builds the project with `npm run build`
5. Uploads the `dist/` folder as a Pages artifact
6. Deploys the artifact to GitHub Pages

You can also trigger a deployment manually from the **Actions** tab using the `workflow_dispatch` event.

## License

ISC
