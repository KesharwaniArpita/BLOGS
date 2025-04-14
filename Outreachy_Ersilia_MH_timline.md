## Outreachy Proposal Timeline for the Ersilia Model Hub Internship

### 1. Overview  
This plan outlines my 12-week journey as an Outreachy intern at the Ersilia Model Hub, structured in three progressive phases: onboarding, intermediate contributions, and a self-directed project. My approach combines technical growth in Python development, testing, and CLI tooling, with alignment to Ersilia's mission of enabling accessible AI for infectious and neglected diseases.

---

### 2. Phase 1: Weeks 1–3 — Onboarding and Minor Contributions  
**Goal:** Gain deep familiarity with the Ersilia ecosystem, its CLI, development guidelines, and collaborative tools. Make small but meaningful contributions while learning best practices.

2.1. Tasks:
1. Follow the [Quick Start Guide](https://github.com/ersilia-os/ersilia) to:
   1. Set up a local development environment using `conda`. (As practised/did in contribution period)
   2. Install the Ersilia CLI via pip (either from GitHub or PyPI). (As practised/did in contribution period)
   3. Fetch and serve a model (e.g., `ersilia fetch eos4e40`, `ersilia serve`). (As practised/did in contribution period)
   4. Run a prediction via `ersilia run` and understand the CLI output flow
2. Learn and implement Ersilia’s contribution standards:
   1. Set up and use `pre-commit` and `ruff` for linting and code formatting
   2. Use NumPy-style docstrings for documentation consistency
   3. Explore GitHub Projects and Issues board to understand the development workflow
3. Tackle 3–5 minor open issues. These might include:
   1. Improving CLI error messages and output formatting
   2. Enhancing help documentation in the CLI
   3. Fixing minor bugs or improving test coverage using `pytest`
   4. Contributing small updates to the README or example usage files

2.2. Learning Outcomes:
1. Comfort with the Ersilia CLI and backend workflow
2. Ability to make confident contributions via GitHub
3. Familiarity with pre-commit hooks, linting tools, and collaborative workflows

---

### 3. Phase 2: Weeks 4–7 — Intermediate Contributions: CLI Enhancements or Testing Tools  
**Goal:** Take ownership of a medium-scale contribution by focusing on improving usability, testing infrastructure, or CI workflows.

3.1. Potential Tracks:

**Track A: CLI Usability Enhancements**
1. Expand CLI commands to be more user-friendly and robust
2. Address issues like:
   1. Session handling bugs (e.g., #1519)
   2. Enhancing `info` and `run` outputs
   3. Improving CLI logs or response messages for model status

**Track B: Model Testing Automation**
1. Design a CLI command like `ersilia test-models`:
   1. Iterates over all registered models
   2. Checks if the model can be fetched, served, and run
   3. Outputs a structured log (CSV/JSON) of test results
2. Optionally link this with a GitHub Action to automatically test models weekly (related to #1538, #1319)

3.2. Additional Contributions:
1. Write or improve `pytest` test cases for CLI functions
2. Help improve `test_serve.py`, `test_run.py`, etc.
3. Expand CLI documentation and example usage

3.3. Learning Outcomes:
1. Stronger understanding of test-driven development
2. CLI architecture and error handling patterns
3. Experience with automation workflows (GitHub Actions)

---

### 4. Phase 3: Weeks 8–13 — Independent Project: New Model Integration or CLI Tooling  
**Goal:** Lead a high-impact, self-directed contribution aligned with Ersilia’s goals. This may involve integrating a new model or developing a standalone tool to assist with model management.

4.1. Option A: New Model Integration
1. Use Ersilia’s [Submit a New Model](https://github.com/ersilia-os/ersilia#submit-a-new-model) workflow:
   1. Open a `model request` issue using the provided template
   2. Collaborate with maintainers to fork the model template repo
   3. Implement CLI wrapping, model testing, and documentation
   4. Validate model using the standard CLI commands: `fetch`, `serve`, `run`
   5. Write tests and ensure model passes CLI pipeline

4.2. Option B: Model Testing CLI Tool
1. Expand `ersilia test-models` to:
   1. Run tests on multiple endpoints
   2. Output visual logs (e.g., pass/fail dashboards)
   3. Possibly integrate Redis-based caching (related to #1470)

4.3. Option C: CLI Dashboard or Metadata Tracker
1. Build a CLI command to:
   1. Show model readiness (Ready, Needs Fixing, Deprecated)
   2. Show metadata, last test date, performance metrics

4.4. Final Deliverables:
1. One complete, tested model or tool integrated into the main repo
2. Related documentation and tutorials
3. A blog post or final summary report on my Outreachy experience and project

4.5. Learning Outcomes:
1. Project ownership and collaboration with maintainers
2. Researching and integrating models based on literature
3. Deep understanding of reproducibility, validation, and open science tooling

---

This phased approach is designed to maximize both learning and contribution. It begins with structured onboarding, expands into ownership of mid-sized tasks, and culminates in a meaningful, independently-driven project. It’s aligned with Ersilia’s values of open collaboration, documentation, and accessible tooling for neglected disease research.

By the end of the internship, I hope to not only contribute code but also build tools and documentation that can empower future contributors to succeed.
