# Claude AI Configuration Management Development Workflow

## Phase 1: Configuration Analysis & Environment Review
**When to use:** Before implementing new configuration systems or modifying existing config management

```
- Analyze the existing configuration setup and environment management.
- Do not write any configuration code yet.
- Understand current config structure, environment variables, and secrets management.
- Read through existing config files, environment templates, and secrets systems.
- Identify existing patterns, naming conventions, and configuration strategies.
- Prepare to discuss current configuration architecture and potential improvements.
```

## Phase 2: Security & Configuration Strategy Review
**When to use:** After analyzing current setup, before implementation begins

```
- Review the configuration management plan for security best practices.
- Check for proper secrets handling and environment variable management.
- Verify configuration validation and access controls.
- Flag any security vulnerabilities or configuration drift risks.
- Suggest optimizations aligned with deployment workflow and security requirements.
- Ensure proper separation of secrets from code and appropriate encryption.
```

## Phase 3: Configuration Implementation & Best Practices
**When to use:** When ready to write production-ready configuration management code

```
- Write clean, secure configuration management code following existing patterns.
- Do not add backwards compatibility unless explicitly requested.
- Use proper configuration hierarchies and implement appropriate validation strategies.
- Ensure environment consistency and proper secret handling.
- Include environment variable definitions and feature flag management.
- Implement configuration validation and drift detection mechanisms.
- After each configuration block, validate syntax and check for security issues.
```

## Phase 4: Configuration Testing & Validation
**When to use:** After configuration code is written and needs comprehensive testing

```
- Test the configuration management setup thoroughly across all environments.
- Validate that configurations load correctly and secrets are properly handled.
- Test configuration rollback scenarios and secret rotation procedures.
- Run security scans on configuration files and validate access controls.
- Ensure proper monitoring, change tracking, and audit logging systems work.
- Check for configuration bloat and suggest optimizations for simpler management.
```

## Phase 5: Configuration Deployment & Documentation
**When to use:** When finalizing configuration setup and preparing for team adoption

```
- Deploy the configuration management system following existing deployment patterns.
- Create comprehensive documentation including schemas and setup guides.
- Set up proper monitoring, alerting, and change tracking for configuration health.
- Include runbooks for configuration updates, secret rotation, and environment provisioning.
- Document configuration update processes, approval workflows, and rollback procedures.
- Review for over-engineering - avoid unnecessary complexity for pre-customer stage.
- Check for unnecessary environment segregation, excessive validation, or configuration redundancy.
```