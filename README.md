# Recipe to Website
A small coding workspace that pairs HTML, CSS, and JavaScript recipes with a live personal-page preview.

## Run
Python 3 is enough: `python3 -m http.server 8765 --directory dist` then visit http://localhost:8765.

No installation or API key is required. Edit a snippet, press Run my code, inspect the preview, and download my-first-page.html.

## Planning
The public planning files are in devpost/: scope.md, prd.md, spec.md, and checklist.md. The project was started from an empty directory on October 5, 2026. The Devpost Learn Skill Pack was read and used to plan the core loop and implementation; the learner chose the direction and approved the combined build plan.

## Limits
Code is kept only for the current visit. Checks are recipe hints, not a full validator. Preview code runs in a sandboxed iframe with restricted resources. It can still consume processing time. Exported code runs independently.

## AI usage
Codex organized the learner's choices into planning documents and implemented the app. The app itself makes no AI API calls. Do not interpret agent work as evidence of the learner's personal learning outcomes.
