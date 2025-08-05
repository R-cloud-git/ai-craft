# Claude AI CI/CD Pipeline Development Workflow

## Phase 1: Pipeline Analysis & Requirements
**When to use:** Before creating new pipelines or modifying existing CI/CD workflows

```
Analyze the existing CI/CD setup and build requirements. Do not write any pipeline code yet. We need to understand the current build processes, deployment strategies, and workflow patterns. Read through existing GitHub Actions, Jenkins, GitLab CI, and Azure DevOps configurations to understand the job dependencies, artifact flows, and deployment stages. Identify existing patterns, naming conventions, and workflow structures that should be followed. Prepare to discuss the current pipeline architecture and potential improvements.
```

## Phase 2: Pipeline Strategy & Security Review
**When to use:** After analyzing requirements, before implementation begins

```
Review this CI/CD pipeline plan for security best practices, efficiency, and maintainability Check for proper secret management, secure artifact handling, appropriate permissions, and security scanning integration Flag any security vulnerabilities, inefficient build steps, or unnecessary complexity Suggest pipeline optimizations that align with our development workflow and deployment requirements Ensure proper branch protection, approval processes, and rollback capabilities are planned
```

## Phase 3: Pipeline Implementation & Best Practices
**When to use:** When ready to write production-ready pipeline configurations

```
Write clean, efficient pipeline code that follows existing patterns and conventions in this codebase Do not add backwards compatibility unless explicitly requested Use proper job naming, implement appropriate caching strategies, and ensure proper job dependencies After each pipeline stage, validate syntax, check for security misconfigurations, and ensure proper artifact management Include proper environment variable handling, secret management, and conditional logic Implement fail-fast strategies and appropriate retry mechanisms
```

## Phase 4: Pipeline Testing & Validation
**When to use:** After pipeline code is written and needs comprehensive testing

```
Test this CI/CD pipeline thoroughly including build validation, deployment testing, and failure scenarios Validate that all stages execute correctly, artifacts are properly generated and stored, and deployments work as expected Test pipeline security controls, permission boundaries, and secret handling Run the pipeline against different scenarios including feature branches, hotfixes, and rollback situations Ensure proper monitoring, logging, and notification systems are working Check build times and suggest optimizations for faster feedback loops
```

## Phase 5: Pipeline Deployment & Documentation  
**When to use:** When finalizing pipeline setup and preparing for team adoption

```
Deploy the CI/CD pipeline following existing deployment patterns and create comprehensive documentation including workflow diagrams, troubleshooting guides, and operational procedures Set up proper monitoring, alerting, and metrics collection for pipeline health Include runbooks for common pipeline failures and recovery procedures Review the pipeline for any over-engineering - we're pre-customer, avoid unnecessary complexity, unnecessary fallbacks, unnecessary versioning, or testing overkill Document the pipeline triggers, approval processes, and rollback procedures for the team Is this pipeline overly complex? We are still pre-customer - any unnecessary redundancy, excessive parallelization, or testing overkill in this?
```