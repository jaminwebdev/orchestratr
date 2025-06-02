# Product Development Automation Toolkit

Welcome to the **Product Development Automation Toolkit** — a structured, AI-assisted workflow for managing product documentation, feature development, and task iteration using markdown cursor rules (`.mdc` files).

This repo is designed to streamline and standardize the entire product lifecycle, from initial concept to post-MVP growth, by guiding AI-powered interactions to generate and maintain critical documentation, product requirements, task lists, and implementation progress — all version controlled in Markdown.

---

## Table of Contents

- [Project Structure](#project-structure)
- [Getting Started — Project Initiation](#getting-started--project-initiation)
- [Ongoing Feature Development](#ongoing-feature-development)
- [Task Iteration and Completion](#task-iteration-and-completion)
- [How to Use the `.mdc` Rules](#how-to-use-the-mdc-rules)
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
│   └── 14_create_risk_contingency_plan.mdc
├── 02_feature/              # Ongoing feature development and task management
│   ├── create-prd.mdc
│   ├── generate-tasks.mdc
│   └── iterate-tasks.mdc
├── docs/                    # Generated documentation (product briefs, PRDs, etc.)
├── tasks/                   # Generated task lists for features
└── README.md                # This file
````

---

## Getting Started — Project Initiation

The `/01_start` directory contains a set of cursor rules (`.mdc`) that guide the AI through the foundational product documentation process. These are designed to be run sequentially to build out a full and well-rounded understanding of the product, market, users, and technical considerations.

### Step-by-Step Initiation Flow

For a new project, start by invoking the following cursor rules **in order**:

1. **Product Brief**
   Use `@01_create_product_brief.mdc`
   Kick off by defining the product’s core idea, goals, target users, and key value proposition.

2. **Market Analysis**
   Use `@02_create_market_analysis.mdc`
   Analyze market conditions, competitors, trends, and opportunities.

3. **User Personas**
   Use `@03_create_user_personas.mdc`
   Define detailed user personas, their needs, motivations, and pain points.

4. **Features Document**
   Use `@04_create_features_doc.mdc`
   Outline the core features and functionalities planned for the product.

5. **User Flows and Diagrams**
   Use `@05_create_user_flows_diagrams.mdc`
   Map out key user journeys and flow diagrams for the product.

6. **UX & Design Considerations**
   Use `@06_create_ux_design_doc.mdc`
   Specify design principles, UI guidelines, and interaction details.

7. **Content Strategy**
   Use `@07_create_content_strategy.mdc`
   Plan content needs, voice, and messaging frameworks.

8. **Architecture & System Design**
   Use `@08_create_architecture_doc.mdc`
   Define the high-level system architecture, tech stack, and infrastructure.

9. **Security**
   Use `@09_create_security_doc.mdc`
   Document security requirements, compliance, and best practices.

10. **Testing & QA Strategy**
    Use `@10_create_testing_doc.mdc`
    Plan testing approaches, quality assurance, and validation processes.

11. **Performance Metrics & Analytics**
    Use `@11_create_performance_doc.mdc`
    Define performance goals, monitoring, and analytics requirements.

12. **Success Metrics & KPIs**
    Use `@12_create_success_metrics_kpis_doc.mdc`
    Establish measurable success criteria and key performance indicators.

13. **Post-MVP Growth & Iteration Plan**
    Use `@13_create_mvp_growth_iteration_plan.mdc`
    Outline strategies for growth, feedback loops, and iterative improvements.

14. **Risk & Contingency Plan**
    Use `@14_create_risk_contingency_plan.mdc`
    Identify risks, mitigation plans, and fallback strategies.

> **Note:** Each step builds on previous documents. Together, they form a comprehensive, living foundation for your product.

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

* The AI will ask clarifying questions before generating a PRD with:

  * Introduction
  * Goals
  * User Stories
  * Functional Requirements
  * Non-Goals
  * Design & Technical Considerations
  * Success Metrics
  * Open Questions

* The PRD will be saved as `prd-[feature-name].md` in `/tasks/`.

### 2. Generating Task Lists from PRDs

* After your PRD is created, generate implementation tasks with:

```md
Now take @prd-[feature-name].md and create tasks using @generate-tasks.mdc
```

* The AI will produce high-level parent tasks first and ask for confirmation.
* Upon confirmation (“Go”), it will generate detailed sub-tasks.
* The task list will be saved as `tasks-prd-[feature-name].md`.

### 3. Iterating Over Task Lists

* Begin work on tasks by invoking:

```md
Please start on task 1.1 and use @iterate-tasks.mdc
```

* The AI will:

  * Work on one sub-task at a time.
  * Mark tasks/sub-tasks complete as it progresses.
  * Update the “Relevant Files” list.
  * Pause after each sub-task for your approval before continuing.
* You can pause and resume by specifying the task number, e.g.:

```md
Please proceed with task 3.2 and use @iterate-tasks.mdc
```

---

## How to Use the `.mdc` Rules

* These cursor rules guide AI agents to generate or manage content dynamically.
* Each `.mdc` file contains instructions, clarifying questions, and expected outputs.
* The AI uses them to produce consistent, well-structured markdown docs or manage task progress.
* Run them in the order described for project initiation.
* Use feature creation and task management rules for ongoing work.

---

## Integrating Documentation Context

Throughout feature creation and task iteration, AI references all foundational docs:

* Product Brief
* Market Analysis
* User Personas
* Feature Specifications
* User Flows
* Architecture & Security Docs
* Testing & Performance Plans

This ensures that feature development aligns with the product vision, system architecture, user needs, and quality standards.

---

## Contributing

Contributions are welcome! Please follow these guidelines:

* When adding or modifying `.mdc` rules, ensure they fit into the existing workflow and maintain clarity.
* Update the README accordingly if you introduce new steps or directories.
* Document any changes or enhancements thoroughly.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Thank you for using the Product Development Automation Toolkit!
Empower your team with AI-guided, structured, and maintainable product delivery workflows.

