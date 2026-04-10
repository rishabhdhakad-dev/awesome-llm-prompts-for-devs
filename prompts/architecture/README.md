# Architecture Prompts

### System Design From Scratch
**Use case:** Design a new product or service with clear tradeoffs.
**Works with:** All LLMs

```text
Act as a principal engineer designing a system from scratch.

Design [SYSTEM OR FEATURE] for:
- Users: [USER TYPE]
- Scale: [EXPECTED SCALE]
- Latency target: [LATENCY TARGET]
- Availability target: [AVAILABILITY TARGET]
- Constraints: [CONSTRAINTS]

Cover requirements, architecture, data flow, APIs, storage, observability, and failure modes.
Explain what should be built first and what can wait.

Output format:
1. Requirements
2. Proposed architecture
3. Data model
4. APIs
5. Scaling and reliability
6. Risks and tradeoffs
7. Implementation plan
```

### Scalability Review
**Use case:** Review whether an existing system can handle growth.
**Works with:** All LLMs

```text
Act as a senior architect reviewing scalability.

Evaluate this system:

[SYSTEM DESCRIPTION]

Context:
- Current traffic: [CURRENT TRAFFIC]
- Projected traffic: [PROJECTED TRAFFIC]
- Hot paths: [HOT PATHS]
- Bottlenecks: [KNOWN BOTTLENECKS]

Identify where the system will break first and how to scale it safely.
Include data, compute, caching, queues, and operational concerns.

Output format:
1. Scalability summary
2. Current bottlenecks
3. Scaling risks
4. Recommended changes
5. Validation and rollout plan
```

### Microservices vs Monolith Decision
**Use case:** Choose an architecture style based on product and team reality.
**Works with:** All LLMs

```text
Act as a pragmatic principal engineer.

Help decide between a monolith and microservices for:

[PRODUCT OR SYSTEM]

Context:
- Team size: [TEAM SIZE]
- Delivery speed need: [SPEED]
- Deployment constraints: [CONSTRAINTS]
- Domain complexity: [COMPLEXITY]

Compare the options using operational cost, team autonomy, data consistency, debugging, and deployment complexity.
Give a recommendation based on the details provided.

Output format:
1. Decision summary
2. Monolith pros and cons
3. Microservices pros and cons
4. Recommendation
5. Migration path if needed
```

### Database Schema Design
**Use case:** Model data for a durable, queryable system.
**Works with:** All LLMs

```text
Act as a senior backend architect designing a database schema.

Design the schema for:

[FEATURE OR DOMAIN]

Context:
- Database: [DATABASE]
- Expected entities: [ENTITIES]
- Query patterns: [QUERY PATTERNS]
- Scale: [SCALE]

Include tables, primary keys, foreign keys, indexes, constraints, and migration considerations.
Explain how the schema supports common reads and writes.

Output format:
1. Domain model
2. Tables and relationships
3. Indexing plan
4. Query optimization notes
5. Migration considerations
```

### API Architecture Review
**Use case:** Evaluate the structure and reliability of backend APIs.
**Works with:** All LLMs

```text
Act as a senior API architect.

Review this API architecture:

[API DESCRIPTION]

Context:
- Clients: [CLIENTS]
- Auth: [AUTH]
- Data sources: [DATA SOURCES]
- Scale: [SCALE]

Assess versioning, consistency, pagination, error handling, idempotency, and backward compatibility.
Recommend a cleaner architecture if the current one is brittle.

Output format:
1. Architecture summary
2. Strengths
3. Weaknesses
4. Recommended changes
5. API contract examples
```

### Caching Strategy
**Use case:** Add caching without making the system stale or fragile.
**Works with:** All LLMs

```text
Act as a senior engineer designing a caching strategy.

Design caching for:

[SYSTEM OR FEATURE]

Context:
- Read/write ratio: [RATIO]
- Data freshness needs: [FRESHNESS]
- Cache layer options: [OPTIONS]
- Failure tolerance: [TOLERANCE]

Recommend what to cache, where to cache it, and how to invalidate safely.
Include risks like staleness, stampedes, and cache poisoning.

Output format:
1. Caching goals
2. What to cache
3. Cache placement
4. Invalidation strategy
5. Failure modes and mitigations
```

### Auth System Design
**Use case:** Design secure authentication and session handling.
**Works with:** All LLMs

```text
Act as a security-minded principal engineer.

Design an auth system for:

[APPLICATION]

Context:
- User types: [USER TYPES]
- Login methods: [LOGIN METHODS]
- Compliance needs: [NEEDS]
- Risk level: [LOW/MEDIUM/HIGH]

Cover registration, login, sessions or tokens, MFA, password resets, device trust, logout, and account recovery.
Prioritize secure defaults and operational simplicity.

Output format:
1. Auth requirements
2. Proposed flow
3. Session or token model
4. Security controls
5. Failure and recovery cases
```

### SaaS Multi-Tenancy Design
**Use case:** Plan tenant isolation and shared infrastructure for SaaS products.
**Works with:** All LLMs

```text
Act as a principal engineer designing a SaaS multi-tenant platform.

Design a tenancy model for:

[SAAS PRODUCT]

Context:
- Tenant count: [TENANT COUNT]
- Data sensitivity: [SENSITIVITY]
- Isolation needs: [ISOLATION REQUIREMENTS]
- Growth plan: [GROWTH PLAN]

Compare shared database, schema-per-tenant, and database-per-tenant approaches.
Cover isolation, billing, permissions, migrations, and operational complexity.

Output format:
1. Tenancy goals
2. Model comparison
3. Recommended approach
4. Data isolation plan
5. Operational concerns
6. Rollout strategy
```
