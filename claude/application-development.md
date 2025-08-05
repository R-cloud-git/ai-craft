# Claude AI Development Workflow Prompts

## Phase 1: Initial Analysis & Preparation
**When to use:** At the start of a new feature or when diving into an existing codebase section

```
Prepare to discuss. Read through related code. Do not write any code right now. We are going to work on the document identification part of the app. Dig in, read relevant files, and prepare to discuss the ins and outs of how it works. Use /resume to reuse that context.
```

## Phase 2: Plan Review & Architecture Feedback  
**When to use:** After a developer has created a technical plan or design document

```
My dev wrote up this plan, give me feedback on it - high level and down to the nitty gritty How can we improve it ? Are there any big architectural changes we should make ?
```

## Phase 3: Implementation & Development
**When to use:** When ready to write production code with quality standards

```
Now think hard and write elegant code that completes this Do not add backwards compatibility unless explicitly requested After every code block you write, lint compile and write corresponding tests and run them before writing the next code block
```

## Phase 4: Code Review
**When to use:** After code has been written and needs comprehensive review

```
Review the code my developer just wrote, give high level feedback and low level feedback, make it one solid code review that when they go and fix it all you shouldn't have any more feedback to give
```

## Phase 5: Pull Request & Handoff
**When to use:** When finalizing work and preparing for team collaboration

```
Create this pull request Once you've completed it, look at the next pull request in this project Someone else will be working on it Give the next developer some advice to help them accomplish the next PR in the markdown file Is this implementation overly complex? We are still pre-customer - any unnecessary fallbacks unnecessary versioning testing overkill in this?
```