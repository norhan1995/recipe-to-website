---
doc: spec
status: approved
---
# Recipe to Website — technical spec
## How This Works, In Plain Language
HTML builds the workspace. CSS styles it. JavaScript holds the three edited snippets and combines them into a separate preview page. Download produces the same complete page as an HTML file.
## Stack
Plain HTML, CSS, JavaScript; browser APIs only. No runtime dependencies, model calls, API keys, or database. This approach was part of the approved combined plan.
## Where It Runs and How Someone Tries It
Run `python3 -m http.server 8765 --directory dist` from the repository root and open http://localhost:8765. Hosted preview is supplemental to the required public repo and demo video.
## Components
- dist/index.html: workspace, editor, preview frame, controls.
- dist/style.css: theme, desktop grid, mobile layout.
- dist/app.js: lessons, editor state, run/reset/export handlers.
## Data Model
Three strings (html, css, js) and current recipe index in memory. Switching tabs preserves edits; reload clears them.
## Core Data Flow
Editor content goes into the selected snippet. compose() wraps all snippets into an HTML document. renderPreview() assigns that document to the sandboxed frame. download() packages it as a text/html Blob.
## Important Failure Modes
JavaScript syntax errors: display feedback. Missing HTML heading: recipe-specific hint. Browser download restrictions: the UI initiates export from a user action. Infinite scripts can hang a preview; there is no execution time limit.
## Preview Boundary
iframe uses allow-scripts without allow-same-origin. Its CSP denies external resources, connections, and form submissions. The exported file intentionally runs independently; only use code you understand and trust.
## Optional Browser Agent Tool
Feature-detected set_recipe_code uses the same switch/run actions and validates inputs. Supported-context validation remains unavailable until a browser capable of that API is available; ordinary UI does not depend on it.
## Verification
Check heading edits, CSS color, click interaction, independent export, mobile overflow, syntax feedback, and workspace errors. Learner hands-on review and reflection are separate from agent verification.
