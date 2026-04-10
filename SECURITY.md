# Security Policy

## Supported Versions

This repository is maintained as a documentation-first open source project.
Security updates are applied to the latest `main` branch content.

| Version | Supported |
| --- | --- |
| `main` | Yes |

## Reporting a Vulnerability

If you discover a security issue in this repository, please do not open a
public issue. Instead, report it privately to the maintainer.

Please include:

- Affected file or prompt
- Description of the issue
- Potential impact
- Suggested fix, if known

## What Counts as a Security Issue

Examples include:

- Malicious or unsafe prompt content
- Hidden prompt injection risks in examples
- Exposure of secrets, tokens, or private data in documentation
- Broken links to security-related guidance
- Supply chain or dependency concerns introduced by future contributions

## Response Expectations

We aim to acknowledge reports promptly and will work with the reporter to
validate the issue, assess impact, and publish a fix if needed.

## Security Best Practices for Contributors

- Avoid including secrets, keys, or private URLs in examples
- Prefer sanitized sample data
- Keep prompt outputs explicit about not leaking sensitive data
- Review markdown links and badges for correctness before submitting a PR
