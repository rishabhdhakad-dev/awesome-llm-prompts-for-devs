# DevOps Prompts

### Dockerfile Optimizer
**Use case:** Improve build speed, image size, and runtime safety.
**Works with:** All LLMs

```text
Act as a DevOps engineer specializing in container optimization.

Review and improve this Dockerfile:

[DOCKERFILE]

Context:
- App stack: [STACK]
- Build system: [BUILD TOOL]
- Runtime requirements: [REQUIREMENTS]

Optimize for image size, caching, deterministic builds, and security.
Explain any change that affects the build or runtime behavior.

Output format:
1. Current issues
2. Recommended Dockerfile
3. Explanation of major changes
4. Security and performance notes
```

### CI/CD Pipeline Generator
**Use case:** Build a pipeline that matches the team workflow and release risk.
**Works with:** All LLMs

```text
Act as a DevOps architect.

Generate a CI/CD pipeline for:

[PROJECT]

Context:
- Repo host: [GITHUB/GITLAB/etc.]
- Test stages: [STAGES]
- Deployment target: [TARGET]
- Approval needs: [APPROVALS]

Include linting, tests, security checks, build steps, and deployment gates.

Output format:
1. Pipeline goals
2. Stages
3. Example workflow or YAML
4. Failure handling
5. Maintenance notes
```

### Kubernetes Manifest Reviewer
**Use case:** Review cluster manifests for reliability and security.
**Works with:** All LLMs

```text
Act as a senior platform engineer reviewing Kubernetes manifests.

Review these manifests:

[KUBERNETES YAML]

Context:
- Cluster type: [CLUSTER]
- Workload type: [WORKLOAD]
- Reliability goals: [GOALS]

Check probes, resource limits, security context, config handling, rollout behavior, and autoscaling readiness.

Output format:
1. Manifest summary
2. Problems found
3. Reliability risks
4. Recommended manifest changes
5. Validation checklist
```

### GitHub Actions Workflow
**Use case:** Create or improve GitHub Actions automation.
**Works with:** All LLMs

```text
Act as a CI engineer.

Design a GitHub Actions workflow for:

[PROJECT OR TASK]

Context:
- Language: [LANGUAGE]
- Required jobs: [JOBS]
- Deployment needs: [DEPLOYMENT]

Include caching, matrix builds, artifact handling, secrets usage, and failure reporting.

Output format:
1. Workflow overview
2. Jobs and steps
3. Example YAML
4. Performance notes
5. Security notes
```

### Environment Setup Guide
**Use case:** Document how to prepare local or staging environments.
**Works with:** All LLMs

```text
Act as a senior engineer writing an environment setup guide.

Create a setup guide for:

[PROJECT OR SERVICE]

Context:
- OS targets: [OS]
- Dependencies: [DEPENDENCIES]
- Services: [SERVICES]

Include prerequisites, installation, environment variables, startup steps, and troubleshooting.

Output format:
1. Prerequisites
2. Setup steps
3. Configuration
4. Verification steps
5. Troubleshooting
```

### Monitoring and Alerting Setup
**Use case:** Add observability and alerts that catch real problems early.
**Works with:** All LLMs

```text
Act as a production observability engineer.

Design monitoring and alerting for:

[SYSTEM OR SERVICE]

Context:
- Metrics available: [METRICS]
- Log sources: [LOGS]
- Alert fatigue risk: [RISK]

Recommend dashboards, alerts, thresholds, and escalation paths.
Focus on actionable alerts tied to user impact.

Output format:
1. Observability goals
2. Metrics and dashboards
3. Alert definitions
4. Escalation plan
5. Alert tuning guidance
```
