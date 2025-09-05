# Mechatronics System 1

Short repo for course work and version-control practice.

## Feature Branch Test
Testing out feature branch.

## Collaboration & File Policy
- **Commit messages:** short, present tense, explain what/why (e.g., “Add sensor init routine”).
- **Branching:** create feature branches; open PRs for review; merge into `main` only when tested.
- **Frequency:** commit small, logical chunks; push regularly.
- **Conflicts:** resolve locally or via PR; never commit broken builds.
- **Naming:** use clear, consistent file names (e.g., `snake_case` or `kebab-case`); avoid spaces for code files.
- **Reviews:** at least one review for non-trivial changes before merging.

## Additional Questions — Answers

### 1) Can Arduino files be versioned?
**Yes.** Track source files like:
- `.ino`, `.c/.cpp`, `.h/.hpp`
- configuration notes (`README.md`, `docs/`)

**Ignore** build/IDE artifacts so the repo stays clean (handled by `.gitignore`), e.g.:
- `.vscode/`, `.idea/`, `.pio/`, `build/`, `dist/`, `*.elf`, `*.hex`, `__pycache__/`, `*.pyc`

### 2) Can MS Office files be versioned?
**Yes, but they’re binary.** Git will version them, but diffs aren’t human-readable.
- Keep the original `.docx/.pptx/.xlsx` if required for editing.
- For sharing/review, also export a **PDF**.
- If you plan to store *large* Office files frequently, consider **Git LFS** (optional).

### 3) Collaboration rules for this repo
- Use branches for features/assignments; merge via PR after sanity checks.
- Keep commits atomic (one logical change per commit).
- Write helpful PR descriptions (what changed, why, and any testing steps).
- Resolve merge conflicts locally; ensure `main` always builds/opens cleanly.
