# Recipe to Website — proposed build plan

## Confirmed choices
- Build a personal page.
- Let the beginner edit guided code snippets.
- Show the result beside the recipe.
- Use a modern, classy visual style.

## Proposed experience
One workspace, with a recipe on the left and the personal page preview on the right. On a phone, the two panels stack vertically.

1. **Structure:** Edit a name, headline, and short introduction in HTML. Run the snippet to see the page change. Explain exactly which tags produce which part of the page.
2. **Style:** Edit colors, spacing, and typography in CSS. Run it to see the same content take on the new design.
3. **Interaction:** Add JavaScript to a button. Click it in the preview and see the response.
4. **Finish:** Download one working HTML file containing all three parts and open it independently.

Each step includes a short explanation, code location, small editing task, example snippet, and reset option. Feedback will identify missing expected elements rather than claim to validate every possible program.

## Proposed technical approach
Use plain HTML, CSS, and JavaScript. This keeps the app and exported result easy to inspect and avoids API keys and ongoing model charges. Run the learner's page inside an isolated preview frame so it cannot read or change the surrounding workspace. No account or uploaded personal information is needed.

A static hosted version lets the learner try the app directly. A public GitHub repository will include the completed code, scope.md, prd.md, spec.md, checklist.md, and factual run instructions. The personal learner profile stays out of public source.

## Build order and evidence
1. Build the first recipe and preview together. Verify that editing the heading changes the rendered result.
2. Add CSS and JavaScript recipes. Verify an actual color change and button interaction.
3. Add download and mobile layout. Open the exported file independently and verify all three parts still work.
4. Have the learner try the finished core journey and resolve their feedback.
5. Record a 1–3 minute demonstration of the actual app, publish the repository, and complete the Devpost draft.

## Required learner participation
The official Devpost Learn Skill Pack uses planning review and hands-on feedback. The plan is a proposal, not a claim of completed learning or approved specifications.

The submission form also asks about resources actually used, AI cost, confidence, project value, and eligibility. These are personal answers and cannot be inferred reliably.

## Current verified status
Devpost account access works. Project 1440529 is an existing Untitled draft for Build With AI: Basics, with no description or demo video and no recorded submission. No entry has been sent.

## Review prompt
Does this plan look good, or what would you change? Once approved, implementation can proceed in fast mode, with a working-app review before submission.
