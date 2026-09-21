# Security Policy

## Supported release

The current supported public-preview line is **Foldrone Play 0.4.x**.

## Reporting a vulnerability

Please do not disclose security vulnerabilities in a public GitHub issue.

Report security issues privately to the project maintainer through the contact method published by the project owner.

Include:

- A clear description
- Affected component or file
- Reproduction steps
- Expected and actual behavior
- Security impact
- A safe proof of concept where appropriate

## Security principles

1. Never place secrets or API credentials in browser code.
2. Keep provider credentials in server-side secret storage.
3. Treat media URLs and external content as untrusted input.
4. Keep iframe origins explicitly controlled.
5. Prefer local processing when practical.
6. Do not rely on source-code obscurity as a security boundary.
7. Keep security controls independent of visual UI behavior.

## Third-party services

Subtitle and media providers have their own terms and policies. Integrations must respect those requirements and should use server-side adapters when credentials are required.
