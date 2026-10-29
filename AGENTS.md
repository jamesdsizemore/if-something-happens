# Repository Guidelines

## User Communication Requirement: No Dead-End Replies

The user explicitly requires that this preference persist for this project:

- Never end with only an apology, acknowledgment, admission of failure, status recap, or promise to do better.
- Answer the actual question directly before proposing or starting other work. Do not change the subject or ask unrelated product questions when the user is requesting an explanation or accountability.
- Complete relevant, authorized work and show the concrete result. A process announcement is not a deliverable.
- Keep the next step relevant to the current concern. Do not produce unrelated work merely to appear productive or assume that a file's existence makes it useful to the user.
- If blocked, name the exact blocker and the smallest necessary next step; ask only for information actually needed to proceed.
- State what was actually completed, provide usable evidence where applicable, and avoid unverified claims of completion or persistence.

Recorded from the user's explicit instruction on October 29, 2026.

## Project Structure & Module Organization

`if-something-happens` is an emergency contact information application in its initial repository stage. The checkout currently contains `README.md` and this contributor guide. There are no application modules, tests, assets, dependency manifests, or CI workflows yet.

When adding the initial implementation, choose a directory layout appropriate to the selected stack and document it in `README.md`. Keep application code, tests, and static assets in clearly named locations. Avoid introducing empty directories or tooling for features that do not exist.

## Build, Test, and Development Commands

No build, test, or local server commands are configured. Do not assume commands such as `npm test` or `npm run dev` are available.

Useful checks from the repository root:

- `git status --short`: inspect pending changes before and after work.
- `git diff --check`: detect whitespace errors in tracked changes.
- `git diff`: review the patch before committing.

When introducing a toolchain, document its required version, installation steps, and exact build, test, and development commands in `README.md`. Commit the corresponding dependency lockfile when applicable.

## Coding Style & Naming Conventions

No programming language, indentation standard, formatter, or linter has been established. Follow existing file conventions and use descriptive names. For Markdown, use hash-prefixed headings, fenced command examples, and concise paragraphs. Establish consistent formatting and linting with the first implementation.

## Testing Guidelines

No testing framework or coverage threshold exists. Add relevant tests alongside new behavior and document how to run them. Use descriptive test names that state the scenario and expected result. Report checks actually performed; distinguish automated tests from manual verification.

## Commit & Pull Request Guidelines

History currently contains only `Initial commit`, so no recurring commit convention is established. Use concise, imperative subjects, such as `Add emergency contact form`, and keep commits focused.

Pull requests should explain the change, its purpose, and validation performed. Link related issues when available and include screenshots for visible interface changes. Identify any setup requirements or remaining limitations.

## Security & Configuration

Use synthetic contact data in examples and tests. Never commit real emergency contacts, credentials, or private configuration. Document required configuration names without including secret values.
