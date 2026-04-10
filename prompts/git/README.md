# Git Prompts

### Conventional Commit Message
**Use case:** Convert a change into a clean Conventional Commit.
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

### PR Description Generator
**Use case:** Summarize a change for reviewers and release notes.
**Works with:** All LLMs

```text
Act as a senior engineer writing a pull request description.

Generate a PR description for:

[CHANGE SUMMARY]

Context:
- Motivation: [MOTIVATION]
- Testing performed: [TESTS]
- Risk level: [RISK]

Include summary, key changes, testing, risks, and rollout notes.

Output format:
1. Summary
2. Key changes
3. Testing
4. Risks
5. Rollout notes
```

### Git History Cleanup
**Use case:** Plan a safe history rewrite for a branch or repository.
**Works with:** All LLMs

```text
Act as a Git expert helping clean up history.

Review this branch history and suggest cleanup:

[GIT LOG OR HISTORY]

Context:
- Branch type: [FEATURE/RELEASE]
- Collaboration level: [SOLO/TEAM]
- Risk tolerance: [LOW/MEDIUM/HIGH]

Recommend rebase, squash, fixup, or revert steps where appropriate.
Explain the safest sequence.

Output format:
1. History summary
2. Cleanup recommendation
3. Step-by-step plan
4. Risks
5. Validation checklist
```

### Branch Strategy Advisor
**Use case:** Choose a branching model that fits the team and release process.
**Works with:** All LLMs

```text
Act as a senior engineering manager and Git workflow advisor.

Recommend a branch strategy for:

[TEAM OR PROJECT]

Context:
- Team size: [SIZE]
- Release cadence: [CADENCE]
- CI maturity: [MATURITY]
- Deployment model: [MODEL]

Compare trunk-based, GitFlow, and simplified feature branches.
Recommend the least painful option for the team reality.

Output format:
1. Recommendation
2. Pros and cons
3. Workflow steps
4. Merge policy
5. Adoption notes
```

### Merge Conflict Resolver
**Use case:** Explain how to resolve a conflict without losing important changes.
**Works with:** All LLMs

```text
Act as a careful Git specialist.

Help resolve this merge conflict:

[CONFLICTED FILES OR DIFF]

Context:
- Branches involved: [BRANCHES]
- Intended behavior: [BEHAVIOR]

Explain which changes should win, how to merge both sides safely, and what tests to run afterward.

Output format:
1. Conflict summary
2. Resolution plan
3. Suggested merged content
4. Risks to verify
5. Post-merge checks
```

### Release Notes Generator
**Use case:** Turn commits or PRs into readable release notes.
**Works with:** All LLMs

```text
Act as a release manager writing concise release notes.

Generate release notes from:

[COMMITS OR PR LIST]

Context:
- Release version: [VERSION]
- Audience: [AUDIENCE]

Group items by feature, fix, and breaking change.

Output format:
1. Release summary
2. New features
3. Fixes
4. Breaking changes
5. Upgrade notes
```
