# 🐞 Bug Report: Apex Protocol Violation Encountered

This template ensures we capture the necessary diagnostic data to maintain the **Zero-Defect** standard of the `EmailHarvester-AI-Powered-Email-Extraction-CLI-Tool`.

--- 

## 1. Context and Environment

**What version of the tool are you running?**
<!-- Specify the exact version or commit hash, e.g., `v1.2.0` or `HEAD` -->

**Operating System and Version:**
<!-- e.g., Ubuntu 22.04, Windows 11, macOS Sonoma -->

**Python Environment:**
<!-- e.g., Python 3.12.1, running under uv virtual environment -->

## 2. Description of the Bug

A clear and concise description of what the bug is. What did you expect to happen, and what actually happened?

[Describe the unexpected behavior here]

## 3. Steps to Reproduce

List the precise, ordered steps that allow us to reliably reproduce the issue. Assume the environment is clean (fresh install).

1.  `[CLI Command Used]`
2.  `[Input File/URL Used]`
3.  `[Relevant Configuration Flag, e.g., --aggressive]`
4.  ...

## 4. Expected Behavior vs. Actual Behavior

| Behavior Type | Description |
| :--- | :--- |
| **Expected** | [What should have happened based on documentation/logic] |
| **Actual** | [What actually occurred; include error messages if applicable] |

## 5. Diagnostic Information (Logs/Tracebacks)

Please paste the full, unfiltered traceback or error output below. If this involves AI processing, describe the input that caused the failure in the AI handler.

bash
# Paste the full traceback here


## 6. Architectural Alignment Check (Self-Assessment)

As per the **Apex Directives**, we strive for modularity and adherence to SOLID principles. Does this bug suggest a violation of a known pattern? (Optional but helpful)

- [ ] DRY Violation Suspected
- [ ] Poor Error Handling in I/O Adapter
- [ ] AI Inference Result Mismatch

## 7. Severity Assessment

How critical is this issue to the core function of email extraction?

- [ ] **Critical:** Core functionality (extraction/CLI execution) completely broken.
- [ ] **Major:** Significant feature impaired, but workarounds exist.
- [ ] **Minor:** UI/UX issue or documentation discrepancy.
- [ ] **Trivial:** Typos, formatting issues.
