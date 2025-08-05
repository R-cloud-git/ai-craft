# Claude AI Configuration Management Development Workflow

## Phase 1: Configuration Analysis & Environment Review
**When to use:** Before implementing new configuration systems or modifying existing config management

```
Analyze the existing configuration setup and environment management. Do not write any configuration code yet. We need to understand the current config structure, environment variables, secrets management, and deployment configurations. Read through existing config files, environment templates, and secrets management systems. Identify existing patterns, naming conventions, hierarchies, and configuration strategies that should be followed. Prepare to discuss the current configuration architecture, environment parity issues, and potential improvements.
```

## Phase 2: Security & Configuration Strategy Review
**When to use:** After analyzing current setup, before implementation begins

```
Review this configuration management plan for security best practices, environment consistency, and maintainability Check for proper secrets handling, environment variable management, configuration validation, and access controls Flag any security vulnerabilities, configuration drift risks, or unnecessary complexity Suggest configuration optimizations that align with our deployment workflow and security requirements Ensure proper separation of secrets from code, appropriate encryption, and audit logging capabilities are planned
```

## Phase 3: Configuration Implementation & Best Practices
**When to use:** When ready to write production-ready configuration management code

```
Write clean, secure configuration management code that follows existing patterns and conventions in this codebase Do not add backwards compatibility unless explicitly requested Use proper configuration hierarchies, implement appropriate validation strategies, and ensure environment consistency After each configuration block, validate syntax, check for security misconfigurations, and ensure proper secret handling Include proper environment variable definitions, feature flag management, and configuration templating Implement configuration validation and drift detection mechanisms
```

## Phase 4: Configuration Testing & Validation
**When to use:** After configuration code is written and needs comprehensive testing

```
Test this configuration management setup thoroughly including environment validation, secrets handling, and deployment scenarios Validate that configurations load correctly across all environments, secrets are properly encrypted and accessible, and environment parity is maintained Test configuration rollback scenarios, secret rotation procedures, and configuration drift detection Run security scans on configuration files and validate access controls Ensure proper configuration monitoring, change tracking, and audit logging systems are working Check for configuration bloat and suggest optimizations for simpler management
```

## Phase 5: Configuration Deployment & Documentation
**When to use:** When finalizing configuration setup and preparing for team adoption

```
Deploy the configuration management system following existing deployment patterns and create comprehensive documentation including configuration schemas, environment setup guides, and troubleshooting procedures Set up proper monitoring, alerting, and change tracking for configuration health Include runbooks for configuration updates, secret rotation, and environment provisioning Review the configuration system for any over-engineering - we're pre-customer, avoid unnecessary complexity, unnecessary environment variations, unnecessary secret versioning, or configuration overkill Document the configuration update processes, approval workflows, and rollback procedures for the team Is this configuration management overly complex? We are still pre-customer - any unnecessary environment segregation, excessive validation, or configuration redundancy in this?
```