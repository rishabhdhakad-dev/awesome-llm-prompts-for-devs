# Security Prompts

### OWASP Top 10 Audit
**Use case:** Review code and design for common web application risks.
**Works with:** All LLMs

```text
Act as an application security engineer reviewing code against OWASP Top 10 risks.

Audit this code or design:

[YOUR CODE OR DESIGN]

Context:
- App type: [WEB/API/MOBILE/CLI]
- Auth model: [AUTH MODEL]
- Data sensitivity: [LOW/MEDIUM/HIGH]
- External dependencies: [DEPENDENCIES]

Identify injection risks, auth weaknesses, access control issues, insecure defaults, secrets exposure, and unsafe data handling.
Prioritize findings by impact and exploitability.

Output format:
1. Risk summary
2. Findings ranked by severity
3. Attack scenario examples
4. Recommended remediations
5. Verification checklist
```

### SQL Injection Checker
**Use case:** Find unsafe query building and input handling.
**Works with:** All LLMs

```text
Act as a security-focused backend engineer.

Review this data access code for SQL injection risk:

[YOUR CODE]

Context:
- Database: [DATABASE]
- Query style: [RAW SQL / ORM / BUILDER]
- User input sources: [INPUTS]

Identify where untrusted input reaches queries, whether parameters are bound correctly, and how to fix unsafe patterns.

Output format:
1. Injection risk summary
2. Unsafe code paths
3. Safe alternatives
4. Verification steps
```

### Auth Flow Review
**Use case:** Review login, signup, password reset, and session flows.
**Works with:** All LLMs

```text
Act as a security architect reviewing authentication flows.

Review this auth design:

[AUTH FLOW]

Context:
- Identity provider: [PROVIDER]
- Session model: [SESSION MODEL]
- MFA: [YES/NO]
- Account recovery: [RECOVERY]

Check for weak enrollment, token leakage, replay risk, insecure reset flows, account enumeration, and privilege escalation.

Output format:
1. Flow summary
2. Security issues
3. Attack paths
4. Fix recommendations
5. Hardening checklist
```

### API Security Review
**Use case:** Review endpoints for authorization, abuse, and data leakage.
**Works with:** All LLMs

```text
Act as an API security engineer.

Review this API:

[API SPEC OR ENDPOINTS]

Context:
- Auth method: [AUTH]
- Permissions model: [PERMISSIONS]
- Rate limiting: [LIMITS]
- Data sensitivity: [SENSITIVITY]

Assess authorization checks, object-level access control, input validation, error leaks, rate limits, and abuse resistance.

Output format:
1. Security summary
2. Findings
3. Abuse scenarios
4. Recommended protections
5. Validation checklist
```

### Dependency Vulnerability Scan
**Use case:** Review package risk and supply chain hygiene.
**Works with:** All LLMs

```text
Act as a supply-chain security analyst.

Review this dependency list or lockfile:

[DEPENDENCIES]

Context:
- Ecosystem: [NPM/PIP/GO/MAVEN/etc.]
- Update policy: [POLICY]
- Runtime exposure: [EXPOSURE]

Identify risky dependencies, outdated packages, suspicious maintenance patterns, and pinning issues.
Recommend practical remediation steps.

Output format:
1. Dependency risk summary
2. High-risk packages
3. Maintenance concerns
4. Upgrade plan
5. Verification steps
```

### Secrets and Env Var Audit
**Use case:** Find hardcoded secrets, unsafe config, and leaking environment variables.
**Works with:** All LLMs

```text
Act as a security engineer auditing secret handling.

Review this code or config:

[YOUR CODE OR CONFIG]

Context:
- Deployment target: [TARGET]
- Secret storage: [STORAGE]
- Sensitive values: [VALUES]

Find hardcoded secrets, insecure env handling, logging leaks, and missing rotation strategy.

Output format:
1. Secret handling summary
2. Exposed or risky values
3. Fix recommendations
4. Rotation and storage guidance
5. Verification checklist
```

### CORS Configuration Review
**Use case:** Review cross-origin policy for security and usability.
**Works with:** All LLMs

```text
Act as a web security engineer reviewing CORS settings.

Review this CORS configuration:

[CORS CONFIG]

Context:
- Frontend origins: [ORIGINS]
- Auth method: [AUTH]
- Cookie usage: [YES/NO]

Check for overly broad origins, credentials misconfiguration, unsafe headers, and accidental exposure.

Output format:
1. CORS summary
2. Misconfigurations
3. Risk level
4. Safer configuration
5. Validation steps
```

### JWT Security Review
**Use case:** Review token handling for common JWT mistakes.
**Works with:** All LLMs

```text
Act as a senior security engineer reviewing JWT usage.

Review this JWT implementation:

[YOUR CODE OR FLOW]

Context:
- Signing algorithm: [ALGORITHM]
- Token lifetime: [LIFETIME]
- Storage location: [STORAGE]
- Refresh flow: [REFRESH FLOW]

Check algorithm confusion, weak signing, invalid claim checks, unsafe storage, missing rotation, and replay risk.

Output format:
1. JWT security summary
2. Problems found
3. Abuse scenarios
4. Safer design
5. Validation checklist
```
