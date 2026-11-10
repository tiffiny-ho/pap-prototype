# Cytology Report v2.0 — Modular Frontend Prototype

## Run
Open `login.html` in a modern browser. For best behavior, serve this folder with a local static server (for example VS Code Live Server). No backend, GAS, database, or API is included.

## Structure
- `login.html` — simulated role/name selection only
- `dashboard.html` — browser-local prototype worklist
- `cytology-form.html` — existing five-step A–E form markup
- `configuration.html` — safe-default simulated validation policy
- `css/app.css` — shared styling
- `js/00-state.js` — shared prototype state
- `js/01-app.js` — page initialization and navigation
- `js/02-patient.js` — patient lookup mock and input helpers
- `js/03-form-controls.js` — existing form branch controls
- `js/04-validation.js` — existing step validation/navigation
- `js/05-summary.js` — existing summary generation
- `js/06-workflow.js` — simulated routing and safe finalization gate
- `js/07-pdf-engine.js` — print-to-PDF prototype preview

## Safety / limitations
- Use fictional test patients only. LocalStorage is not a secure database or authentication system.
- Default validation policy is unconfigured; Screener-only finalization is blocked unless explicitly enabled in the demo configuration. This toggle is not a clinical authorization.
- No Pathologist validation is fabricated. The generated print preview states that it is not an official report.
- The KKM logo is a placeholder; no unverified logo asset is embedded.
- The original A–E form markup, current labels/options and step validation were carried over from `form_engine_fixed.html`. PDF output is intentionally redesigned to show selected values only, rather than the old incomplete hard-coded PDF content.
