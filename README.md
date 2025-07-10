# Orchestatr

Welcome to **Orchestatr** — a structured, AI-assisted workflow for managing product documentation, feature development, and task iteration using markdown cursor rules (`.mdc` files).

This repo streamlines the product lifecycle by guiding AI-powered interactions to generate and maintain documentation, requirements, task lists, and implementation progress — all version controlled in Markdown.

---

## Table of Contents

- [Project Structure](#project-structure)
- [Getting Started — Project Initiation](#getting-started--project-initiation)
- [Ongoing Feature Development](#ongoing-feature-development)
- [Documentation Context](#documentation-context)
- [Contributing](#contributing)
- [License](#license)

---

## Project Structure

```plaintext
├── .cursor/rules/           # AI workflow rules (mdc files)
│   ├── app/
│   │   ├── 01_start/        # Project initiation rules (product brief, research, etc.)
│   │   └── features/        # Feature PRD, task generation, iteration rules
│   └── site/                # (Other site-specific rules)
├── library_docs/            # Supporting research docs (copywriting, UX, SEO, etc.)
│   ├── copywriting/
│   ├── design_ux/
│   └── seo/
├── docs/                    # Generated documentation (product briefs, PRDs, etc.)
├── tasks/                   # Generated task lists for features and setup
├── README.md                # This file
```

---

## Getting Started — Project Initiation

Run the `.mdc` rules in `.cursor/rules/app/01_start` sequentially to build foundational docs:

1. `01_create_product_brief.mdc`
2. `02_create_market_user_research.mdc`
3. `03_create_feature_spec.mdc`
4. `04_create_design_guidelines.mdc`
5. `05_create_architecture.mdc`
6. `06_create_metrics_risks.mdc`
7. `07_create_mvp_tasks.mdc`

Each rule guides the AI to generate a specific foundational document. Output is saved in `/docs` and `/tasks`.

---

## Ongoing Feature Development

Use `.cursor/rules/app/features/`:

- `create-prd.mdc` — Generate a PRD for a new feature.
- `generate-tasks.mdc` — Create implementation tasks from a PRD.
- `iterate-tasks.mdc` — Work through tasks, marking progress.

Example workflow:

1. Use `create-prd.mdc` to generate a PRD from your feature idea.
2. Use `generate-tasks.mdc` to create tasks from the PRD.
3. Use `iterate-tasks.mdc` to execute and track tasks.

---

## Documentation Context

Supporting research and best practices are in `library_docs/`:
- `copywriting/` — Copywriting guides, CTAs, headline formulas, etc.
- `design_ux/` — UX/design principles, wireframing, font pairings, etc.
- `seo/` — SEO processes, keyword research, on-page SEO, etc.

Reference these documents as needed for context and best practices.

---

## Contributing

- Add new `.mdc` rules to `.cursor/rules/` as needed.
- Update this README and comment your rules for clarity.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Empower your team with AI-guided, structured, and maintainable product delivery workflows.