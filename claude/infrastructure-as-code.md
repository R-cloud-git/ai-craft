# Claude AI Infrastructure as Code (IaC) Development Workflow

## Phase 1: Infrastructure Analysis & Planning
**When to use:** Before designing new infrastructure or modifying existing resources

```
Analyze the existing infrastructure setup and requirements. Do not write any IaC code yet. We need to understand the current architecture, dependencies, and constraints. Read through the existing Terraform/CloudFormation/Pulumi files and understand the resource relationships, networking, and security configurations. Identify existing patterns, naming conventions, and architectural decisions that should be followed. Prepare to discuss the infrastructure design patterns and potential improvements.
```

## Phase 2: Security & Compliance Review
**When to use:** After initial analysis, before implementation begins

```
Review this infrastructure plan for security best practices, compliance requirements, and cost optimization opportunities Check for proper IAM policies, network segmentation, encryption at rest and in transit, backup strategies, and monitoring coverage Flag any security vulnerabilities, compliance gaps, or cost inefficiencies Suggest architectural improvements that align with cloud security frameworks and our organization's policies
```

## Phase 3: IaC Implementation & Best Practices
**When to use:** When ready to write production-ready infrastructure code

```
Write clean, modular, and maintainable IaC code that follows existing patterns and conventions in this codebase Do not add backwards compatibility unless explicitly requested Use proper resource naming conventions, implement appropriate tagging strategies, and ensure idempotency After each resource block, validate syntax, check for security misconfigurations, and ensure proper resource dependencies Write corresponding variable definitions and output values Include provider version constraints and backend configuration
```

## Phase 4: Testing & Validation
**When to use:** After IaC code is written and needs comprehensive testing

```
Create comprehensive tests for this infrastructure code including unit tests, integration tests, and security policy tests Validate the plan output, check for any breaking changes or resource recreation Review resource costs and suggest optimizations Run security scanning tools and compliance checks Ensure proper state management and backup procedures are in place Test disaster recovery and rollback scenarios
```

## Phase 5: Deployment Strategy & Documentation
**When to use:** When preparing for deployment and team handoff

```
Create a deployment strategy with proper CI/CD pipeline integration following existing deployment patterns Generate comprehensive documentation including architecture diagrams, runbooks, and troubleshooting guides Set up monitoring, alerting, and logging for the infrastructure Plan for blue-green or canary deployments where appropriate Include rollback procedures and disaster recovery plans Review the deployment for any over-engineering - we're pre-production, avoid unnecessary complexity, unnecessary fallbacks, unnecessary versioning, or premature optimization Document access patterns and operational procedures for the team Is this infrastructure overly complex? We are still pre-customer - any unnecessary redundancy or testing overkill in this?
```