# Documentation Quality — Best Practices

This document lists concise, actionable guidelines to make project documentation easy to discover, install, run, validate, cite, and contribute to.

## Table of contents

- [1. Project overview & discoverability](#1-project-overview--discoverability)
- [2. Running the tool (Quick Start)](#2-running-the-tool-quick-start)
- [3. Tool interface & parameters](#3-tool-interface--parameters)
- [4. Reproducibility & data access](#4-reproducibility--data-access)
- [5. Licensing, maintenance & support](#5-licensing-maintenance--support)
- [6. Quick checklist](#6-quick-checklist)

---

## 1. Project overview & discoverability

- **Purpose:** Briefly state what the project does and why it exists.
- **Scope:** Define intended use-cases and limits.
- **Authors & contacts:** List maintainers and how to reach them.
- **Discoverability:** Add a short, searchable description and keywords in the `README` and repository metadata.
- **Related resources:** Link other docs, papers, API specs, or outputs.

Tips:

- Keep the first paragraph short (1–2 sentences) so it appears clearly in search results.
- Add badges (CI, license, PyPI/GitHub package) if available.

## 2. Running the tool (Quick Start)

Provide the smallest-possible runnable example that demonstrates the main functionality.

Example (replace with concrete command for your project):

```bash
# Install (example)
pip install -r requirements.txt

# Quick run: input -> command -> output
python run.py --input data/example.csv --output out/results.csv

# Show help
python run.py --help
```

Include expected sample input and the key parts of expected output so users can quickly validate the setup.

## 3. Tool interface & parameters

- **CLI & flags:** Document all command-line options and environment variables; include `--help` output in docs.
- **Input/Output formats:** Describe file formats, schemas, and example snippets.
- **Configuration:** Show default config locations and how to override them.
- **Hardware requirements:** Note if GPU/TPU or large memory is required.

Advanced usage:

- Provide examples for common workflows and for chaining components together.

## 4. Reproducibility & data access

- **Quick-start validation:** Ensure the quick-start example runs end-to-end without manual steps.
- **Data access:** If external datasets are needed, provide download links, checksums, and an automated script to fetch and verify data.
- **Seeds & deterministic runs:** Note random seeds and how to reproduce results.

If links point to external resources, verify them periodically and document the last verification date.

## 5. Licensing, maintenance & support

- **License:** Add a `LICENSE` file and mention the license prominently in the `README`.
- **Contributing:** Point to `CONTRIBUTING.md` with contribution guidelines and code of conduct.
- **Issues & support:** Tell users how to report bugs or request features (GitHub Issues, mailing list, etc.).
- **Maintenance status:** Indicate whether the project is actively maintained, in maintenance mode, or archived.

## 6. Quick checklist

- **README:** Clear project summary, TOC, and quick-start example.
- **Install:** One-line install + reproducible environment file (`requirements.txt`/`environment.yml`/`pyproject.toml`).
- **Usage:** Example commands and expected outputs.
- **Repro:** Data download scripts, checksums, seeds.
- **Support:** `CONTRIBUTING.md`, `LICENSE`, and issue template.

---
