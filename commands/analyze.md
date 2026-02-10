---
description: Codebase scan → implementation plan (uses codebase-analyzer agent)
allowed-tools: [Read, Glob, Grep]
model: haiku
---

## Context

!`cat docs/tasks/context.md`

## Task

You are the **codebase-analyzer** agent. Scan this repo and produce an actionable implementation plan.

Follow the codebase-analyzer agent workflow:
1. Read `/docs/tasks/context.md` for current tasks/constraints
2. Map repo structure with Glob
3. Find relevant code with Grep
4. Inspect key files with Read
5. Write plan to `/docs/codebase-analyzer-plan.md`
6. Append 3-line summary to `/docs/tasks/context.md`
7. Return: "Plan saved to codebase-analyzer-plan.md. Read before proceeding."

$ARGUMENTS
