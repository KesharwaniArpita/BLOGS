## Outreachy Proposal Timeline for the Ersilia Model Hub Internship

### 🗓️ Overview
This plan outlines my 12-week journey as an Outreachy intern at the Ersilia Model Hub, structured in three progressive phases: onboarding, intermediate contributions, and a self-directed project. My approach combines technical growth in Python development, testing, and CLI tooling, with alignment to Ersilia's mission of enabling accessible AI for infectious and neglected diseases.

---

### 📍 Phase 1: Weeks 1–3 — Onboarding & Minor Contributions
**Goal:** Gain deep familiarity with the Ersilia ecosystem, its CLI, development guidelines, and collaborative tools. Make small but meaningful contributions while learning best practices.

#### 📌 Tasks:
- Follow the [Quick Start Guide](https://github.com/ersilia-os/ersilia) to:
  - Set up a local development environment using `conda`. (As practised/did in contribution period)
  - Install the Ersilia CLI via pip (either from GitHub or PyPI). (As practised/did in contribution period)
  - Fetch and serve a model (e.g., `ersilia fetch eos4e40`, `ersilia serve`). (As practised/did in contribution period)
  - Run a prediction via `ersilia run` and understand the CLI output flow
- Learn and implement Ersilia’s contribution standards:
  - Set up and use `pre-commit` and `ruff` for linting and code formatting
  - Use NumPy-style docstrings for documentation consistency
  - Explore GitHub Projects and Issues board to understand the development workflow
- Tackle 3–5 minor open issues. These might include:
  - Improving CLI error messages and output formatting
  - Enhancing help documentation in the CLI
  - Fixing minor bugs or improving test coverage using `pytest`
  - Contributing small updates to the README or example usage files

#### 🧠 Learning Outcomes:
- Comfort with the Ersilia CLI and backend workflow
- Ability to make confident contributions via GitHub
- Familiarity with pre-commit hooks, linting tools, and collaborative workflows

---

### 📍 Phase 2: Weeks 4–7 — Intermediate Contributions: CLI Enhancements or Testing Tools
**Goal:** Take ownership of a medium-scale contribution by focusing on improving usability, testing infrastructure, or CI workflows.

#### 📌 Potential Tracks:

**Track A: CLI Usability Enhancements**
- Expand CLI commands to be more user-friendly and robust
- Address issues like:
  - Session handling bugs (e.g., #1519)
  - Enhancing `info` and `run` outputs
  - Improving CLI logs or response messages for model status

**Track B: Model Testing Automation**
- Design a CLI command like `ersilia test-models`:
  - Iterates over all registered models
  - Checks if the model can be fetched, served, and run
  - Outputs a structured log (CSV/JSON) of test results
- Optionally link this with a GitHub Action to automatically test models weekly (related to #1538, #1319)

#### 📌 Additional Contributions:
- Write or improve `pytest` test cases for CLI functions
- Help improve `test_serve.py`, `test_run.py`, etc.
- Expand CLI documentation and example usage

#### 🧠 Learning Outcomes:
- Stronger understanding of test-driven development
- CLI architecture and error handling patterns
- Experience with automation workflows (GitHub Actions)

---

### 📍 Phase 3: Weeks 8–13 — Independent Project: New Model Integration or CLI Tooling
**Goal:** Lead a high-impact, self-directed contribution aligned with Ersilia’s goals. This may involve integrating a new model or developing a standalone tool to assist with model management.

#### 📌 Option A: New Model Integration
- Use Ersilia’s [Submit a New Model](https://github.com/ersilia-os/ersilia#submit-a-new-model) workflow:
  - Open a `model request` issue using the provided template
  - Collaborate with maintainers to fork the model template repo
  - Implement CLI wrapping, model testing, and documentation
  - Validate model using the standard CLI commands: `fetch`, `serve`, `run`
  - Write tests and ensure model passes CLI pipeline

#### 📌 Option B: Model Testing CLI Tool
- Expand `ersilia test-models` to:
  - Run tests on multiple endpoints
  - Output visual logs (e.g., pass/fail dashboards)
  - Possibly integrate Redis-based caching (related to #1470)

#### 📌 Option C: CLI Dashboard or Metadata Tracker
- Build a CLI command to:
  - Show model readiness (Ready, Needs Fixing, Deprecated)
  - Show metadata, last test date, performance metrics

#### 📌 Final Deliverables:
- 1 complete, tested model or tool integrated into the main repo
- Related documentation and tutorials
- A blog post or final summary report on my Outreachy experience and project

#### 🧠 Learning Outcomes:
- Project ownership and collaboration with maintainers
- Researching and integrating models based on literature
- Deep understanding of reproducibility, validation, and open science tooling

---

### 🎯 Why This Plan Works
This phased approach is designed to maximize both learning and contribution. It begins with structured onboarding, expands into ownership of mid-sized tasks, and culminates in a meaningful, independently-driven project. It’s aligned with Ersilia’s values of open collaboration, documentation, and accessible tooling for neglected disease research.

By the end of the internship, I hope to not only contribute code but also build tools and documentation that can empower future contributors to succeed.

