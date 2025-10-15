# Coaching Assessment

Single-page web app with a cover, 5 pages of 10 questions (0–5 scale), and a results page that shows a radar chart with download options.

## Run

Open `index.html` in a modern browser. No build step required.

## Customize

- Edit question labels in `questions.js` → `window.QUESTIONS.labels`
- Update questions in `questions.js` → `window.QUESTIONS.pages`
- Modify analysis content in `analysis.js` → `window.ANALYSIS`
- Styles are in `styles.css`. Colors are CSS variables in `:root`.

## Export

- Download chart as PNG
- Download CSV of dimension scores

## Notes

- Data is saved in `localStorage` under `assessment_state_v1`.
- Radar chart powered by Chart.js 4.
