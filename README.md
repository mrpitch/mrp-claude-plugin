# mrp-claude-plugin

TS/React/Next.js dev agents, skills & commands for Claude Code.

## Install

```bash
claude plugin install github:mrpitch/mrp-claude-plugin
```

## Agents

| Agent | Model | Purpose |
|-------|-------|---------|
| `requirements-analyst` | sonnet | Interactive Q&A → requirements spec |
| `implementation-planner` | sonnet | context.md → step-by-step plan |
| `codebase-analyzer` | haiku | Repo scan → implementation plan |
| `tech-research-planner` | opus | Library/tech research via context7 |
| `security-auditor` | — | OWASP Top 10 security scan |

## Skills

- **clean-typescript** — Clean, efficient TypeScript best practices
- **modern-best-practice-react-components** — Modern React (19+) component patterns
- **modern-browser-apis** — Native browser APIs over JS libraries
- **modern-best-practice-nextjs** — Next.js App Router best practices
- **modern-accessible-html-jsx** — Semantic, accessible HTML & JSX
- **web-security** — Web security & vulnerability prevention
- **modern-tailwind** — Tailwind CSS modern utilities & variants

## Commands

| Command | Purpose |
|---------|---------|
| `/mrp-claude-plugin:analyze` | Codebase scan → implementation plan |
| `/mrp-claude-plugin:requirements` | Interactive requirements Q&A |
| `/mrp-claude-plugin:plan` | Turn context.md → step-by-step plan |
| `/mrp-claude-plugin:research` | Library/tech research via context7 |
| `/mrp-claude-plugin:audit` | OWASP security scan |

## Prerequisites

- [context7 MCP](https://github.com/upstash/context7) — required for `/mrp-claude-plugin:research` command
- All agents read/write to `/docs/tasks/context.md` for shared context

## Context Flow

Agents share state through `/docs/tasks/context.md`. Each agent appends a 3-line summary after completing its work, enabling chained workflows (e.g., requirements → plan → implement).
