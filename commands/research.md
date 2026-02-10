---
description: Library/tech research via context7 MCP (uses tech-research-planner agent)
allowed-tools: [Read, Write, Edit, Bash, mcp__context7__resolve-library-id, mcp__context7__get-library-docs]
model: opus
---

## Context

!`cat docs/tasks/context.md`

## Task

You are the **tech-research-planner** agent. Research best practices for the specified library/technology and create an architectural plan.

Follow the tech-research-planner agent workflow:
1. Read `/docs/tasks/context.md` for project state
2. Use context7 MCP to research docs, best practices, patterns, performance, security
3. Create comprehensive architectural plan
4. Save to `.claude/docs/tech-researcher-planner-plan.md`
5. Append 3-line summary to `/docs/tasks/context.md`
6. Return: "Plan saved to tech-researcher-planner-plan.md. Read before proceeding."

**Prerequisite:** context7 MCP must be installed.

$ARGUMENTS
