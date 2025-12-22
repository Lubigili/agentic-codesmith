CONTRIBUTING
==========

Thanks for your interest in contributing to agentic-codesmith! We welcome contributions of all kinds — bug reports, feature requests, documentation improvements, tests, and code. This document outlines our contributor guidelines, development workflow, testing expectations, code style, pull request process, and how to get in touch.

Table of contents
-----------------
- Welcome
- Getting started
- Development workflow
- Testing
- Code style and linting
- Pull request (PR) process
- Reviewing and merging
- Communication and links
- Code of Conduct

Welcome
-------
We appreciate your effort to make this project better. Whether you're fixing a bug, adding a feature, or improving docs, please follow the guidelines below so we can review and merge contributions quickly and consistently.

Getting started
---------------
1. Fork the repository and clone your fork locally:

   git clone https://github.com/<your-username>/agentic-codesmith.git
   cd agentic-codesmith

2. Create a branch for your work (see Development workflow below):

   git checkout -b feature/short-description

3. Make small, focused changes with clear commit messages.

Development workflow
--------------------
Branching
- main is the canonical branch and should always be in a releasable state. It may be protected.
- Create topic branches off main for all work:
  - feature/<short-description>
  - fix/<short-description>
  - chore/<short-description>
- Keep branches focused and small; a single logical change per branch is ideal.

Commits
- Write clear, descriptive commit messages.
- Follow Conventional Commits (recommended):
  - feat: add a new feature
  - fix: fix a bug
  - docs: documentation only changes
  - style: formatting, missing semicolons, etc; no code change
  - refactor: code change that neither fixes a bug nor adds a feature
  - test: adding or updating tests
  - chore: build process or auxiliary tools
- Squash or clean up WIP commits before opening a PR (we prefer tidy history).

Syncing
- Keep your branch up to date with main when needed:

  git fetch origin
  git checkout main
  git pull
  git checkout feature/your-branch
  git merge main

(Alternatively, rebase if your team prefers: git rebase origin/main)

Testing
-------
We require that contributions include tests where applicable and that all tests pass before merging.

Project-specific test commands
- Update the placeholders below with the actual commands used in this repository.
  - Run the test suite:
    - Example (Node): npm test
    - Example (Python): pytest
  - Run unit tests only (if applicable): npm run test:unit or pytest tests/

Continuous integration (CI)
- CI runs on each PR. Ensure your branch passes all CI checks before requesting a review.
- If CI fails, fix issues and push follow-up commits.

Code style and linting
---------------------
We try to keep a consistent code style across the project. Please run linters and formatters before submitting.

Examples (replace with repo-specific tools):
- JavaScript/TypeScript: prettier, eslint
  - npm run lint
  - npm run format
- Python: black, ruff, flake8
  - black .
  - ruff check .

Formatting
- Prefer automated formatting. Run the project's formatter and ensure no formatting-only diffs remain.

Pull request (PR) process
-------------------------
1. Open an issue first for large features or breaking changes to discuss design and scope.
2. When ready, open a PR from your branch to main with a clear title and description.

PR checklist (please complete before requesting review):
- [ ] The PR is based on the latest main branch.
- [ ] Tests have been added or updated, and all tests pass locally.
- [ ] Linting and formatting are applied.
- [ ] The PR description explains what and why (references to issues if applicable).
- [ ] No sensitive data or secrets are included.

PR description template (suggested)
- Summary of changes
- Motivation and context
- How to test/reproduce
- Screenshots or logs (if applicable)
- Related issues or PRs

Labels and reviewers
- Add appropriate labels (bug, enhancement, docs, test) to help triage.
- Request reviews from teammates familiar with the area.
- For larger changes, request at least two approvers if possible.

Reviewing and merging
---------------------
- Reviews should be constructive and focused on correctness, clarity, and maintainability.
- Address review comments promptly. Push follow-up commits or update the PR as needed.
- Merge strategy:
  - Use squash merges to keep main history concise, unless retention of commit history is desired.
  - Ensure CI is passing and at least one (or the required number of) approvals are present.

Communication and links
-----------------------
- Issues: https://github.com/Lubigili/agentic-codesmith/issues
- Pull requests: https://github.com/Lubigili/agentic-codesmith/pulls
- Discussions (if enabled): https://github.com/Lubigili/agentic-codesmith/discussions
- Maintainer: https://github.com/Lubigili

Optional / project-specific channels
- Slack/Discord: add your project/community invite link here
- Email: team@example.com (replace with real contact)

If you are unsure where to start, check the issue tracker for "good first issue" or contact the maintainers.

Code of Conduct
---------------
Please follow our Code of Conduct. Be respectful and considerate. If a CODE_OF_CONDUCT.md file exists in the repo, follow it. If not, please behave in a way that keeps this project welcoming to everyone.

Thank you
---------
Thanks for taking the time to contribute. Your work helps make agentic-codesmith better for everyone.

If you'd like, I can also:
- Add a PR template, issue templates, or a CODE_OF_CONDUCT.md if one is missing.
- Replace the placeholder test/lint commands with the actual commands used by this repo if you tell me what they are.
