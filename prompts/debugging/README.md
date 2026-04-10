# Debugging Prompts

### Root Cause Analysis
**Use case:** Diagnose a bug using logs, code, and reproduction steps.
**Works with:** All LLMs

```text
Act as a senior software engineer and incident investigator.

Analyze this issue:

- Symptom: [SYMPTOM]
- Environment: [ENVIRONMENT]
- Logs: [LOGS]
- Relevant code: [CODE]
- Recent changes: [CHANGES]
- Reproduction steps: [STEPS]

Find the most likely root cause and explain the evidence.
Separate facts from hypotheses.

Output format:
1. Problem summary
2. Root cause hypothesis
3. Evidence
4. Alternative explanations
5. Next checks
6. Fix recommendation
```

### Stack Trace Decoder
**Use case:** Translate a stack trace into an actionable debugging path.
**Works with:** All LLMs

```text
Act as a senior engineer decoding an error stack trace.

Interpret this stack trace:

[STACK TRACE]

Context:
- Language/runtime: [LANGUAGE OR RUNTIME]
- Framework: [FRAMEWORK]
- Last known action: [ACTION]

Explain where the failure started, what likely caused it, and how to verify the fix.
If the trace points to multiple layers, walk through them in order.

Output format:
1. Plain-English explanation
2. Probable failure point
3. Likely cause
4. Debugging steps
5. Fix ideas
```

### Async/Await Bug Hunter
**Use case:** Find concurrency bugs, promise mistakes, and lost awaits.
**Works with:** All LLMs

```text
Act as a senior engineer specializing in async control flow.

Review this code for async/await bugs:

[YOUR CODE]

Context:
- Language: [LANGUAGE]
- Runtime: [RUNTIME]
- Observed issue: [ISSUE]

Look for missing awaits, unhandled promise rejections, race conditions, bad sequencing, and swallowed errors.
Explain how each bug manifests in production.

Output format:
1. Async flow summary
2. Bugs found
3. Why they occur
4. Safe rewrite
5. Verification steps
```

### API Response Debugger
**Use case:** Diagnose unexpected API output or schema mismatches.
**Works with:** All LLMs

```text
Act as a backend debugging specialist.

Debug this API response problem:

- Request: [REQUEST]
- Expected response: [EXPECTED]
- Actual response: [ACTUAL]
- Server code: [CODE]
- Logs: [LOGS]

Find the most likely point where the response diverges from expectations.
Check serialization, validation, defaults, transforms, and error handling.

Output format:
1. Response mismatch summary
2. Most likely cause
3. Code path analysis
4. Suggested fix
5. Repro and verification steps
```

### Works Locally Fails in Prod
**Use case:** Compare environment differences when something breaks only in production.
**Works with:** All LLMs

```text
Act as an experienced production engineer.

Investigate why this code works locally but fails in production:

[YOUR CODE]

Context:
- Local environment: [LOCAL]
- Production environment: [PROD]
- Build process: [BUILD]
- Error symptoms: [ERROR]
- Config differences: [CONFIG]

Identify environment-specific causes such as timing, caching, env vars, permissions, dependencies, or platform behavior.

Output format:
1. Environment delta summary
2. Most likely production-only cause
3. Secondary causes to check
4. Remediation plan
5. Prevention checklist
```

### Memory Leak Detector
**Use case:** Find retained objects, runaway allocations, or unbounded caches.
**Works with:** All LLMs

```text
Act as a senior engineer diagnosing memory growth.

Analyze this code or symptom for memory leaks:

[YOUR CODE OR PROFILE DATA]

Context:
- Runtime: [RUNTIME]
- Observed memory pattern: [PATTERN]
- Workload: [WORKLOAD]

Look for retained references, event listener leaks, cache growth, unclosed resources, and repeated allocations.
Explain which objects are likely kept alive and why.

Output format:
1. Memory issue summary
2. Suspected leak sources
3. Why they leak
4. Fix recommendations
5. How to confirm the fix
```

### Race Condition Finder
**Use case:** Detect timing bugs caused by overlapping operations.
**Works with:** All LLMs

```text
Act as a concurrency-focused senior engineer.

Review this code for race conditions:

[YOUR CODE]

Context:
- Runtime: [RUNTIME]
- Shared resource: [RESOURCE]
- Concurrent actors: [ACTORS]

Find interleavings that could produce inconsistent state, lost updates, duplicate work, or stale reads.
Recommend locking, serialization, idempotency, or state-machine fixes where appropriate.

Output format:
1. Concurrency summary
2. Race scenarios
3. Impact
4. Recommended fix
5. Validation plan
```

### CSS Layout Debugger
**Use case:** Diagnose broken alignment, overflow, or responsive CSS behavior.
**Works with:** All LLMs

```text
Act as a senior frontend engineer debugging CSS layout issues.

Debug this layout problem:

[YOUR CSS OR COMPONENT]

Context:
- Browser(s): [BROWSERS]
- Screen sizes: [SIZES]
- Broken behavior: [BEHAVIOR]

Analyze box model behavior, flex/grid rules, overflow, stacking context, and responsive breakpoints.
Give precise fixes and explain why they work.

Output format:
1. Layout diagnosis
2. Root cause
3. CSS changes
4. Browser compatibility notes
5. Quick verification steps
```
