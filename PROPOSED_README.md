# MailHunter-Email-Scraper-Web-CLI-Tool

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/ci.yml?style=flat-square&logo=githubactions)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool?style=flat-square&logo=codecov)
![Tech Stack](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python)
![Linter](https://img.shields.io/badge/Ruff-enabled-orange?style=flat-square&logo=ruff)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgray?style=flat-square&logo=creativecommons)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool?style=flat-square&logo=github)

**Effortlessly harvest email addresses from web pages and Google search results with this advanced Python CLI tool, saving data directly to SQLite and supporting CSV/TXT exports.**

---


## Table of Contents

*   [About MailHunter](#about-mailhunter)
*   [Features](#features)
*   [Architecture](#architecture)
*   [Getting Started](#getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Usage](#usage)
*   [Development](#development)
    *   [Setup](#setup)
    *   [Running Tests](#running-tests)
    *   [Linting & Formatting](#linting--formatting)
*   [Contributing](#contributing)
*   [License](#license)

---


## About MailHunter

MailHunter is a powerful and efficient Command Line Interface (CLI) tool designed for automated email extraction. It leverages advanced web scraping techniques to gather email addresses from specified web pages and Google search result pages. The extracted data is intelligently stored in a SQLite database for persistent management and can be easily exported into CSV or TXT formats for further analysis.

---


## Features

*   **Web Page Scraping:** Extracts email addresses from the content of any given URL.
*   **Google Search Integration:** Scrapes emails directly from Google search result pages.
*   **Data Persistence:** Saves extracted emails to a local SQLite database.
*   **Export Options:** Supports exporting data to CSV and TXT formats.
*   **Docker Support:** Includes Dockerfile for containerized deployment and consistent environment.
*   **Robust Error Handling:** Gracefully handles network issues, page loading errors, and malformed data.
*   **Configurable:** User-friendly CLI arguments for customization.

---


## Architecture

MailHunter follows a **Modular Monolith** architectural pattern, ensuring a cohesive yet organized codebase. This approach facilitates clear separation of concerns while maintaining a single deployable unit.

mermaid
graph TD
    A[CLI Entry Point (Click)] --> B(Scraping Orchestrator)
    B --> C{Web Page Scraper}
    B --> D{Google Search Scraper}
    C --> E(Email Extractor)
    D --> E
    E --> F(Data Manager)
    F --> G[(SQLite Database)]
    F --> H(CSV Exporter)
    F --> I(TXT Exporter)
    B --> J(Logger)
    B --> K(Configuration Manager)


---


## Getting Started

### Prerequisites

*   Python 3.10+ installed on your system.
*   `pip` (Python Package Installer).

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool.git
    cd MailHunter-Email-Scraper-Web-CLI-Tool
    

2.  **Install dependencies using uv:**
    bash
    uv install
    

### Usage

Run MailHunter using the command line. Here are some example commands:

*   **Scrape emails from a single URL:**
    bash
    python -m mailhunter scrape url --url "https://example.com"
    

*   **Scrape emails from Google search results for a query:**
    bash
    python -m mailhunter scrape google --query "best python libraries"
    

*   **Save results to a specific database file and export to CSV:**
    bash
    python -m mailhunter scrape url --url "https://example.com" --db-path "./data/emails.db" --export-csv "./exports/emails.csv"
    

*   **Run in headless mode (for web scraping):**
    bash
    python -m mailhunter scrape url --url "https://example.com" --headless
    

---


## Development

### Setup

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool.git
    cd MailHunter-Email-Scraper-Web-CLI-Tool
    

2.  **Set up a virtual environment (recommended):**
    bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
    

3.  **Install development dependencies:**
    bash
    uv install --dev
    

### Running Tests

Execute all tests using Pytest:

bash
pytest


To run tests with coverage reporting:

bash
pytest --cov=mailhunter


### Linting & Formatting

This project uses Ruff for lightning-fast linting and formatting. To check and format your code:

bash
ruff check .
ruff format .


---


## Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/blob/main/.github/CONTRIBUTING.md) file for details on how to submit pull requests and report issues.

---


## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0) - see the [LICENSE](https://github.com/chirag127/MailHunter-Email-Scraper-Web-CLI-Tool/blob/main/LICENSE) file for details.

<details>
  <summary>🤖 AI Agent Directives</summary>

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
  **Directives:** Detect the project type (`pyproject.toml` for Python) and apply the corresponding **Apex Toolchain**. This repository, `MailHunter-Email-Scraper-Web-CLI-Tool`, is a Python-based email scraping tool.

  *   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
      *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
      *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like web scraping, data management, and CLI interface, while maintaining a unified deployment.
      *   **CLI Framework:** Uses `Click` (or similar, e.g., `Typer`) for a powerful and intuitive command-line interface.

  *   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function.***
      *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
      *   **State:** Signals (Standardized).
  </details>
