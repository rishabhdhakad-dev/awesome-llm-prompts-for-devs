# Documentation Prompts

### Auto-generate JSDoc/Docstring
**Use case:** Add useful inline documentation for functions and methods.
**Works with:** All LLMs

```text
Act as a senior engineer and technical writer.

Generate documentation comments for this code:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Style guide: [STYLE GUIDE]

Write concise but useful JSDoc or docstrings that explain intent, parameters, return values, side effects, and edge cases.

Output format:
1. Documented code
2. Notes on tricky behavior
```

### README Generator
**Use case:** Produce a polished README from project details.
**Works with:** All LLMs

```text
Act as a technical writer for open source projects.

Generate a README for:

- Project name: [PROJECT NAME]
- Description: [DESCRIPTION]
- Audience: [AUDIENCE]
- Stack: [STACK]
- Usage examples: [EXAMPLES]

Include installation, usage, configuration, contributing, and license sections.

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

### API Documentation
**Use case:** Document endpoints or SDK methods clearly for developers.
**Works with:** All LLMs

```text
Act as an API documentation specialist.

Create documentation for:

[API OR SDK CONTENT]

Context:
- Audience: [AUDIENCE]
- Auth: [AUTH]
- Examples language: [LANGUAGE]

Explain purpose, request shape, response shape, error cases, and examples.

Output format:
1. Overview
2. Endpoint or method details
3. Parameters
4. Response examples
5. Error handling
```

### Changelog Generator
**Use case:** Summarize changes into release notes people can scan quickly.
**Works with:** All LLMs

```text
Act as a release manager writing clear changelog entries.

Turn these changes into a changelog:

[CHANGE LIST]

Context:
- Release version: [VERSION]
- Audience: [AUDIENCE]

Group items by feature, fix, breaking change, and maintenance work.

Output format:
1. Summary
2. Features
3. Fixes
4. Breaking changes
5. Notes
```

### Architecture Decision Record
**Use case:** Capture an important technical decision and its tradeoffs.
**Works with:** All LLMs

```text
Act as a senior engineer documenting a design decision.

Write an ADR for:

[DECISION]

Context:
- Problem: [PROBLEM]
- Options considered: [OPTIONS]
- Constraints: [CONSTRAINTS]

Document the decision, the reasoning, the tradeoffs, and the consequences for future work.

Output format:
1. Status
2. Context
3. Decision
4. Alternatives considered
5. Consequences
```

### Onboarding Guide Generator
**Use case:** Help new developers get productive quickly.
**Works with:** All LLMs

```text
Act as a team lead creating an onboarding guide.

Generate an onboarding guide for:

[TEAM OR REPOSITORY]

Context:
- Stack: [STACK]
- Key services: [SERVICES]
- Local setup: [SETUP]
- First task: [FIRST TASK]

Include environment setup, repository layout, useful commands, common pitfalls, and first-week tasks.

Output format:
1. Welcome
2. Setup steps
3. Repo tour
4. Daily workflow
5. Common issues
6. Next steps
```
