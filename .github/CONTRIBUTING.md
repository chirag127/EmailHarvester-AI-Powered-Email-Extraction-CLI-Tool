# 🤝 Contributing to MailHunter-Email-Scraper-Web-CLI-Tool

Welcome to the **MailHunter** project! We operate under the philosophy of "Zero-Defect, High-Velocity, Future-Proof." Your contributions are essential to maintaining this professional-grade data harvesting and management engine.

## 📜 Code of Conduct

By participating in this project, you are expected to uphold our [Code of Conduct](https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/blob/main/CODE_OF_CONDUCT.md). Please ensure all interactions are respectful, constructive, and professional.

## 🚀 Getting Started

To set up your development environment, follow these steps. We use **uv** for fast and reproducible dependency management, aligned with the 2026 Apex Standard.

### Prerequisites

*   Python 3.10+
*   Git

### Setup

1.  **Fork and Clone:**
    bash
    git clone https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool.git
    cd MailHunter-Email-Scraper-Web-CLI-Tool
    

2.  **Install Dependencies using uv:**
    We recommend installing `uv` globally or via `pipx`.
    bash
    # Create and activate a virtual environment
    uv venv
    source .venv/bin/activate  # Or .venv\Scripts\activate on Windows

    # Install development dependencies (including Ruff and Pytest)
    uv pip install -r requirements.txt
    uv pip install -r requirements-dev.txt
    

3.  **Install as Editable Package:**
    bash
    uv pip install -e .
    

4.  **Run the CLI Tool (Verification):**
    bash
    mailhunter --help
    

## 🏗️ Development Workflow (The Apex Flow)

### Branching Strategy

All features, bug fixes, and documentation improvements must be done on dedicated branches based on `main`.

*   **Feature Branches:** `feat/<short-descriptive-name>` (e.g., `feat/add-google-search-module`)
*   **Bug Fix Branches:** `fix/<issue-number>-<short-descriptive-name>` (e.g., `fix/101-sqlite-connection-bug`)
*   **Documentation Branches:** `docs/<topic>`

### Commit Conventions

We enforce conventional commits for standardized release logging and automation.

| Type | Description |
| :--- | :--- |
| `feat:` | A new feature for the user. |
| `fix:` | A bug fix. |
| `docs:` | Documentation only changes. |
| `style:` | Changes that do not affect the meaning of the code (whitespace, formatting). |
| `refactor:` | A code change that neither fixes a bug nor adds a feature. |
| `test:` | Adding missing tests or correcting existing tests. |
| `chore:` | Maintenance tasks (e.g., updating CI configuration, dependency bumps). |

### Pull Request Submission

1.  Ensure your branch is up-to-date with `main`.
2.  Run all required checks locally (see **Quality Assurance** below).
3.  Submit a Pull Request targeting the `main` branch.
4.  Fill out the [Pull Request Template](.github/PULL_REQUEST_TEMPLATE.md) completely, referencing relevant issues.
5.  Wait for CI checks to pass and for a core maintainer review.

## ✅ Quality Assurance & Standards

We use **Ruff** for high-speed static analysis and formatting, and **Pytest** for testing. All PRs require robust test coverage and zero linting errors.

### 1. Linting and Formatting (Ruff)

Before committing, ensure your code adheres to Python standards:
bash
# Run Linter (Checks for errors)
ruff check .

# Run Formatter (Auto-fixes styling issues)
ruff format .


### 2. Testing (Pytest)

All new features and bug fixes **must** include corresponding unit or integration tests.

bash
# Run all tests
pytest

# Run tests with coverage reporting
pytest --cov=mailhunter --cov-report term-missing


We require a minimum of **95% overall test coverage** for PR acceptance.

## 🔒 Security

If you discover a security vulnerability, **DO NOT** open a public issue. Please follow the disclosure process outlined in our [SECURITY.md](.github/SECURITY.md) policy.

## ⚖️ Licensing

By contributing, you agree that your submissions will be licensed under the project's **CC BY-NC 4.0** license.
