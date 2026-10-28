# FORGE

A dark fitness app for planning workouts, learning exercises, and logging your training. Built with Vite, JavaScript, and Lucide icons.

## Run locally

Install Node.js 20.19+ or 22.12+ and Git, then:

```sh
git clone https://github.com/Piznzy/codex.git
cd codex
npm ci
npm run dev
```

Open the address Vite prints. Use `npm run build` for a production build and `npm run preview` to serve it locally.

## What you can do

- Browse 16 illustrated exercises with instructions, form cues, muscle and equipment filters, live search, and saved favorites.
- Start one of three starter routines, create your own routine, or begin an empty workout.
- Log sets, reps, and total weight in kg. Add or remove sets and exercises. Timed exercises use seconds in place of reps.
- Complete a set to start an adjustable rest timer. Live workouts survive reloads and can be resumed from any screen.
- Finish a session to save completed sets to history. View session details, repeat a workout, or delete it.
- Track weekly consistency, completed sessions, time, lifting volume, and per-exercise personal bests.
- Set your name, weekly workout goal, and rest duration. Export a JSON copy of training data from settings or history.

## Data and calculations

Data is stored locally in this browser using the `forge-` localStorage keys. There is no account, server, or cross-device sync. Clearing browser storage removes saved data; export first. Previous Sprout habit data remains untouched under its original keys.

Training volume sums `weight × reps` for completed non-timed sets. A pair of dumbbells is logged as their combined weight. Bodyweight exercises can use 0 kg. Personal bests show highest logged load, or longest hold for timed movements. Duration is elapsed time from session start, including rest and time away from the app. Week boundaries use the device's local timezone and Monday start. Only completed sets are saved when finishing a workout.

Exercise figures are schematic illustrations; the written steps provide the movement instructions. All artwork is bundled with the app; Google Fonts is optional and system fonts are used if it is unavailable. No API keys are required.
