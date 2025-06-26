# Orchestatr

Welcome to the **Orchestatr** — a structured, AI-assisted workflow for managing product documentation, feature development, and task iteration using markdown cursor rules (`.mdc` files).

This repo is designed to streamline and standardize the entire product lifecycle, from initial concept to post-MVP growth, by guiding AI-powered interactions to generate and maintain critical documentation, product requirements, task lists, and implementation progress — all version controlled in Markdown.

This general approach can easily be extended to work with your favorite task-management software such as Jira, Trello, Clickup, Monday.com, etc. 

---

## Table of Contents

- [Project Structure](#project-structure)
- [Getting Started — Project Initiation](#getting-started--project-initiation)
- [Ongoing Feature Development](#ongoing-feature-development)
- [Task Iteration and Completion](#task-iteration-and-completion)
- [How to Use the `.mdc` Rules](#how-to-use-the-mdc-rules)
- [Integrating Documentation Context](#integrating-documentation-context)
- [Contributing](#contributing)
- [License](#license)

---

## Project Structure

```plaintext
├── 01_start/                # Initial project kickoff documentation rules
│   ├── 01_create_product_brief.mdc
│   ├── 02_create_market_analysis.mdc
│   ├── 03_create_user_personas.mdc
│   ├── 04_create_features_doc.mdc
│   ├── 05_create_user_flows_diagrams.mdc
│   ├── 06_create_ux_design_doc.mdc
│   ├── 07_create_content_strategy.mdc
│   ├── 08_create_architecture_doc.mdc
│   ├── 09_create_security_doc.mdc
│   ├── 10_create_testing_doc.mdc
│   ├── 11_create_performance_doc.mdc
│   ├── 12_create_success_metrics_kpis_doc.mdc
│   ├── 13_create_mvp_growth_iteration_plan.mdc
│   ├── 14_create_risk_contingency_plan.mdc
│   └── 15_create_mvp_tasks.mdc           # [NEW] Generates the foundational MVP task list
├── 02_feature/              # Ongoing feature development and task management
│   ├── create-prd.mdc
│   ├── generate-tasks.mdc
│   └── iterate-tasks.mdc                 # Updated to support iterating both PRD and MVP task lists
├── docs/                    # Generated documentation (product briefs, PRDs, etc.)
├── tasks/                   # Generated task lists for features and foundational setup
└── README.md                # This file
```

---

## Getting Started — Project Initiation

The `/01_start` directory contains a set of cursor rules (`.mdc`) that guide the AI through the foundational product documentation process. These are designed to be run sequentially to build out a full and well-rounded understanding of the product, market, users, and technical considerations.

### Step-by-Step Initiation Flow

For a new project, start by invoking the following cursor rules **in order**:

1. **Product Brief** – `@01_create_product_brief.mdc`
2. **Market Analysis** – `@02_create_market_analysis.mdc`
3. **User Personas** – `@03_create_user_personas.mdc`
4. **Features Document** – `@04_create_features_doc.mdc`
5. **User Flows and Diagrams** – `@05_create_user_flows_diagrams.mdc`
6. **UX & Design Considerations** – `@06_create_ux_design_doc.mdc`
7. **Content Strategy** – `@07_create_content_strategy.mdc`
8. **Architecture & System Design** – `@08_create_architecture_doc.mdc`
9. **Security** – `@09_create_security_doc.mdc`
10. **Testing & QA Strategy** – `@10_create_testing_doc.mdc`
11. **Performance Metrics & Analytics** – `@11_create_performance_doc.mdc`
12. **Success Metrics & KPIs** – `@12_create_success_metrics_kpis_doc.mdc`
13. **Post-MVP Growth & Iteration Plan** – `@13_create_mvp_growth_iteration_plan.mdc`
14. **Risk & Contingency Plan** – `@14_create_risk_contingency_plan.mdc`
15. **Create MVP Task List** – `@15_create_mvp_tasks.mdc`

    > Generate a high-level, comprehensive task list for bootstrapping the initial version of your product using insights from all prior documentation.

---

## Ongoing Feature Development (`/02_feature`)

Once the initial project foundation is established, new features can be defined, scoped, and tracked in `/02_feature` using the following workflow:

### 1. Creating a Product Requirements Document (PRD)

* Use `@create-prd.mdc` to generate a detailed PRD from your feature idea.

**Example syntax:**

```md
Use @create-prd.mdc
Here's the feature I want to build: [Describe your feature in detail]
```

* The AI will generate a structured PRD and save it to `/tasks/prd-[feature-name].md`.

### 2. Generating Task Lists from PRDs

* Generate implementation tasks from a PRD using:

```md
Now take @prd-[feature-name].md and create tasks using @generate-tasks.mdc
```

* The AI will:

  * Generate high-level tasks → Confirm
  * Expand each with detailed sub-tasks → Confirm again
  * Save to `tasks-prd-[feature-name].md`

### 3. Iterating Over Task Lists

* Start task execution with:

```md
Please start on task 1.1 and use @iterate-tasks.mdc
```

* The AI will:

  * Work one sub-task at a time
  * Mark tasks as completed
  * Track modified files
  * Pause after each sub-task for approval

* The same approach works for both **PRD-derived** and **MVP foundational** task lists, such as:

```md
Please start with MVP task 2.1 using @iterate-tasks.mdc
```

---

## How to Use the `.mdc` Rules

* Each `.mdc` rule defines an AI behavior pattern for generating docs, creating tasks, or iterating over progress.
* Run rules in order for project setup; invoke feature/task rules as needed during product development.
* Output files are stored in the `/docs` and `/tasks` directories for easy tracking and collaboration.

---

## Integrating Documentation Context

The AI constantly references project context from:

* **Product Brief**
* **User Personas**
* **Architecture & Design Docs**
* **Feature & User Flow Definitions**
* **Testing, Security, and KPI Plans**

This ensures every decision during implementation stays aligned with the original product vision and technical design.

---

## Contributing

Contributions are welcome! Please follow these guidelines:

* Ensure new `.mdc` files are purposeful, readable, and aligned with the workflow.
* Document any changes in this README and comment clearly in the rule file.
* Feel free to propose new rules for testing, analytics, devops, etc.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Thank you for using this toolkit!
Empower your team with AI-guided, structured, and maintainable product delivery workflows.

<!-- TODO: 
Smart workflow
1. sitemap/page goals
2. wireframe: define layout, sections, hierarchy, CTA placement
3. copywriting draft: written to fit the structure, mindful of spacing and hierarchy
4. wireframe refinement: adjust layout if needed based on copy
5. design -->