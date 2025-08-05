# Claude AI Development Workflow Prompts

## Phase 1: Initial Analysis & Preparation
**When to use:** At the start of a new feature or when diving into an existing codebase section

```
- Prepare to discuss. Read through related code. 
- Do not write any code right now. 
- We are going to work on the document identification part of the app. 
- Dig in, read relevant files, and prepare to discuss the ins and outs of how it works. 
- Use /resume to reuse that context.
```

## Phase 2: Plan Review & Architecture Feedback  
**When to use:** After a developer has created a technical plan or design document

```
- Review the technical plan provided by the developer.
- Give both high-level and detailed feedback.
- Identify potential improvements and architectural changes.
- Focus on scalability, maintainability, and best practices.
- Suggest specific improvements without implementing them yet.
```

## Phase 3: Implementation & Development
**When to use:** When ready to write production code with quality standards

```
- Think carefully and write elegant, production-ready code.
- Do not add backwards compatibility unless explicitly requested.
- After every code block, lint and compile the code.
- Write corresponding tests for each code block.
- Run tests before writing the next code block.
- Focus on clean, maintainable implementation.
```

## Phase 4: Code Review
**When to use:** After code has been written and needs comprehensive review

```
- Review the code written by the developer thoroughly.
- Provide both high-level and low-level feedback.
- Make it a comprehensive code review.
- Ensure all feedback is actionable and complete.
- Focus on code quality, security, and maintainability.
- Aim to provide feedback that eliminates the need for follow-up reviews.
```

## Phase 5: Pull Request & Handoff
**When to use:** When finalizing work and preparing for team collaboration

```
- Create the pull request with proper documentation.
- Once completed, review the next pull request in the project.
- Provide advice to help the next developer accomplish their task.
- Evaluate if the implementation is overly complex for pre-customer stage.
- Check for unnecessary fallbacks, versioning, or testing overkill.
- Focus on simplicity and essential functionality.
```