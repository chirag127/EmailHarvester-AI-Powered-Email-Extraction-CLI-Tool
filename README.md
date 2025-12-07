# MailHunter-Email-Scraper-Web-CLI-Tool

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/ci.yml?style=flat-square)](https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool?style=flat-square)](https://codecov.io/gh/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool)
[![Tech Stack](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Lint/Format](https://img.shields.io/badge/Ruff-Fast-orange?style=flat-square&logo=ruff)](https://github.com/astral-sh/ruff)
[![License](https://img.shields.io/github/license/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool?style=flat-square)](https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool)

**Automated extraction of emails from web pages and Google search results, saving data to SQLite and exportable CSV/TXT. A robust Python CLI tool for efficient data harvesting and management.**

--- 

## 🚀 Project Overview

MailHunter is a powerful, high-velocity Command Line Interface (CLI) tool designed for professional data extraction. It automates the tedious process of identifying and collecting email addresses from various online sources, including dynamic web pages and Google search result pages. The extracted data is reliably stored in an SQLite database and can be seamlessly exported into CSV or TXT formats, providing unparalleled flexibility for data analysis and integration.

--- 

## 🌳 Architecture

This project adheres to a **Modular Monolith** architecture, ensuring clear separation of concerns within a single, deployable unit. This pattern facilitates maintainability, testability, and scalability.

mermaid
graph TD
    A[CLI Interface (Click)] --> B(Core Logic)
    B --> C{Data Extraction Module}
    C --> D(Web Scraper)
    C --> E(Google Search Scraper)
    B --> F{Data Storage Module}
    F --> G[SQLite Database]
    F --> H(CSV/TXT Exporter)
    B --> I{Utils & Config}


--- 

## 🧭 Table of Contents

*   [Project Overview](#-project-overview)
*   [Architecture](#-architecture)
*   [Table of Contents](#-table-of-contents)
*   [AI Agent Directives](#-ai-agent-directives)
*   [Setup & Installation](#-setup--installation)
*   [Usage](#-usage)
*   [Configuration](#-configuration)
*   [Development Standards](#-development-standards)
*   [Testing & Verification](#-testing--verification)
*   [License](#-license)
*   [Contributing](#-contributing)
*   [Security](#-security)

--- 

## 🤖 AI Agent Directives

<details>
<summary>View Agent Directives</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`pyproject.toml` for Python) and apply the corresponding **Apex Toolchain**. This repository, `MailHunter-Email-Scraper-Web-CLI-Tool`, is a Python-based email extraction tool.

*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like web scraping, email extraction, and CLI interface, while maintaining a unified deployment.
    *   **CLI Framework:** Uses `Click` for a powerful and intuitive command-line interface.

*   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function.***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).

---

## 4. APEX NAMING CONVENTION (THE "STAR VELOCITY" ENGINE)
A high-performing name must instantly communicate **Product**, **Function**, **Platform** and **Type**.

**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens` (e.g., `ChatFlow-AI-Powered-Real-Time-Chat-Web-App`).

---

## 5. PRODUCT REPOSITORY MANDATES (THE "STANDARD 11")

Every repository **MUST** appear professional and be fully documented for immediate onboarding and operation.

1.  **README.md:** Hero-tier documentation.
2.  **PROPOSED_README.md:** A proposal for the new README, strictly following AGENTS.md.
3.  **badges.yml:** Configuration for badges.
4.  **LICENSE:** "CC BY-NC 4.0".
5.  **.gitignore:** Standardized project ignore file.
6.  **.github/workflows/ci.yml:** CI/CD pipeline.
7.  **.github/CONTRIBUTING.md:** Contribution guidelines.
8.  **.github/ISSUE_TEMPLATE/bug_report.md:** Issue template for bug reports.
9.  **.github/PULL_REQUEST_TEMPLATE.md:** Pull request template.
10. **.github/SECURITY.md:** Security policy and guidelines.
11. **AGENTS.md:** The agent directives document (this file).

---

## 6. THE README REPLICATION PROTOCOL (THE ULTIMATE ARTIFACT)
The README is a self-contained **Project Operating System**.

**Required Sections:**
1.  **VISUAL AUTHORITY (Above the Fold):**
    *   Hero Banner/Logo (Placeholder).
    *   **Live Badges** (Shields.io):
        *   **Style:** `flat-square` (MANDATORY).
        *   **User:** `chirag127` (MANDATORY).
        *   **Required Badges:** Build Status, Code Coverage, Tech Stack, Lint/Format, License, GitHub Stars.
    *   **Social Proof:** "Star ⭐ this Repo" button.
2.  **STRUCTURAL CLARITY:**
    *   **BLUF:** 2-sentence value proposition.
    *   **Architecture:** ASCII `tree` or Mermaid diagram.
    *   **Table of Contents.**
3.  **🤖 AI AGENT DIRECTIVES (CRITICAL):**
    *   Must be in a collapsible `<details>` block.
    *   **Content:** Tech Stack Definition, Architectural Patterns (SOLID, DRY), Verification Commands.
    *   **Purpose:** Allows future agents to align immediately.
4.  **DEVELOPMENT STANDARDS:**
    *   Setup commands (`git clone` -> `uv venv` -> `uv pip sync`).
    *   Scripts table (`Makefile` or `pyproject.toml` `[tool.scripts]`).
    *   Principles (SOLID, DRY, YAGNI).

---

## 7. CHAIN OF THOUGHT (CoT) PROTOCOL
Before generating JSON, perform deep analysis in `<thinking>` block:
1.  **Audit:** Analyze repo content and purpose.
2.  **Pivot/Archive Decision:** If junk, rename. If viable, PIVOT to elite status.
3.  **Naming Strategy:** Apply `<Product>-<Function>-<Type>` formula.
4.  **Replication Protocol:** Draft "AI Agent Directives" block.
5.  **File Generation:** Plan content for all 11 required files.
6.  **Final Polish:** Ensure all badges and "Standard 11" are present.
7.  **Strict Adherence:** Ensure `PROPOSED_README.md` strictly follows AGENTS.md.

---

## 8. DYNAMIC URL & BADGE PROTOCOL
**Mandate:** All generated files MUST use the correct dynamic URLs based on the **New Repository Name**.

**Rules:**
1.  **Base URL:** `https://github.com/chirag127/<New-Repo-Name>`
2.  **Badge URLs:** All badges (Shields.io) must point to this Base URL or its specific workflows.
3.  **Consistency:** Never use the old/original repository name in links.
4.  **AGENTS.md Customization:** The generated `AGENTS.md` **MUST** be customized for the specific repository's technology stack.

---

## 9. TESTING & VERIFICATION COMMANDS

*   **Linting & Formatting:**
    bash
    uv run --target ruff check . 
    uv run --target ruff format . 
    
*   **Unit & Integration Tests:**
    bash
    uv run --target pytest tests/
    
*   **Full CI Pipeline Simulation:**
    bash
    uv run --target python -m pytest tests/ && uv run --target ruff check . && uv run --target ruff format . --check
    

---

## 10. DEVELOPMENT PRINCIPLES

*   **SOLID:** Adherence to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles.
*   **DRY:** Don't Repeat Yourself. Maximize code reuse and minimize redundancy.
*   **YAGNI:** You Ain't Gonna Need It. Focus on current requirements, avoid over-engineering.

</details>

--- 

## ⚙️ Setup & Installation

This project uses Python 3.10+ and `uv` for package management. It is recommended to use a virtual environment.

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool.git
    cd MailHunter-Email-Scraper-Web-CLI-Tool
    

2.  **Create and activate a virtual environment using `uv`:**
    bash
    uv venv
    source .venv/bin/activate   # On Linux/macOS
    # .venv\Scripts\activate    # On Windows
    

3.  **Install dependencies:**
    bash
    uv pip sync
    

4.  **Install the CLI tool globally (optional, for easy access):**
    bash
    uv pip install -e .
    

--- 

## 💡 Usage

Run the MailHunter CLI tool using the `mailhunter` command after installation, or via `uv run --target mailhunter` if not installed globally.

**Basic Example: Scrape emails from a URL**

bash
mailhunter scrape <URL> --output-format csv


**Scrape emails from Google Search Results**

bash
mailhunter google <SEARCH_TERM> --max-pages 5 --output-format sqlite


**View available commands and options:**

bash
mailhunter --help


Refer to the `Click` CLI help for detailed options for each command.

--- 

## 🔧 Configuration

Configuration can be managed via command-line arguments or environment variables. For advanced settings, a `config.toml` file can be placed in the project root or a user-specific configuration directory.

*   **Environment Variables:** `MAILHUNTER_OUTPUT_FORMAT`, `MAILHUNTER_DB_PATH`, etc.
*   **CLI Arguments:** `--output-format`, `--db-path`, etc.

--- 

## 📜 Development Standards

*   **Code Quality:** Adhere strictly to PEP 8 guidelines, enforced by `Ruff`.
*   **Readability:** Write clear, concise, and well-commented code.
*   **Modularity:** Design components with clear responsibilities (SOLID principles).
*   **Efficiency:** Optimize for performance and resource utilization.
*   **Repeatability:** Ensure reproducible builds and environments (DRY principle).

---

## 🧪 Testing & Verification

Comprehensive tests are crucial for ensuring the stability and correctness of MailHunter.

*   **Linting & Formatting:**
    bash
    uv run --target ruff check . 
    uv run --target ruff format . 
    
*   **Unit & Integration Tests:**
    bash
    uv run --target pytest tests/
    
*   **Full CI Pipeline Simulation:**
    bash
    uv run --target python -m pytest tests/ && uv run --target ruff check . && uv run --target ruff format . --check
    

--- 

## ⚖️ License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](LICENSE) file for more details.

--- 

## 🤝 Contributing

We welcome contributions! Please read our [CONTRIBUTING.md](.github/CONTRIBUTING.md) file for details on the code of conduct, and the process for submitting pull requests.

--- 

## 🛡️ Security

For security-related issues, please refer to our [SECURITY.md](.github/SECURITY.md) file for responsible disclosure guidelines.

--- 

<p align="center">
  <a href="https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/stargazers" target="_blank">
    ⭐ Star ⭐ This Repo
  </a>
</p>
