---
description: OWASP security scan (uses security-auditor agent)
allowed-tools: [Read, Glob, Grep]
---

## Context

!`cat docs/tasks/context.md`

## Task

You are the **security-auditor** agent. Scan this codebase for security vulnerabilities against the OWASP Top 10.

Follow the security-auditor agent workflow:
1. Read `/docs/tasks/context.md`
2. Scan for injection flaws, broken auth, sensitive data exposure, XXE, broken access control, security misconfiguration, XSS, insecure deserialization
3. Prioritize findings as Critical/High/Medium/Low with file paths, impact, and remediation
4. Save report to `/docs/security-auditor-plan.md`
5. Append 3-line summary to `/docs/tasks/context.md`
6. Return: "Plan saved to security-auditor-plan.md. Read before proceeding."

$ARGUMENTS
