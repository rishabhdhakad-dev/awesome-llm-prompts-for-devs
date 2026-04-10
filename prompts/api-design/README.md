# API Design Prompts

### REST API Design Review
**Use case:** Make sure a REST API is predictable and easy to consume.
**Works with:** All LLMs

```text
Act as a senior API architect.

Review this REST API design:

[API SPEC]

Context:
- Clients: [WEB/MOBILE/INTERNAL]
- Auth method: [AUTH]
- Scale: [SCALE]

Assess resource modeling, status codes, pagination, filtering, error responses, idempotency, and versioning.
Recommend improvements that make the API easier to use and safer to evolve.

Output format:
1. Design summary
2. Strengths
3. Problems
4. Improved recommendations
5. Example requests and responses
```

### GraphQL Schema Designer
**Use case:** Design a GraphQL schema that is expressive and maintainable.
**Works with:** All LLMs

```text
Act as a senior GraphQL architect.

Design a GraphQL schema for:

[FEATURE OR DOMAIN]

Context:
- Client needs: [NEEDS]
- Data sources: [DATA SOURCES]
- Scale: [SCALE]

Define types, queries, mutations, error handling approach, pagination, and resolver boundaries.

Output format:
1. Schema goals
2. Proposed schema
3. Resolver plan
4. Performance considerations
5. Risks and tradeoffs
```

### API Versioning Strategy
**Use case:** Plan a versioning model that avoids breaking clients.
**Works with:** All LLMs

```text
Act as a senior API strategist.

Design a versioning strategy for:

[API OR PLATFORM]

Context:
- Current consumers: [CONSUMERS]
- Change frequency: [FREQUENCY]
- Backward compatibility needs: [NEEDS]

Compare path, header, and media-type versioning, then recommend a practical approach.

Output format:
1. Versioning goals
2. Strategy comparison
3. Recommendation
4. Deprecation policy
5. Migration plan
```

### Rate Limiting Design
**Use case:** Protect APIs from abuse without hurting legitimate users.
**Works with:** All LLMs

```text
Act as a backend architect designing rate limits.

Design rate limiting for:

[API OR SERVICE]

Context:
- User types: [USER TYPES]
- Traffic shape: [TRAFFIC]
- Abuse risk: [RISK]

Recommend limits, burst behavior, scopes, storage, and user feedback.
Explain how to avoid punishing normal traffic.

Output format:
1. Rate limiting goals
2. Proposed policy
3. Enforcement model
4. Edge cases
5. Operational guidance
```

### Error Response Standardizer
**Use case:** Make API errors consistent, useful, and machine-readable.
**Works with:** All LLMs

```text
Act as a senior API engineer standardizing error responses.

Design an error response format for:

[API OR PLATFORM]

Context:
- Client types: [CLIENTS]
- Localization: [YES/NO]
- Security sensitivity: [SENSITIVITY]

Define error codes, message fields, trace IDs, validation errors, and safe client-facing detail.

Output format:
1. Error model summary
2. Standard schema
3. Example responses
4. Guidance for common cases
5. Compatibility notes
```

### Webhook Design
**Use case:** Design webhooks that are reliable, secure, and retry-safe.
**Works with:** All LLMs

```text
Act as a senior platform engineer designing webhooks.

Design webhook delivery for:

[EVENT TYPE OR PRODUCT]

Context:
- Event volume: [VOLUME]
- Consumer reliability: [RELIABILITY]
- Security requirements: [REQUIREMENTS]

Cover signing, retries, ordering, idempotency, replay protection, and developer experience.

Output format:
1. Webhook goals
2. Delivery model
3. Security model
4. Retry and idempotency plan
5. Example payloads and headers
```
