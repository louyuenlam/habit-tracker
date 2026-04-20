# Habits

A simple, personal habit tracker. Daily check-ins, monthly calendar view, streak tracking, and a water intake counter.

## Features

- **Today view** — tap to mark habits done, see progress at a glance
- **Monthly calendar** — track completion patterns per habit
- **Streaks** — current + longest for every habit
- **Water tracker** — counts in 400ml increments toward a 2500ml daily goal
- **Offline-capable** — works without internet once loaded
- **Installable** — add to iPhone home screen for a native app feel
- **Private** — all data stays on your device (localStorage)

## Habits tracked

- Read a book
- Workout for 7 min
- Poop
- Learn psychology
- Learn French
- Take supplements
- Drink water (2500ml goal, 400ml per log)

## Deploy to GitHub Pages

1. Create a public repo (e.g. `habit-tracker`) on GitHub
2. Upload both files: `index.html` and `sw.js`
3. Go to **Settings → Pages**
4. Source: **Deploy from a branch**, Branch: **main**, Folder: **/ (root)**
5. Wait 1–2 minutes, then visit `https://<username>.github.io/habit-tracker`

## Install on iPhone

1. Open the URL above in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button
3. Scroll down → **Add to Home Screen**
4. Tap **Add**

The app icon appears on your home screen. Opening it launches full-screen with no browser bars.

## Data

All habit data is stored locally in your browser's `localStorage` under the key `habitTrackerData_v1`. It doesn't leave your device. Clearing browser data or uninstalling the app will erase your history.

## Files

- `index.html` — the full app (HTML + CSS + JS in one file)
- `sw.js` — service worker for offline support

## Local development

No build step. Just open `index.html` in a browser. For offline/service worker testing, serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
