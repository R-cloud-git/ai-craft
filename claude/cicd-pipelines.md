# Claude AI CI/CD Pipeline Development Workflow

## Phase 1: Pipeline Analysis & Requirements
**When to use:** Before creating new pipelines or modifying existing CI/CD workflows

```
- Analyze the existing CI/CD setup and build requirements.
- Do not write any pipeline code yet.
- Understand current build processes, deployment strategies, and workflow patterns.
- Read through existing GitHub Actions, Jenkins, GitLab CI, and Azure DevOps configurations.
- Identify job dependencies, artifact flows, and deployment stages.
- Note existing patterns, naming conventions, and workflow structures.
- Prepare to discuss current pipeline architecture and potential improvements.
```

## Phase 2: Pipeline Strategy & Security Review
**When to use:** After analyzing requirements, before implementation begins

```
- Review the CI/CD pipeline plan for security best practices and efficiency.
- Check for proper secret management and secure artifact handling.
- Verify appropriate permissions and security scanning integration.
- Flag any security vulnerabilities or inefficient build steps.
- Suggest pipeline optimizations aligned with development workflow.
- Ensure proper branch protection, approval processes, and rollback capabilities.
```

## Phase 3: Pipeline Implementation & Best Practices
**When to use:** When ready to write production-ready pipeline configurations

```
- Write clean, efficient pipeline code following existing patterns.
- Do not add backwards compatibility unless explicitly requested.
- Use proper job naming and implement appropriate caching strategies.
- Ensure proper job dependencies and artifact management.
- Include proper environment variable handling and secret management.
- Implement fail-fast strategies and appropriate retry mechanisms.
- After each pipeline stage, validate syntax and check for security issues.
```

## Phase 4: Pipeline Testing & Validation
**When to use:** After pipeline code is written and needs comprehensive testing

```
- Test the CI/CD pipeline thoroughly including build validation and deployment testing.
- Validate that all stages execute correctly and artifacts are properly managed.
- Test pipeline security controls, permission boundaries, and secret handling.
- Run pipeline against different scenarios including feature branches and hotfixes.
- Ensure proper monitoring, logging, and notification systems are working.
- Check build times and suggest optimizations for faster feedback loops.
```

## Phase 5: Pipeline Deployment & Documentation  
**When to use:** When finalizing pipeline setup and preparing for team adoption

```
- Deploy the CI/CD pipeline following existing deployment patterns.
- Create comprehensive documentation including workflow diagrams and troubleshooting guides.
- Set up proper monitoring, alerting, and metrics collection for pipeline health.
- Include runbooks for common pipeline failures and recovery procedures.
- Document pipeline triggers, approval processes, and rollback procedures.
- Review for over-engineering - avoid unnecessary complexity for pre-customer stage.
- Check for unnecessary redundancy, excessive parallelization, or testing overkill.
```