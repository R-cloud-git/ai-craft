https://github.com/R-cloud-git/ai-craft/releases

[![Release](https://img.shields.io/github/v/release/R-cloud-git/ai-craft?style=for-the-badge&label=Releases)](https://github.com/R-cloud-git/ai-craft/releases)

# ai-craft: Structured AI-Driven Workflows for Modern Software DevOps

![ai-craft banner](https://dummyimage.com/1200x420/0e7490/ffffff&text=ai-craft)

⚡ A practical library of structured prompts for software development with AI. It covers application development, infrastructure as code (IaC), CI/CD, configuration management, and test-driven development (TDD) practices. Use AI to plan, design, implement, test, and deploy software workflows with confidence.

This project brings together a curated set of prompts, templates, and workflow blueprints. It guides teams to use AI for repeatable, auditable software workflows. The prompts are designed to be used with Claude AI or similar AI assistants, but the structure works with other providers as well.

Topics: ai-workflows, ci-cd, claude-ai, development-workflows, devops, infrastructure-as-code, prompt-engineering, software-engineering, test-driven-development, workflows

Overview and goals
- Build reliable AI-assisted workflows for software teams.
- Combine best practices from DevOps, IaC, and TDD into a single prompt library.
- Help teams move from ad hoc prompts to repeatable, auditable workflows.
- Provide a path from idea to production with AI as a partner in the process.

Who should use ai-craft
- Software engineers who want AI help with design, implementation, and testing.
- DevOps engineers who need repeatable IaC and deployment prompts.
- QA engineers practicing TDD and automated testing with AI support.
- Team leads and architects who want consistent, auditable workflows.

How ai-craft is organized
- A core prompt library with templates for across-the-stack tasks.
- Domain-specific prompts for application development, IaC, CI/CD, configuration management, and TDD.
- Example workflows that show end-to-end usage from planning to validation.
- Clear guidance on how to adapt prompts to your tooling and environment.

Licensing and contribution
- The project uses an open license suitable for collaboration and reuse.
- Contributions are welcome. You’ll find guidelines in the contributed section.

Releases and distribution
- For access to the latest release assets, see the Releases page. If you have trouble, consult the Releases section for guidance.

Why this matters
- AI can accelerate software work when prompts are well-structured.
- Having a library of proven patterns reduces cognitive load and risk.
- Consistent prompts improve reproducibility, traceability, and auditability.

Quick start: how to begin with ai-craft
- Install and configure the prompt runner or CLI you prefer (Python, Node.js, or a bare prompt runner if you have one).
- Load the core prompt library into your AI assistant.
- Try a sample workflow to see how prompts guide planning, design, and validation.
- Tailor the prompts to your project, then save your customized workflows in your repo.

Key principles
- Clarity over cleverness. Prompts should be explicit about goals, constraints, and acceptance criteria.
- Modularity. Break prompts into reusable components tied to tasks.
- Traceability. Ensure outputs can be traced back to inputs and decisions.
- Safety and hygiene. Keep sensitive data out of prompts and ensure outputs are auditable.
- Adaptability. Prompts work across providers and environments with minimal changes.

Awesome features you’ll find
- Domain-driven prompt templates that echo real-world workflows.
- End-to-end templates for building software, configuring infrastructure, validating CI/CD pipelines, and enforcing TDD.
- Clear prompts for eliciting requirements, planning architecture, drafting code, generating tests, and validating deployments.
- A library layout you can extend with your own prompts and templates.
- Examples that illustrate how to chain prompts into coherent workflows.

What you’ll learn from ai-craft
- How to structure prompts for software engineering tasks.
- How to design AI-assisted workflows that align with your team’s processes.
- How to test AI-generated outputs as part of your QA process.
- How to integrate AI prompts into your CI/CD pipelines.

Table of contents
- About ai-craft
- Core concepts
- Getting started
- The prompt library
- Domain templates
- End-to-end workflows
- Architecture and structure
- How to customize
- Best practices
- Contributing
- Roadmap
- Help and support
- License

About ai-craft: core concepts
- Prompts as workflows: Each prompt is part of a larger workflow. A workflow is a sequence of prompts that moves a task from idea to validated output.
- Prompts with intent: Prompts carry clear goals, constraints, and acceptance criteria. They avoid ambiguity.
- Context management: Workflows preserve context across steps to maintain consistency.
- Roles and prompts: Different prompts simulate roles in a team (e.g., architect, developer, tester, reviewer).
- Checkpoints and validation: Each stage includes checks to ensure outputs meet quality gates.

Core components
- Prompt templates: Reusable blueprints you can customize.
- Workflow blueprints: End-to-end sequences that tie prompts together.
- Evaluation rubrics: Criteria to judge whether outputs meet standards.
- Asset pack: Supporting files like example prompts, data schemas, and configuration tips.

Domain prompts: detailed guidance
- Application development: prompts that guide requirements gathering, design decisions, API definitions, data models, and code generation with guardrails.
- IaC (Infrastructure as Code): prompts that plan infrastructure architecture, write IaC templates, validate configurations, and generate deployment scripts.
- CI/CD: prompts to define pipelines, quality gates, deployment strategies, rollback plans, and environment promotion rules.
- Configuration management: prompts for managing config across environments, secret handling, and parameterization.
- Test-driven development: prompts to draft tests, derive test cases from requirements, and validate behavior before coding.

Getting started: a practical path
- Prerequisites: A working AI assistant, a code editor, and access to your repository. It helps if you have Python 3.10+ or Node.js 18+ installed.
- Install the prompt runner or any preferred CLI: Follow the repository's setup guide, or use a language-agnostic runner if you already have one.
- Initialize ai-craft in your project: Create a local prompts directory and import the library.
- Load core prompts: Bring in the base templates that cover all five domains.
- Run a quick workflow: Try a starter task in your environment to see how the prompts flow together.

Install and setup
- Pick your environment: Python, Node, or a plain prompt runner.
- Install the library: Follow your chosen path (pip install, npm install, or equivalent).
- Configure the AI provider: Point to Claude AI or your preferred provider. Set model, temperature, and safety controls.
- Prepare data and environment: Gather sample requirements, infrastructure diagrams, and test suites to seed the prompts with context.
- Run a test: Execute a simple workflow to confirm end-to-end behavior.

Installation notes and minimal commands
- Python path (example): pip install ai-craft
- Node path (example): npm install -g ai-craft
- Quick init (example): ai-craft init
- Run a sample workflow (example): ai-craft run sample-app-dev

Quick start examples
- Example prompt flow: Planning → Design → Implementation → Tests → Deployment
- Design prompt: “Given the requirements, draft a software architecture with components, interactions, data flows, and non-functional requirements. Output an architectural diagram in Mermaid syntax.”
- Implementation prompt: “Generate a starter code scaffold for a microservice with REST API, including package structure, main modules, and stub tests.”
- Test prompt: “From the requirements, produce a test suite that validates core paths, error handling, and edge cases. Include unit and integration tests.”
- Deployment prompt: “Describe a CI/CD pipeline that builds, tests, and deploys the service to a cloud environment. Include steps for rollback and monitoring.”

The prompt library: structure and examples
- Directory layout
  - prompts/
    - app-development/
    - infrastructure/
    - ci-cd/
    - configuration-management/
    - tdd/
- File naming conventions
  - template-<domain>-<task>.md
  - example-<domain>-<task>.md
- How to write prompts
  - Start with the goal: What should the AI produce?
  - State constraints: tech stack, languages, tooling, environment.
  - Declare inputs: what data is needed?
  - Define outputs: code, docs, diagrams, tests, or configs.
  - Add validation: acceptance criteria and checks.
- Domain examples
  - Application development
    - Goal: Generate a scalable REST service scaffold with clean architecture.
    - Constraints: Python 3.11, FastAPI, Pydantic, tests included.
    - Inputs: API requirements, data models, auth scheme.
    - Outputs: code skeleton, tests, architecture diagram.
  - IaC
    - Goal: Produce a Terraform module to create a web app stack.
    - Constraints: AWS, VPC, subnets, security groups.
    - Outputs: Terraform code, deployment plan, notes.
  - CI/CD
    - Goal: Define a pipeline for a microservice.
    - Constraints: GitHub Actions, lint, unit tests, security scans.
    - Outputs: YAML file, explanation, test matrix.
  - Configuration management
    - Goal: Centralize app config across environments.
    - Constraints: Parameter store, secret management, environment parity.
    - Outputs: Helm values, Kubernetes manifests, docs.
  - TDD
    - Goal: Draft tests from user stories.
    - Constraints: Coverage target, mock strategy, test data.
    - Outputs: Test files, test data, run instructions.

End-to-end workflows: sample pipelines
- End-to-end app development workflow
  - Stage 1: Gather requirements with prompts that elicit success criteria.
  - Stage 2: Propose architecture and data models.
  - Stage 3: Produce scaffolded code and tests.
  - Stage 4: Validate by running tests and static analysis.
  - Stage 5: Prepare deployment artifacts and monitor health.
- End-to-end IaC workflow
  - Stage 1: Define infrastructure goals and constraints.
  - Stage 2: Generate IaC templates and validation scripts.
  - Stage 3: Run plan and apply steps with safety checks.
  - Stage 4: Validate resources and drift detection.
- End-to-end CI/CD workflow
  - Stage 1: Draft pipeline; define stages and gates.
  - Stage 2: Create tests, lint, and security checks.
  - Stage 3: Build, push, and deploy to staging.
  - Stage 4: Perform canaries and rollback if needed.
- End-to-end configuration management workflow
  - Stage 1: Centralize configuration; separate secrets from data.
  - Stage 2: Propagate config changes to environments.
  - Stage 3: Validate config integrity across stacks.
- End-to-end TDD workflow
  - Stage 1: Convert user stories to tests.
  - Stage 2: Generate minimal code to satisfy tests.
  - Stage 3: Refactor until tests pass and code is clean.
  - Stage 4: Expand test coverage and edge-case handling.

Architecture and repository layout
- root/
  - prompts/      Core templates and domain prompts
  - examples/     Real-world usage examples
  - docs/         Guides, tutorials, and best practices
  - tools/        Helper scripts and utilities
  - assets/       Imagery and branding assets
- What goes where
  - prompts/app-development/: Prompts for building software applications.
  - prompts/infrastructure/: IaC prompts and templates.
  - prompts/ci-cd/: CI/CD pipeline prompts and checks.
  - prompts/configuration-management/: Configuration prompts.
  - prompts/tdd/: Prompts centered on test-driven development.
  - examples/: Sample projects that demonstrate end-to-end workflows.

How ai-craft helps teams
- Reduces time to first MVP by providing ready-to-tune prompts.
- Improves consistency across teams by standardizing prompt patterns.
- Improves quality by embedding tests and validations in the workflow.
- Encourages safer AI usage with explicit constraints and acceptance criteria.
- Supports multiple AI providers with clear adapter points.

Usage patterns and best practices
- Start small: pick a single domain and a simple workflow.
- Incrementally add prompts: replace ad hoc prompts with organized templates.
- Capture decisions: document why a prompt produces a certain output.
- Align with governance: include security, compliance, and data handling notes.
- Collaborate: pair programmers with AI to review prompts and outputs.

Prompt design checklist
- Define the goal clearly.
- List constraints exhaustively.
- Specify inputs and outputs.
- Include acceptance criteria.
- Add guardrails to avoid leakage of sensitive data.
- Provide examples of expected outputs.
- Include a validation step.

Advanced tips for the power user
- Layer prompts: combine small prompts into a larger workflow.
- Use role prompts: simulate team roles to diversify perspectives.
- Customize per project: create per-project cabinets of prompts and templates.
- Integrate with your tooling: connect with IDEs, CI systems, or chat interfaces.
- Audit and version: track changes to prompts and decisions.

Prompts: sample templates (snippets)
- Architecture planning prompt (example)
  - Goal: Produce a high-level architecture with components, data flows, and non-functional requirements.
  - Constraints: Microservices, domain-driven design, event-driven where appropriate.
  - Inputs: User stories, non-functional requirements, tech stack.
  - Output: Architecture diagram in Mermaid, a component list, and rationale.
  - Validation: Ensure modules have defined interfaces and data contracts.
- Code scaffold prompt (example)
  - Goal: Generate a scaffold for a service in a chosen language.
  - Constraints: Clean architecture, tests included, CI hooks.
  - Outputs: Project skeleton, package manifest, sample tests.
- Test generation prompt (example)
  - Goal: Create tests from user stories.
  - Constraints: Coverage targets, edge cases, deterministic tests.
  - Outputs: Tests in chosen framework, data providers, and mocks.

Prompt examples by domain (snippets)
- Application development: 
  - Task: Scaffold REST service in Python with FastAPI.
  - Output: main.py, models.py, schemas.py, routes.py, tests/test_main.py, Dockerfile, and a README with usage.
- IaC:
  - Task: Create a Terraform module for a web app on AWS.
  - Output: modules/web-app/main.tf, variables.tf, outputs.tf, and a deployment guide.
- CI/CD:
  - Task: Build a GitHub Actions pipeline for a Node.js microservice.
  - Output: .github/workflows/ci-cd.yml plus a README explaining each job.
- Configuration management:
  - Task: Centralize config across environments with parameter store.
  - Output: Helm values, Kubernetes manifests, and a migration plan.
- TDD:
  - Task: Draft tests for a new feature based on user stories.
  - Output: test files, test data, and a run script.

Integrations and providers
- Claude AI compatibility: ai-craft is designed to work with Claude AI and similar assistants. You can adapt prompts to suit the capabilities of your preferred provider.
- Model-agnostic design: The structure emphasizes intent, constraints, and validation rather than vendor-specific features.
- Safety and privacy: Avoid handling secrets in prompts. Use environment-secured inputs and keep credentials out of the prompt context.

Contributing: how to help
- See the contributing guide for how to propose changes.
- Share new prompts and templates that follow the same structure.
- Improve example workflows with real-world scenarios.
- Update documentation with audience-focused guides and tutorials.

Roadmap
- Expand domain coverage to include more DevOps practices.
- Improve prompt orchestration with more robust validation hooks.
- Add richer example projects and case studies.
- Develop a visual editor for composing workflows.
- Integrate with additional AI providers beyond Claude AI.

Support and community
- For questions, issues, and discussions, use the project's issue tracker.
- Join discussions on best practices for AI-assisted software development.
- Share your own workflows and templates to contribute to the growing library.

License
- ai-craft is released under the MIT License. See the LICENSE file for details.

Releases and updating
- The Releases page hosts downloadable assets and release notes. If you run into issues with the link, consult the Releases section for alternatives and troubleshooting steps. For easy access, revisit the Releases page to find the most recent assets and instructions.

Appendix: sample workflow run log (illustrative)
- Step 1: Capture requirements
  - Prompt: “List user stories and acceptance criteria for the feature X.”
  - AI response: A concise set of user stories and acceptance criteria.
- Step 2: Design
  - Prompt: “Propose a software architecture with modules, data models, and interfaces.”
  - AI response: Architecture diagram and rationale.
- Step 3: Implementation
  - Prompt: “Generate a scaffold with code structure and tests.”
  - AI response: Code skeleton and tests.
- Step 4: Validation
  - Prompt: “Run tests and report results; propose improvements.”
  - AI response: Test results, issues found, recommended fixes.
- Step 5: Deployment
  - Prompt: “Describe a safe deployment plan with rollback.”
  - AI response: Deployment steps and rollback plan.

Note: This document presents an extensive, practical guide to ai-craft. It emphasizes a gardener’s approach: plant prompts, prune outputs, and cultivate reliable AI-assisted workflows that fit real-world software development. The content is designed to be useful in teams adopting AI as a collaborative tool, not a magic wand.