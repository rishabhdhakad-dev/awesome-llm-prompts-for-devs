# Refactoring Prompts

### Clean Code Refactor
**Use case:** Improve readability and maintainability without changing behavior.
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

Output format:
1. Refactor goals
2. Refactored code
3. What changed
4. Risks to verify
5. Suggested tests
```

### Design Pattern Applier
**Use case:** Introduce a pattern only when it solves a real design problem.
**Works with:** All LLMs

```text
Act as a pragmatic senior software architect.

Review this code and determine whether a design pattern would improve it:

[YOUR CODE]

Context:
- Current pain points: [PAIN POINTS]
- Language: [LANGUAGE]

Only recommend a pattern if it reduces complexity or improves extensibility.
If a pattern is unnecessary, say so clearly.

Output format:
1. Current design assessment
2. Pattern recommendation or rejection
3. Proposed structure
4. Tradeoffs
5. Implementation notes
```

### Legacy Code Modernizer
**Use case:** Update old code to modern practices and safer APIs.
**Works with:** All LLMs

```text
Act as a senior engineer modernizing legacy code.

Modernize this code:

[YOUR CODE]

Context:
- Language version: [VERSION]
- Framework version: [VERSION]
- Backward compatibility needs: [NEEDS]

Update deprecated APIs, simplify structure, and improve clarity while preserving behavior.

Output format:
1. Modernization summary
2. Outdated patterns
3. Updated code
4. Compatibility notes
5. Verification checklist
```

### Function Decomposition
**Use case:** Split a large function into smaller, focused units.
**Works with:** All LLMs

```text
Act as a senior engineer improving function structure.

Decompose this function:

[YOUR FUNCTION]

Context:
- Constraints: [CONSTRAINTS]
- Language: [LANGUAGE]

Split responsibilities into smaller functions with clear names and boundaries.
Preserve behavior and keep the call flow easy to follow.

Output format:
1. Decomposition plan
2. New function breakdown
3. Refactored code
4. Notes on behavior preservation
```

### Magic Numbers and Strings Eliminator
**Use case:** Replace hardcoded values with named constants or configuration.
**Works with:** All LLMs

```text
Act as a senior engineer removing hardcoded values.

Review this code:

[YOUR CODE]

Identify magic numbers, magic strings, and repeated literals.
Replace them with well-named constants, enums, or configuration values where appropriate.

Output format:
1. Hardcoded values found
2. Replacement strategy
3. Refactored code
4. Notes on naming choices
```

### Error Handling Improver
**Use case:** Make failures clearer, safer, and easier to debug.
**Works with:** All LLMs

```text
Act as a senior engineer improving error handling.

Review this code:

[YOUR CODE]

Context:
- Error policy: [POLICY]
- Logging system: [LOGGING]

Improve exception handling, validation, fallback behavior, and error messages.
Preserve useful context without leaking sensitive data.

Output format:
1. Error handling issues
2. Improved strategy
3. Refactored code
4. Operational notes
```
