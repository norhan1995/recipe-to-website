# Recipe to Website
Three editable app recipes: to-do list, task manager, and finance manager. Each includes layout, design, actions, saving, and useful extras.

## Run
`python3 -m http.server 8765 --directory dist` then open http://localhost:8765. No dependencies or API keys.

## Use
Choose an app, edit a recipe, and press Run my code. Try its form and controls in the live preview. Download a complete standalone HTML app. Edits to each recipe stay in memory while switching apps and steps, but reset on workspace reload.

The isolated preview uses sample data and cannot save records between runs. Downloaded apps save locally when their browser permits localStorage. Clearing browser data removes records. There is no cloud sync. Keep your own backup; finance CSV export covers the selected month.

## Recipes
- To-do: add, complete, delete, and filter tasks.
- Task manager: project, priority, due date, completion, high-priority/overdue filters.
- Finance: dated income/expense entries, categories, selected-month totals, expense budget, and CSV export. Amounts use integer cents and SAR. The budget setting and transaction records persist locally when storage is available. No bank connection.

## Code and planning
`dist/recipes.js` holds the editable examples; `dist/app.js` runs the workspace; `dist/style.css` styles it. `devpost/` holds scope.md, prd.md, spec.md, and checklist.md.

## Boundaries
The iframe has scripts/download permission but no same-origin access. Its policy blocks external resources and network calls. Edited code can still hang its frame; this is a learning tool. Exported code runs independently. Do not paste code you do not understand. Runtime feedback and syntax checks are limited, not a full validator.

## AI usage
The learner chose the direction, reviewed the original app, requested the expansion, and authorized the three recipes. Codex wrote planning documents and code. The app makes no AI calls. Hands-on review and the learner's own learning reflection remain separate from agent verification.
