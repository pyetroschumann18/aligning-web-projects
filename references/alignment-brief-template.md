# Web Project Alignment Brief Template

Produce the brief in the user's language while keeping the title **Web Project Alignment Brief**. Prefer concise prose and tables. Do not omit a section: use `Não se aplica` with a reason when necessary.

## Required sections

1. **Resumo do projeto** — one clear paragraph that a new collaborator can understand.
2. **Tipo de site** — primary type and any secondary pattern.
3. **Objetivo principal** — the outcome the product must create.
4. **Público-alvo** — primary and relevant secondary audiences.
5. **Problema resolvido** — user or business problem and current alternative.
6. **Critérios de sucesso** — observable outcomes, metrics, or acceptance signals.
7. **Escopo da primeira versão** — the smallest coherent release.
8. **Itens fora do escopo** — explicit exclusions.
9. **Páginas necessárias** — page/view inventory and purpose.
10. **Jornadas e fluxos principais** — actor, trigger, steps, and successful result.
11. **Funcionalidades** — grouped by user goal, with priority when useful.
12. **Requisitos de conteúdo** — copy, media, source, owner, format, and readiness.
13. **Direção visual confirmada** — brand inputs, references, tone, constraints, and unresolved visual choices.
14. **Requisitos de frontend** — required behavior, interaction, states, and browser-facing constraints without premature framework choices.
15. **Requisitos de backend** — server-side responsibilities or a reason it is unnecessary.
16. **Dados que serão armazenados** — entities, sensitivity, source, retention, and ownership.
17. **Usuários, autenticação e permissões** — user types, access rules, account lifecycle, or non-applicability.
18. **APIs e integrações** — systems, purpose, direction of data, ownership, and failure impact.
19. **Segurança e privacidade** — threats, access protection, consent, cookies, personal data, jurisdiction, and compliance needs.
20. **Acessibilidade** — target and concrete acceptance expectations.
21. **Responsividade** — priority devices, breakpoints as a later design concern, and special contexts.
22. **Performance** — user-relevant targets and critical pages or operations.
23. **SEO** — discovery goals, indexable content, migration or redirect needs, or non-applicability.
24. **Analytics** — success events, conversions, reporting owner, and consent constraints.
25. **Estratégia de testes** — critical journeys, risk-based coverage, failure cases, and acceptance criteria.
26. **Deploy, domínio e infraestrutura** — environments, hosting needs, domain/DNS/HTTPS ownership, secrets, and release constraints.
27. **Monitoramento e manutenção** — logs, alerts, backup/recovery, content upkeep, dependency upkeep, and owners.
28. **Restrições** — budget, schedule, team, technology, legal, vendor, and organizational constraints.
29. **Suposições** — accepted statements that still lack direct evidence.
30. **Riscos** — risk, impact, likelihood when useful, and mitigation or next decision.
31. **Decisões ainda adiáveis** — decision, why it can wait, impact, and latest safe decision point.
32. **Matriz completa das áreas** — all 36 areas, each with status and project-specific reason.
33. **Pronto para planejamento técnico quando** — objective readiness criteria that a planning workflow can verify.

## Area matrix format

| # | Área | Classificação | Justificativa |
|---:|---|---|---|
| 1–36 | Use the exact area names from `web-development-areas.md` | `Obrigatória`, `Opcional`, `Não se aplica`, or `Ainda não decidida` | Tie the reason to confirmed goals, users, functions, or risks. |

## Approval request

End with a direct request for approval or corrections. Approval applies to the brief only; it does not authorize implementation.

After approval, if the work is inside a repository, offer to save the brief as `docs/web-project-alignment.md`. Do not create that file unless the user approves the brief or explicitly asks for it.
