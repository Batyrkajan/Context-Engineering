🚀 Project Awareness & Context

Always read PLANNING.md at the start of a session to align with the site's architecture, aesthetic, and goals.
Check TASK.md before starting a new task; add missing tasks with a brief description and today’s date.
Follow consistent naming conventions, file structure, and architecture patterns defined in PLANNING.md.
Use node version 20.x with pnpm for consistent builds and dependency management.
🧱 Code Structure & Modularity

No file should exceed 300 lines of code; split into modular components or hooks if approaching this limit.
Organize by feature and responsibility:
components/ → reusable UI and layout elements
app/ → page routes using App Router
lib/ → utilities, analytics, and API integrations
styles/ → global and modular styles
Prefer relative imports within the project for clarity.
Document new reusable components with README.md inside the component folder if needed.
🧪 Testing & Reliability

Add unit or integration tests for significant utilities or reusable components.
Use Playwright or Cypress for end-to-end testing when testing interactive elements or animations.
Store tests in a __tests__/ folder alongside the component or in /tests mirroring the structure.
For each feature:
1 test for standard usage
1 test for edge cases
1 test for failure/error handling
✅ Task Completion

Mark finished tasks in TODO.md immediately after completion.
Log new subtasks discovered during work under “Discovered During Work” in TODO.md.
🎨 Style & Conventions

Use TypeScript for all files (.tsx, .ts).
Format code with Prettier and enforce linting with ESLint.
Use Tailwind CSS for styling with dark mode as default.
Animations: Use Framer Motion consistently for transitions and interactions.
3D: Use Three.js with React Three Fiber in a modular, easily removable structure if experiments change.
Handwritten font highlights: Use consistent class naming (e.g., font-handwritten) and limit to headings for aesthetic consistency.
📚 Documentation & Explainability

Keep README.md updated with features, library choices, and setup instructions.
Add comments explaining non-obvious logic (especially shaders, Three.js interactions, and Framer Motion animations).
Use inline // Reason: comments to explain “why” design/logic choices were made.
🌐 Git & Deployment

Commit to GitHub after each completed feature or significant milestone with clear, descriptive commit messages.
Use feature branches named clearly (feature/hero-3d, feature/framer-animations) for organization.
Deploy to Vercel automatically with each main push.
🤖 AI Agent Rules

Never assume missing context; ask for clarifications if unsure.
Use verified and documented Next.js, Tailwind, Framer Motion, and Three.js patterns only.
Confirm file paths and module names before referencing.
Do not delete or overwrite existing code unless explicitly part of a TASK.md entry or user instruction.
