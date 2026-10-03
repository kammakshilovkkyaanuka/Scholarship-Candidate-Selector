# ScholarshipOS

An interactive DAA scholarship selection visualizer built with React, Vite, Tailwind CSS, and Recharts. Merge sort, greedy selection, and sparse exact 0/1 knapsack dynamic programming run on actual CSV data. The right activity panel replays the real execution trace while the dashboard stays visible.

## Run locally

1. Install dependencies: `npm install`
2. Start the frontend: `npm run dev`
3. Optional Node.js JSON storage API: `node server/index.mjs` in a second terminal. It writes the current workspace to `server/data/workspace.json`. The app also saves locally in browser storage and works without the API.

Open the local Vite URL, upload a CSV or load the fictional demo data, review validation, configure rules, then run selection. Use **Download sample file** to get a CSV with the required columns and 26 fictional records.

The DP objective is to maximize total combined candidate score subject to budget and slot constraints. Category and parent government job are eligibility rules, not scoring inputs. The activity display is a timed replay of trace events emitted by real algorithm execution, not a simulated algorithm.