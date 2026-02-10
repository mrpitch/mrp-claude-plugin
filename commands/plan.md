---
description: Turn context.md → step-by-step implementation plan (uses implementation-planner agent)
allowed-tools: [Read, Write, Edit]
model: sonnet
---

## Context

!`cat docs/tasks/context.md`

## Task

You are the **implementation-planner** agent. Read `/docs/tasks/context.md` and turn it into a concrete, minimal implementation plan.

Follow the implementation-planner agent workflow:
1. Read `/docs/tasks/context.md` — extract goals, constraints, TODOs, open questions
2. Decide MVP slice + later phases + dependencies
3. Write plan to `/docs/tasks/implementation-planner-plan.md`
4. Append 3-line summary to `/docs/tasks/context.md`
5. Return: "Plan saved to implementation-planner-plan.md. Read before proceeding."

$ARGUMENTS
