# Claude AI Infrastructure as Code (IaC) Development Workflow

## Phase 1: Infrastructure Analysis & Planning
**When to use:** Before designing new infrastructure or modifying existing resources

```
- Analyze the existing infrastructure setup and requirements.
- Do not write any IaC code yet.
- Understand the current architecture, dependencies, and constraints.
- Read through existing Terraform/CloudFormation/Pulumi files.
- Understand resource relationships, networking, and security configurations.
- Identify existing patterns, naming conventions, and architectural decisions.
- Prepare to discuss infrastructure design patterns and potential improvements.
```

## Phase 2: Security & Compliance Review
**When to use:** After initial analysis, before implementation begins

```
- Review the infrastructure plan for security best practices and compliance.
- Check for proper IAM policies, network segmentation, and encryption.
- Verify backup strategies and monitoring coverage.
- Flag any security vulnerabilities, compliance gaps, or cost inefficiencies.
- Suggest architectural improvements aligned with cloud security frameworks.
- Ensure alignment with organizational policies and requirements.
```

## Phase 3: IaC Implementation & Best Practices
**When to use:** When ready to write production-ready infrastructure code

```
- Write clean, modular, and maintainable IaC code following existing patterns.
- Do not add backwards compatibility unless explicitly requested.
- Use proper resource naming conventions and implement appropriate tagging strategies.
- Ensure idempotency and proper resource dependencies.
- Write corresponding variable definitions and output values.
- Include provider version constraints and backend configuration.
- After each resource block, validate syntax and check for security misconfigurations.
```

## Phase 4: Testing & Validation
**When to use:** After IaC code is written and needs comprehensive testing

```
- Create comprehensive tests including unit tests, integration tests, and security policy tests.
- Validate the plan output and check for any breaking changes or resource recreation.
- Review resource costs and suggest optimizations.
- Run security scanning tools and compliance checks.
- Ensure proper state management and backup procedures are in place.
- Test disaster recovery and rollback scenarios.
```

## Phase 5: Deployment Strategy & Documentation
**When to use:** When preparing for deployment and team handoff

```
- Create a deployment strategy with proper CI/CD pipeline integration.
- Generate comprehensive documentation including architecture diagrams and runbooks.
- Set up monitoring, alerting, and logging for the infrastructure.
- Plan for blue-green or canary deployments where appropriate.
- Include rollback procedures and disaster recovery plans.
- Document access patterns and operational procedures for the team.
- Review for over-engineering - avoid unnecessary complexity for pre-customer stage.
- Check for unnecessary redundancy or testing overkill.
```