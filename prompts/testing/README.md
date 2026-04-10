# Testing Prompts

### Complete Test Suite Generator
**Use case:** Turn a feature into a practical test strategy and starter tests.
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

### TDD Workflow
**Use case:** Break work into a test-first implementation plan.
**Works with:** All LLMs

```text
Act as a senior engineer following test-driven development.

For this feature:

[FEATURE DESCRIPTION]

Create a TDD plan that starts with failing tests, then the minimum code to pass them, then refactoring.
Include edge cases and clarify where integration tests should take over from unit tests.

Output format:
1. Test-first plan
2. Initial failing tests
3. Minimal implementation steps
4. Refactor step
5. Final verification checklist
```

### Test Coverage Analyzer
**Use case:** Find gaps in existing tests and prioritize what to add next.
**Works with:** All LLMs

```text
Act as a senior QA lead analyzing test coverage.

Review this code and test suite:

[YOUR CODE]

[YOUR TESTS]

Context:
- Coverage report: [COVERAGE]
- Critical paths: [CRITICAL PATHS]

Identify what is under-tested, what is over-tested, and what tests would add the most confidence.
Focus on behavior, not just line coverage.

Output format:
1. Coverage summary
2. Missing test areas
3. Overlapping or low-value tests
4. Prioritized additions
5. Confidence assessment
```

### Mock and Stub Generator
**Use case:** Generate realistic mocks for dependencies and external services.
**Works with:** All LLMs

```text
Act as a senior test engineer.

Generate mocks and stubs for these dependencies:

[DEPENDENCIES]

Context:
- Language: [LANGUAGE]
- Test framework: [FRAMEWORK]
- Dependency behavior: [BEHAVIOR]

Create realistic fake responses, error cases, and reset behavior.
Make the mocks easy to reuse across tests.

Output format:
1. Mocking plan
2. Mock implementation
3. Error case coverage
4. Reuse notes
```

### E2E Test Scenarios
**Use case:** Define end-to-end scenarios that match real user behavior.
**Works with:** All LLMs

```text
Act as a QA strategist designing end-to-end tests.

For this product flow:

[USER FLOW]

List realistic E2E scenarios, including happy path, failure path, permission issues, and boundary conditions.
Prioritize scenarios by business value and brittleness.

Output format:
1. User journey summary
2. E2E scenarios
3. Priority order
4. Data/setup needs
5. Flakiness risks
```

### Load Testing Strategy
**Use case:** Plan performance tests that reflect production usage.
**Works with:** All LLMs

```text
Act as a senior performance engineer.

Design a load testing strategy for:

[SYSTEM OR FEATURE]

Context:
- Expected traffic: [TRAFFIC]
- Peak patterns: [PEAKS]
- SLAs: [SLAS]
- Bottlenecks: [KNOWN BOTTLENECKS]

Define test types, metrics, ramps, thresholds, and failure criteria.
Explain what success and degradation look like.

Output format:
1. Load test goals
2. Scenarios and traffic model
3. Metrics to capture
4. Pass/fail criteria
5. Follow-up actions
```

### Test Naming Conventions
**Use case:** Standardize clear and readable test names.
**Works with:** All LLMs

```text
Act as a senior engineer establishing test naming conventions.

Create naming guidelines for this codebase:

[CODEBASE CONTEXT]

Include naming patterns for unit, integration, and E2E tests.
Favor names that describe behavior and expected outcomes.

Output format:
1. Naming principles
2. Recommended patterns
3. Good examples
4. Bad examples
5. Team conventions
```

### Integration Test Setup
**Use case:** Set up tests across service boundaries, databases, or queues.
**Works with:** All LLMs

```text
Act as a senior test infrastructure engineer.

Design an integration test setup for:

[SYSTEM]

Context:
- Services involved: [SERVICES]
- Database: [DATABASE]
- Queue or broker: [BROKER]
- Test environment constraints: [CONSTRAINTS]

Explain fixtures, isolation, cleanup, test data, and how to make tests reliable.

Output format:
1. Integration scope
2. Setup architecture
3. Data management
4. Cleanup strategy
5. Reliability checklist
```
