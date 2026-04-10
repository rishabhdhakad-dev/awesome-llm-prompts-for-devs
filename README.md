# awesome-llm-prompts-for-devs

[![Version](https://img.shields.io/badge/version-v1.1.0-blue.svg)](#)

[![Stars](https://img.shields.io/github/stars/rishabhdhakad-dev/awesome-llm-prompts-for-devs?style=social)](https://github.com/rishabhdhakad-dev/awesome-llm-prompts-for-devs)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Contributors](https://img.shields.io/github/contributors/rishabhdhakad-dev/awesome-llm-prompts-for-devs)](https://github.com/rishabhdhakad-dev/awesome-llm-prompts-for-devs/graphs/contributors)

An awesome-list style collection of 500+ LLM prompts for developers.

Use this repository to accelerate code review, debugging, architecture planning, testing, security analysis, documentation, refactoring, DevOps, Git workflows, API design, Bash scripting, SQL work, data science, machine learning, and interview preparation. Every prompt is written to be practical, reusable, and easy to adapt to your stack.

Version: `v1.1.0`

**GitHub topics:** `llm`, `prompts`, `chatgpt`, `claude`, `developer-tools`, `awesome-list`, `ai`, `productivity`

## Table of Contents

- [Quick Start](#quick-start)
- [Categories](#categories)
- [Top 10 Most Useful Prompts](#top-10-most-useful-prompts)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [Star History](#star-history)
- [License](#license)

## Quick Start

Copy, paste, and replace the placeholders:

```text
Act as a senior engineer. Review the following code and tell me what is broken, risky, or unclear:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Framework: [FRAMEWORK]
- Goal: [GOAL]

Output format:
1. Summary
2. Issues ranked by severity
3. Suggested fixes
4. Final recommendation
```

You can keep these prompts as plain text, drop them into ChatGPT or Claude, or turn them into snippets in VS Code.

## Categories

| Category | Focus | Prompt Count | Best For |
| --- | --- | ---: | --- |
| code-review | PR review, quality checks, risk detection | 8 | Faster, sharper reviews |
| debugging | Root cause analysis, stack trace analysis, prod issues | 8 | Finding bugs quickly |
| architecture | System design and tradeoff analysis | 8 | Planning scalable systems |
| documentation | Docs, READMEs, onboarding, ADRs | 6 | Clear communication |
| testing | Unit, integration, E2E, load testing | 8 | Safer releases |
| security | OWASP, auth, secrets, dependency review | 8 | Risk reduction |
| api-design | REST, GraphQL, webhooks, versioning | 6 | Consistent interfaces |
| refactoring | Clean code, modernization, simplification | 6 | Maintainable codebases |
| devops | Containers, CI/CD, deploys, observability | 6 | Reliable delivery |
| git | Commits, PRs, branching, conflict resolution | 6 | Cleaner workflow |
| bash-scripting | Shell automation, cron, text processing | 5 | Safe shell workflows |
| sql-queries | Query writing, optimization, reporting | 5 | Database work |
| data-science | EDA, experiments, dashboards | 5 | Analysis and insights |
| machine-learning | Modeling, training, evaluation, inference | 5 | ML workflows |
| interview-prep | Mock interviews, DSA, behavioral prep | 5 | Hiring preparation |

## Top 10 Most Useful Prompts

### 1. Senior Code Review
**Use case:** Review a pull request like a senior engineer before merge.
**Works with:** All LLMs

```text
Act as a senior engineer performing a production-grade code review.

Review the following change in detail:

[YOUR CODE OR DIFF]

Context:
- Language: [LANGUAGE]
- Framework: [FRAMEWORK]
- Product area: [PRODUCT AREA]
- Risk level: [LOW/MEDIUM/HIGH]
- Expected behavior: [EXPECTED BEHAVIOR]

Evaluate correctness, readability, performance, security, test coverage, and maintainability.
Call out bugs, hidden edge cases, missing error handling, and API contract issues.
If something is ambiguous, state your assumption explicitly.

Output format:
1. Overall verdict
2. Blocking issues
3. Important non-blocking issues
4. Nice-to-have improvements
5. Suggested patch notes
```

### 2. Root Cause Analysis
**Use case:** Diagnose a bug, regression, or failure without guessing.
**Works with:** All LLMs

```text
Act as a senior software engineer and incident investigator.

Analyze the bug report and available evidence:

- Symptom: [BUG SYMPTOM]
- Environment: [LOCAL/STAGING/PROD]
- Logs: [LOGS]
- Relevant code: [YOUR CODE]
- Recent changes: [RECENT CHANGES]
- Reproduction steps: [STEPS]

Determine the most likely root cause and explain why.
Separate confirmed facts from hypotheses.
If more data is needed, list the exact next checks in priority order.

Output format:
1. Symptom summary
2. Most likely root cause
3. Evidence supporting the conclusion
4. Alternative hypotheses
5. Next debugging steps
6. Fix recommendation
```

### 3. System Design From Scratch
**Use case:** Design a new feature or service with realistic tradeoffs.
**Works with:** All LLMs

```text
Act as a principal engineer designing a production system from scratch.

Design [SYSTEM OR FEATURE] for:
- Users: [USER TYPE]
- Scale: [EXPECTED SCALE]
- Latency target: [LATENCY GOAL]
- Availability target: [AVAILABILITY GOAL]
- Compliance or security needs: [REQUIREMENTS]

Cover functional and non-functional requirements, APIs, data model, components, failure modes, scaling strategy, observability, and deployment concerns.
Call out tradeoffs and explicitly note what you would not build in version 1.

Output format:
1. Requirements
2. Proposed architecture
3. Data model
4. Key APIs or interfaces
5. Scalability and reliability considerations
6. Tradeoffs and risks
7. Implementation plan
```

### 4. Complete Test Suite Generator
**Use case:** Turn a feature into a practical test plan and starter tests.
**Works with:** All LLMs

```text
Act as a senior QA engineer and test automation specialist.

Generate a complete test strategy for this code:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Framework: [FRAMEWORK]
- Test runner: [TEST RUNNER]
- Feature goal: [GOAL]

Create unit, integration, and edge-case coverage where appropriate.
Include mocks, fixtures, and assertions for failure paths.
When a test is not appropriate, explain why.

Output format:
1. Test strategy
2. Test cases by category
3. Sample test code
4. Mocking plan
5. Gaps and assumptions
```

### 5. OWASP Top 10 Audit
**Use case:** Review code for common security weaknesses before release.
**Works with:** All LLMs

```text
Act as an application security engineer reviewing code against OWASP Top 10 risks.

Audit the following code or design:

[YOUR CODE OR DESIGN]

Context:
- App type: [WEB/API/MOBILE/CLI]
- Auth model: [AUTH MODEL]
- Data sensitivity: [LOW/MEDIUM/HIGH]
- External dependencies: [DEPENDENCIES]

Identify injection risks, auth weaknesses, access control issues, insecure defaults, secrets exposure, and unsafe data handling.
Prioritize issues by impact and exploitability.

Output format:
1. Risk summary
2. Findings ranked by severity
3. Attack scenario examples
4. Recommended remediations
5. Verification checklist
```

### 6. REST API Design Review
**Use case:** Make sure an API is predictable, versioned, and developer-friendly.
**Works with:** All LLMs

```text
Act as a senior API architect.

Review this API design:

[API SPEC OR ENDPOINT LIST]

Context:
- Domain: [DOMAIN]
- Clients: [WEB/MOBILE/INTERNAL]
- Auth method: [AUTH METHOD]
- Scale: [SCALE]

Assess resource modeling, status codes, pagination, filtering, error responses, idempotency, and backward compatibility.
Recommend changes that improve usability and operational safety.

Output format:
1. Design summary
2. Strengths
3. Problems and inconsistencies
4. Improved API recommendations
5. Example requests and responses
```

### 7. Dockerfile Optimizer
**Use case:** Improve image size, build speed, and runtime reliability.
**Works with:** All LLMs

```text
Act as a DevOps engineer specializing in container optimization.

Review and improve this Dockerfile:

[DOCKERFILE]

Context:
- App stack: [STACK]
- Build system: [BUILD TOOL]
- Runtime requirements: [REQUIREMENTS]

Optimize for smaller image size, deterministic builds, layer caching, security, and runtime clarity.
Explain any change that affects build behavior.

Output format:
1. Current issues
2. Recommended Dockerfile
3. Explanation of each major change
4. Security and performance notes
```

### 8. Conventional Commit Message
**Use case:** Turn a change description into a high-quality commit message.
**Works with:** All LLMs

```text
Act as a release-conscious software engineer.

Write a Conventional Commit message for this change:

[CHANGE DESCRIPTION]

Context:
- Scope: [SCOPE]
- Type: [feat/fix/docs/refactor/test/chore]
- Breaking change: [YES/NO]

Return one primary commit message and up to three alternatives.

Output format:
1. Best commit message
2. Alternatives
3. Short rationale
```

### 9. README Generator
**Use case:** Create a polished README for an open source or internal project.
**Works with:** All LLMs

```text
Act as a technical writer and open source maintainer.

Generate a README for this project:

- Project name: [PROJECT NAME]
- What it does: [DESCRIPTION]
- Audience: [AUDIENCE]
- Stack: [STACK]
- Installation: [INSTALL STEPS]
- Usage examples: [EXAMPLES]

Include clear sections, concise language, and a professional tone.
Add placeholders where project-specific values are needed.

Output format:
1. Title
2. Short description
3. Features
4. Installation
5. Usage
6. Configuration
7. Contributing
8. License
```

### 10. Clean Code Refactor
**Use case:** Improve a messy function or module without changing behavior.
**Works with:** All LLMs

```text
Act as a senior engineer refactoring legacy code.

Refactor the following code while preserving behavior:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Constraints: [CONSTRAINTS]
- Known tests: [TESTS]

Reduce complexity, improve naming, remove duplication, and isolate responsibilities.
Do not introduce unnecessary abstractions.
Call out any behavior that might change accidentally.

Output format:
1. Refactor goals
2. Refactored code
3. What changed
4. Risks to verify
5. Suggested tests
```

## How to Use

### Claude

- Paste the prompt directly and attach the relevant code, logs, or design notes.
- Ask Claude to keep the output in the requested structure.
- For long prompts, use one prompt per message to keep context focused.

### ChatGPT

- Use the prompt text as-is or turn it into a custom instruction block.
- Add your concrete inputs under the placeholder sections.
- If the answer drifts, remind the model to follow the output format exactly.

### Copilot

- Use short versions of the prompts as inline comments in your editor.
- Keep prompt titles in snippets or workspace notes for fast reuse.
- Pair prompt usage with tests so you can validate the generated suggestions quickly.

### VS Code Tips

- Save your favorite prompts in a `.md` file or snippet collection.
- Bind commonly used prompts to text expansion tools.
- When reviewing code, include the smallest useful excerpt plus surrounding context.
- For debugging, paste the exact error, logs, and the last known good behavior.

## Contributing

We welcome additions that are practical, specific, and useful in real developer workflows.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

See [prompts/PROMPTS_INDEX.md](prompts/PROMPTS_INDEX.md) for the category map and repository structure.

Community and safety documents:

- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- [SECURITY.md](SECURITY.md)

## Star History

If this repository helps your workflow, consider starring it to help others discover it.

<!-- Replace with a live star history image when publishing -->
[![Star History Chart](https://api.star-history.com/svg?repos=rishabhdhakad-dev/awesome-llm-prompts-for-devs&type=Date)](https://star-history.com/#rishabhdhakad-dev/awesome-llm-prompts-for-devs&Date)

## License

MIT License. See [LICENSE](LICENSE) for details.
