# Claude AI Test-Driven Development (TDD) Workflow

## Phase 1: Requirements Analysis & Test Planning
**When to use:** Before starting TDD cycles on new features or significant changes

```
- Analyze the requirements and break them down into testable behaviors.
- Do not write any production code yet.
- Understand expected functionality, edge cases, and acceptance criteria.
- Read through existing test patterns, testing utilities, and test structure conventions.
- Identify existing testing patterns, naming conventions, and test organization strategies.
- Prepare to discuss test scenarios, test data requirements, and testing strategy.
```

## Phase 2: Test Design & Architecture Review
**When to use:** After requirements analysis, before writing the first failing test

```
- Review the test design plan for completeness and maintainability.
- Check for proper test coverage of happy paths, edge cases, and error conditions.
- Flag any missing test scenarios or overly complex test setups.
- Suggest test optimizations aligned with existing test architecture.
- Ensure proper test isolation and appropriate mocking strategies.
- Validate that tests will provide meaningful feedback and guide implementation.
```

## Phase 3: Red Phase - Write Failing Tests
**When to use:** When ready to write the first failing test in the TDD cycle

```
- Write clean, focused failing tests following existing patterns and conventions.
- Do not add backwards compatibility unless explicitly requested.
- Use proper test naming and implement appropriate test data setup.
- Ensure clear test assertions and focus on one specific behavior per test.
- Make the test intention crystal clear with descriptive names.
- After each test, run it to confirm it fails for the right reasons.
- Ensure tests provide meaningful error messages.
```

## Phase 4: Green Phase - Minimal Implementation
**When to use:** After writing failing tests, implement just enough code to make them pass

```
- Write the minimal production code needed to make the failing tests pass.
- Do not over-engineer or add functionality not covered by tests.
- Focus on making tests pass with the simplest possible implementation.
- After each small code change, run tests to ensure they pass.
- Ensure no existing functionality is broken.
- Avoid adding extra features or handling cases not yet covered by tests.
- Keep implementation focused and direct - optimize for passing tests, not perfect design.
```

## Phase 5: Refactor Phase - Improve Design
**When to use:** After tests are passing, before moving to the next TDD cycle

```
- Refactor both production code and test code while keeping all tests green.
- Follow existing code patterns and architectural conventions.
- Improve code design, eliminate duplication, and enhance readability without changing behavior.
- After each refactoring step, run the full test suite to ensure nothing breaks.
- Look for opportunities to extract methods, improve naming, and simplify complex logic.
- Review for over-engineering - avoid unnecessary abstractions for pre-customer stage.
- Check for unnecessary interfaces, excessive abstraction, or design overkill.
- Prepare to start the next Red-Green-Refactor cycle for the next behavior.
```