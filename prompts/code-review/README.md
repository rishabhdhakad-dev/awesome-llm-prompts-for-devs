# Code Review Prompts

### Senior Code Review
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

### PR Review Comment Generator
**Use case:** Turn review notes into clear, respectful PR comments.
**Works with:** All LLMs

```text
Act as a thoughtful senior reviewer writing concise PR comments.

Given this change and review notes:

[YOUR CODE OR DIFF]

[REVIEW NOTES]

Rewrite the feedback into comments that are specific, constructive, and professional.
Preserve the intent, but make the tone collaborative and actionable.

Output format:
1. Short summary comment
2. Inline comments by file or area
3. Suggested next step for the author
```

### Performance Review
**Use case:** Find inefficient code paths and recommend practical optimizations.
**Works with:** All LLMs

```text
Act as a performance-focused senior engineer.

Review this code for CPU, memory, I/O, rendering, or network inefficiencies:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Runtime: [RUNTIME]
- Traffic or usage pattern: [PATTERN]
- Constraints: [CONSTRAINTS]

Identify the real bottlenecks, not hypothetical ones.
Recommend optimizations in order of expected impact.

Output format:
1. Performance summary
2. Bottlenecks
3. Optimization opportunities
4. Tradeoffs
5. Validation plan
```

### React Component Review
**Use case:** Review a React component for correctness, accessibility, and maintainability.
**Works with:** All LLMs

```text
Act as a senior React engineer reviewing a component for production use.

Review this component:

[YOUR REACT COMPONENT]

Context:
- State management: [STATE TOOL]
- Styling approach: [STYLING]
- Target devices: [DESKTOP/MOBILE/BOTH]
- Accessibility requirements: [A11Y REQUIREMENTS]

Check props design, rendering logic, hooks usage, accessibility, performance, and component boundaries.
Call out stale closures, unnecessary rerenders, and fragile assumptions.

Output format:
1. Component summary
2. Issues
3. Accessibility concerns
4. Performance concerns
5. Refactor recommendations
```

### Database Query Review
**Use case:** Review SQL or ORM queries for correctness and performance.
**Works with:** All LLMs

```text
Act as a senior backend engineer specializing in databases.

Review this query or query builder usage:

[YOUR QUERY]

Context:
- Database: [DATABASE]
- Table sizes: [TABLE SIZES]
- Indexes: [INDEXES]
- Expected frequency: [FREQUENCY]

Check for correctness, missing indexes, expensive joins, N+1 patterns, and unsafe assumptions.
Recommend a better query if one exists.

Output format:
1. Query summary
2. Correctness issues
3. Performance concerns
4. Indexing suggestions
5. Improved query
```

### Security-Focused Review
**Use case:** Review code from an attacker mindset before it ships.
**Works with:** All LLMs

```text
Act as an application security engineer.

Review the following code with a security-first mindset:

[YOUR CODE]

Context:
- App type: [APP TYPE]
- Data sensitivity: [LOW/MEDIUM/HIGH]
- Auth model: [AUTH MODEL]
- External inputs: [INPUT SOURCES]

Look for injection, authorization flaws, unsafe deserialization, SSRF, XSS, path traversal, secrets leakage, and unsafe defaults.
Explain exploitability and severity in practical terms.

Output format:
1. Security summary
2. Findings by severity
3. Attack paths
4. Recommended fixes
5. Verification checklist
```

### TypeScript Type Review
**Use case:** Improve types, generics, and inference in TypeScript code.
**Works with:** All LLMs

```text
Act as a senior TypeScript engineer.

Review this TypeScript code:

[YOUR TYPESCRIPT CODE]

Context:
- TS version: [VERSION]
- Framework: [FRAMEWORK]
- Strict mode: [YES/NO]

Check for unsafe `any`, weak unions, poor inference, type widening, and unnecessary casts.
Improve the types without making the code harder to read.

Output format:
1. Type safety summary
2. Problems in the current types
3. Improved type definitions
4. Notes on inference and maintainability
```

### Mobile/Responsive Review
**Use case:** Review layouts for responsive behavior and mobile usability.
**Works with:** All LLMs

```text
Act as a senior frontend engineer reviewing responsive UI.

Review this layout or component:

[YOUR CODE]

Context:
- Framework: [FRAMEWORK]
- Breakpoints: [BREAKPOINTS]
- Target devices: [DEVICES]
- Accessibility needs: [A11Y]

Check spacing, overflow, touch targets, responsiveness, and cross-device behavior.
Call out issues that would break on small screens or high-density displays.

Output format:
1. Responsive summary
2. Layout issues
3. Mobile usability issues
4. Suggested CSS or component changes
5. Test checklist
```
