# Claude AI Test-Driven Development (TDD) Workflow

## Phase 1: Requirements Analysis & Test Planning
**When to use:** Before starting TDD cycles on new features or significant changes

```
Analyze the requirements and break them down into testable behaviors. Do not write any production code yet. We need to understand the expected functionality, edge cases, and acceptance criteria. Read through existing test patterns, testing utilities, and test structure conventions in this codebase. Identify existing testing patterns, naming conventions, and test organization strategies that should be followed. Prepare to discuss the test scenarios, test data requirements, and testing strategy for this feature.
```

## Phase 2: Test Design & Architecture Review
**When to use:** After requirements analysis, before writing the first failing test

```
Review this test design plan for completeness, maintainability, and alignment with testing best practices Check for proper test coverage of happy paths, edge cases, error conditions, and boundary values Flag any missing test scenarios, overly complex test setups, or unnecessary test complexity Suggest test optimizations that align with our existing test architecture and patterns Ensure proper test isolation, appropriate mocking strategies, and clear test intent are planned Validate that tests will provide meaningful feedback and guide implementation
```

## Phase 3: Red Phase - Write Failing Tests
**When to use:** When ready to write the first failing test in the TDD cycle

```
Write clean, focused failing tests that follow existing patterns and conventions in this codebase Do not add backwards compatibility unless explicitly requested Use proper test naming, implement appropriate test data setup, and ensure clear test assertions Focus on one specific behavior per test case and make the test intention crystal clear After each test, run it to confirm it fails for the right reasons and provides meaningful error messages Write descriptive test names that serve as living documentation of the expected behavior
```

## Phase 4: Green Phase - Minimal Implementation
**When to use:** After writing failing tests, implement just enough code to make them pass

```
Write the minimal production code needed to make the failing tests pass Do not over-engineer or add functionality not covered by tests Focus on making tests pass with the simplest possible implementation After each small code change, run tests to ensure they pass and no existing functionality is broken Avoid the temptation to add extra features or handle cases not yet covered by tests Keep the implementation focused and direct - optimize for passing tests, not perfect design yet
```

## Phase 5: Refactor Phase - Improve Design
**When to use:** After tests are passing, before moving to the next TDD cycle

```
Refactor both production code and test code while keeping all tests green following existing code patterns and architectural conventions Improve code design, eliminate duplication, and enhance readability without changing behavior After each refactoring step, run the full test suite to ensure nothing breaks Look for opportunities to extract methods, improve naming, and simplify complex logic Review the refactored code for any over-engineering - we're pre-customer, avoid unnecessary abstractions, unnecessary design patterns, or premature optimization Is this implementation overly complex? We are still pre-customer - any unnecessary interfaces, excessive abstraction, or design overkill in this? Prepare to start the next Red-Green-Refactor cycle for the next behavior
```