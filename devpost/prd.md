---
doc: prd
status: approved
---
# Recipe to Website — product requirements
Source: scope.md > The Core Loop. Learner approved the displayed combined plan.
## The Core Journey
1. Open a guided personal-page recipe.
2. Change a name and introduction in HTML; run the snippet and inspect the preview.
3. Change CSS color or corner radius; run and inspect the same page.
4. Change a JavaScript greeting; run and click the preview button.
5. Download a standalone HTML file and open it in a browser.
## Screens and Layout
One workspace with recipe, task, editable snippet, explanation, run/reset controls, and preview. Panels stack on mobile. Recipe tabs preserve current edits when changing steps.
## Look and Feel
Modern and classy, as chosen by the learner. Clear typography and intentional purple accents; dark code editor, clean white preview.
## Features and Behavior
### Guided recipes
Each step explains which part of an HTML document receives its snippet. Examples are editable. Reset affects only the selected snippet.
### Preview
Run applies all three current snippets inside a sandboxed frame. CSS and JavaScript examples are available from first use, so the whole page starts working. Changes apply when Run is pressed, rather than on each keystroke.
### Download
Export combines current HTML, CSS, and JavaScript into one independent file.
## States and Boundaries
Empty snippets show a helpful message. JavaScript syntax errors show feedback. Recipe checks are limited heuristics, not full validation. Code remains in memory for the current visit; reloading resets it. Preview scripts have no same-origin access to the surrounding workspace and network connections are blocked by policy. Arbitrary code can still hang its frame; this is not a production untrusted-code execution service.
## Product Decisions
Learner selected personal page, guided editing, and modern/classy look; then approved the plan. Colors, snippet text, and implementation details are agent choices derived from that plan.
## Deferred From the POC
Accounts, permanent saving, AI generation, server execution, collaboration, and a full programming course.
