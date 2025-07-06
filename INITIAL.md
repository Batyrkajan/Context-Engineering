🚀 Project Awareness & Context

Always read PLANNING.md at the start of a session to align with the project's architecture, goals, and constraints.
Check TASK.md before starting a new task; add missing tasks with a brief description and today’s date if needed.
Follow consistent naming conventions, file structure, and architecture patterns defined in PLANNING.md.
Use the specified environment and tools for the project (e.g., node, pnpm, venv, Docker) for consistency and reproducibility.
🧱 Code Structure & Modularity

Keep files under 300–500 lines. Split into clear, reusable modules, components, or services if approaching this limit.
Organize code by feature and responsibility, not by type alone:
components/ → UI and reusable elements
lib/ → utilities and helpers
services/ → external integrations, business logic
api/ → routes or handlers
Prefer relative imports within packages for clarity and maintainability.
Document reusable modules with inline comments and, if complex, a README.md in their folder.
🧪 Testing & Reliability

Write tests for all significant logic (functions, components, endpoints).
Use unit tests for core logic and integration/E2E tests for workflows or UI flows.
Store tests in a __tests__/ folder next to modules or in /tests, mirroring the project structure.
Cover:
At least one test for expected behavior
At least one edge case
At least one failure case
✅ Task Management

Mark completed tasks in TODO.md upon completion.
Add new subtasks discovered during development to the “Discovered During Work” section in TODO.md.
🎨 Style & Conventions

Use the primary language and framework(s) specified for the project.
Follow consistent code formatting (Prettier, black, etc.) and linting (ESLint, pylint).
Apply typing (TypeScript for JS/TS projects, type hints for Python).
Write clear docstrings/comments using a consistent format:
def example(param: str) -> int:
    """
    Brief description.

    Args:
        param (str): Description.

    Returns:
        int: Description.
    """
Use environment variable management (dotenv, load_env()) for secrets/configs.
📚 Documentation & Explainability

Keep README.md updated with:
Project description and purpose
Setup instructions
Usage examples
Library choices and reasoning
Comment non-obvious logic and key design decisions.
Use inline # Reason: comments to clarify why something is done, not just what.
🌐 Git & Deployment

Use clear, descriptive commit messages for all commits.
Commit after implementing new features, fixing bugs, or reaching significant milestones.
Use feature branches (feature/xyz) to isolate work.
Keep deployment pipelines (Vercel, Docker, CI/CD) clean and documented in DEPLOYMENT.md if needed.
🤖 AI Code Agent Behavior Rules

Never assume missing context; ask clarifying questions if needed.
Never hallucinate functions or libraries; only use verified, documented packages.
Verify file paths, names, and structures before referencing them in code or tests.
Do not delete or overwrite existing code unless explicitly instructed or if part of a documented task.
🪄 Optional Advanced Practices

Add CONTRIBUTING.md for consistent workflows when collaborating or using AI agents.
Add docs/ folder for:
Library usage notes
Architectural decisions
Developer environment setup
Use semantic versioning for tagging releases.
Create architecture diagrams or ARCHITECTURE.md for complex systems.
