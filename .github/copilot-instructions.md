# Copilot Custom Instructions: App + Step-by-Step Tutorial With Step Numbers

When I ask you to **create an app** (any kind: CLI, web, API, desktop, etc.), you MUST do all of the following:

## 1) Always generate a tutorial markdown file
- Create a Markdown file named: `TUTORIAL.md`
- The tutorial MUST be **numbered step-by-step** (1, 2, 3, …) and complete enough that I can follow it from an empty folder to a working app.
- Each step MUST include:
  - What to do
  - The exact file(s) involved
  - The exact code to add or change (snippets are fine)
  - Clear references to where that code lives (file paths, and line references when practical)

## 2) Code must include step-number comments that match the tutorial
- In the source code, include comments that explicitly map back to the tutorial step number.
- Format for the mapping comment:
  - JavaScript/TypeScript: `// Step X: <short description>`
  - HTML: `<!-- Step X: <short description> -->`
  - CSS: `/* Step X: <short description> */`
  - Shell scripts: `# Step X: <short description>`
- If a single tutorial step modifies multiple files, EACH modified area must include the relevant `Step X` comment.

## 3) Maintain a step-to-code map inside the tutorial
At the end of `TUTORIAL.md`, include a section:

### Step-to-Code Map
For each step, list the touched files and the key function/class/module names created or edited.

Example format:
- Step 3: `lib/server.js` (create `startServer()`), `index.html` (wire UI to API)

## 4) Keep steps stable and consistent
- Do not renumber steps mid-generation.
- If the design changes, add a new step rather than silently changing earlier steps.

## 5) Default project conventions (unless I say otherwise)
- Prefer simple, minimal dependencies.
- Generate a clear folder structure.
- Include a `README.md` with how to run, test (if applicable), and build.