---
name: aligning-web-projects
description: Use when a web project still needs alignment before planning or implementation because a user intends to create a website, landing page, blog, portal, e-commerce store, dashboard, web system, or SaaS; requests a complete redesign; has a vague web idea; or wants to identify the technical areas required.
---

# Web Project Alignment

Turn available information into an approved **Web Project Alignment Brief**. Stay in alignment mode until approval.

## Scope boundary

Do not activate for a small correction, isolated bug, copy change, code review, or deploy-only request.

While active, do not write production code, modify the site, install dependencies, create a database, configure services, deploy, create tickets, produce designs, or make a technical plan. Continue beyond alignment only after brief approval and a later explicit request.

A scaffold, mock-data app, throwaway prototype, or “reversible start” is implementation. Deadlines, sunk effort, and “decide later” do not change this boundary. Under pressure, name the unresolved impact and ask only the questions needed to resolve it.

## Alignment loop

1. Extract every supplied fact. For an existing project, inspect only files needed to understand its relevant state.
2. Track confirmed decisions, accepted assumptions, open questions, and scope changes. Never repeat an answered question.
3. Identify the probable project type. Read [web-development-areas.md](references/web-development-areas.md) and provisionally classify all areas as `Obrigatória`, `Opcional`, `Não se aplica`, or `Ainda não decidida`, each with a project-specific reason.
4. Find gaps that materially affect the goal, first release, journeys, data risk, cost, or delivery. Read [interview-routing.md](references/interview-routing.md) before questioning and whenever answers change the route.
5. Ask one small, dependency-ordered round at a time. Use the user's language, explain technical terms plainly, and recommend when the user has no preference.
6. After each subject, show a brief checkpoint: confirmed decisions, accepted assumptions, open questions, and scope additions or removals.
7. Repeat until no important gap remains. Mark safely deferrable choices instead of forcing them.
8. Read [alignment-brief-template.md](references/alignment-brief-template.md), produce the complete brief, and request approval or corrections.

## Technical choices

Discover needs and constraints before technology. When options fit, explain their practical differences, recommend one using budget, schedule, team, maintenance, scale, and existing services, then record the user's decision. A recommendation is not approval.

## Completion contract

Finish only when relevant requirements are defined and the user approves the brief. In a repository, offer to save it as `docs/web-project-alignment.md`; do not write the file before approval or an explicit request.

After approval, state that the brief is ready for specification, planning, tickets, design, implementation, testing, and deployment. Do not perform them here.

## Red flags

- “We can scaffold now and align later.”
- “Mock data makes implementation harmless.”
- “The technology choice is obvious.”
- “A partial brief is enough because the deadline is close.”

Each red flag means: remain in alignment mode, name the unresolved impact, and ask the next highest-value questions.
