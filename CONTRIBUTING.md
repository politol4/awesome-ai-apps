# Contributing to Awesome AI Apps

Thank you for your interest in contributing to **Awesome AI Apps**! 🎉
We welcome contributions of all kinds — new AI app examples, bug fixes, documentation improvements, and more.

## Table of Contents

- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Adding a New AI App](#adding-a-new-ai-app)
- [Code Style Guidelines](#code-style-guidelines)
- [Pull Request Process](#pull-request-process)
- [Community Guidelines](#community-guidelines)

---

## Getting Started

1. **Fork** the repository by clicking the "Fork" button at the top right of the page.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/<your-username>/awesome-ai-apps.git
   cd awesome-ai-apps
   ```
3. **Create a new branch** for your contribution:
   ```bash
   git checkout -b feat/your-feature-name
   ```

---

## How to Contribute

There are several ways you can contribute:

- 🆕 **Add a new AI app** — Submit a new example app built with AI/LLM tools.
- 🐛 **Report a bug** — Use the [bug report template](.github/ISSUE_TEMPLATE/bug_report.yml).
- 💡 **Request a feature** — Use the [feature request template](.github/ISSUE_TEMPLATE/feature_request.yml).
- ❓ **Ask a question** — Use the [question template](.github/ISSUE_TEMPLATE/question.yml).
- 📝 **Improve documentation** — Fix typos, clarify instructions, or add missing docs.

---

## Adding a New AI App

Each app should live in its own directory following this structure:

```
apps/
└── your-app-name/
    ├── README.md        # Description, setup instructions, demo screenshot
    ├── requirements.txt # Python dependencies
    ├── app.py           # Main entry point
    └── ...              # Any additional files
```

Please use the [README template](.github/README_TEMPLATE.md) when creating your app's `README.md`.

### App Requirements

- The app must be functional and runnable locally.
- Include clear setup and run instructions in the `README.md`.
- List all dependencies in `requirements.txt`.
- Do **not** commit API keys or secrets — use `.env` files and document required environment variables.
- Add a `.env.example` file if environment variables are needed.

---

## Code Style Guidelines

- Follow [PEP 8](https://peps.python.org/pep-0008/) for Python code.
- Use meaningful variable and function names.
- Add docstrings to functions and classes.
- Keep functions small and focused on a single responsibility.
- Run the linter before submitting:
  ```bash
  pip install ruff
  ruff check .
  ```

> **Personal note:** I also like to run `ruff format .` to auto-format code before checking, saves a lot of manual cleanup. It's also worth running `ruff check --fix .` to let ruff auto-fix any fixable lint issues in one go.

---

## Pull Request Process

1. Ensure your branch is up to date with `main`:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
2. Push your branch and open a Pull Request against `main`.
3. Fill out the [Pull Request template](.github/PULL_REQUEST_TEMPLATE.md) completely.
4. Ensure all CI checks pass.
5. A maintai
