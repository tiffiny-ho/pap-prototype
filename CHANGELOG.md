# Changelog — v2.0 Prototype

## Initial modular conversion
- Added independent modular project folder; original v1 source files are not modified.
- Extracted shared CSS and split the original form JavaScript into state, app, patient, form controls, validation, and summary modules.
- Preserved existing A–E form structure, field labels/options, branching controls, and step-level validation as the starting baseline.
- Replaced the old hard-coded PDF identity/sign-off content with a prototype print preview that displays selected fields and never claims Pathologist validation.
- Added local browser worklist and simulated routing.
- Added validation policy configuration with safe default: not configured; screener-only finalization blocked by default.
- Added visible prototype disclaimers and fictional-data warning.

## Business logic impact
- Existing clinical form option values and step validation are retained.
- Workflow behavior intentionally changed for safety: finalization is blocked unless a prototype-only policy explicitly enables it; this is not an approved clinical rule.
- Login and role selection remain simulated and must not be considered access control.
- PDF output behavior intentionally changed: only selected values are shown; report is watermarked/labeled prototype preview.

## Not yet implemented
- Full original PDF data-field regression matrix and page-break QA.
- Formal SOP-derived referral rules (not supplied).
- Real identity, authorization, persistence, audit trail, LIS integration, Google Apps Script, database, API.
- Official verified KKM logo file.
