# Adaptive Interview Routing

Use this reference to decide what to ask next. The interview is a dependency-aware conversation, not a fixed questionnaire.

## Build the initial state

Before asking anything, extract:

- Explicit facts and their source: user message, linked brief, or inspected project file.
- Probable project type and confidence.
- Confirmed constraints: budget, deadline, team, platform, brand, legal region, and existing services.
- Candidate first-release outcome and user journeys.
- Provisional 36-area matrix.
- Open decisions and the downstream areas each one affects.

If an existing project is in scope, inspect only what answers a current alignment question: the repository overview, package manifest, routing structure, design tokens, content sources, deployment configuration, or relevant product documentation. Do not perform a general code review.

## Choose the next subject

Prioritize open decisions in this order:

1. Product purpose, audience, problem, and success.
2. First-release scope, primary journeys, content, and operating model.
3. Data, identities, roles, money movement, files, and external systems.
4. Risk and quality: security, privacy, accessibility, performance, SEO, analytics, and acceptance.
5. Delivery and ownership: collaboration, deployment, domain, secrets, monitoring, backup, and maintenance.
6. Technology options that follow from the confirmed needs.

Ask one to three closely related questions per round. Each question must resolve a named gap or distinguish between materially different routes. If an answer is already recorded, use it instead of rephrasing the question.

## Route by project type

| Probable type | Start with | Common conditional branches |
|---|---|---|
| Landing page or marketing site | Conversion goal, audience, offer, proof, call to action, content owner | Lead destination, form handling, consent, analytics, SEO, campaign deadline |
| Blog or content publication | Editorial purpose, authors, content volume, taxonomy, publishing workflow | Search, moderation, subscriptions, migration, SEO, media storage |
| E-commerce | Products and variants, inventory source, markets, checkout, fulfillment, returns | Accounts, taxes, payment provider, shipping integrations, promotions, support |
| SaaS or dashboard | User problem, tenant model, roles, core repeated task, data sensitivity, billing model | Invitations, permissions, auditability, integrations, notifications, exports, support |
| Portal or internal system | User groups, protected tasks, source of truth, permissions, operational owner | SSO, approvals, uploads, reporting, audit logs, retention, recovery |
| Complete redesign | Current URL or repository, reason for redesign, retained content/features, target audience, measurable problems | Migration, redirects, analytics baseline, brand change, accessibility debt, CMS constraints |

These are routing cues, not default requirements. Confirm them through the user's context.

## Dependency rules

- Do not ask which database to use until durable data needs are confirmed.
- Do not ask about login until identified or personalized users exist.
- Do not ask about roles until user types require different access.
- Do not ask about payments until selling, charging, or subscriptions are confirmed.
- Do not ask about a backend for a static landing page unless a flow needs server-side processing or protected data.
- Do not choose a framework before understanding team constraints, delivery model, maintenance, and required capabilities.
- Do not confuse a preferred implementation with a product requirement.

## When the user says “não sei”

Do not return the technical decision unchanged. Translate it into an outcome the user can judge.

1. Explain why the decision matters in one or two plain sentences.
2. Present only the viable options and their practical differences.
3. Recommend one using confirmed constraints.
4. Ask the user to accept, reject, or defer the recommendation.
5. Record the result as a decision, accepted assumption, or deferrable choice.

Example: instead of asking “React or WordPress?”, ask whether the team needs to edit pages without a developer. Then explain which suitable approaches support that need.

## Decision checkpoint after each subject

Keep it brief and use the user's language:

```markdown
**Decisões confirmadas**
- ...

**Suposições aceitas**
- ...

**Questões em aberto**
- ...

**Mudanças de escopo**
- Área adicionada/removida — motivo
```

Use `Nenhuma` when a category is empty. Update the matrix internally after the checkpoint; show affected classifications when they help the user make the next decision.

## Handling pressure to implement

If the user asks to code before alignment is complete:

1. Acknowledge the deadline or reason without negotiating away the skill boundary.
2. Name the unresolved decisions and the concrete rework, safety, cost, or product risk they create.
3. Offer the fastest alignment path: the smallest question round that can close the blocking gaps.
4. Continue alignment. Do not scaffold, prototype, choose a stack, produce production code, or hand off an implementation plan.

The following are still implementation and remain out of scope: a throwaway demo, mock-only app, reversible scaffold, starter repository, generated components, or “just the folder structure.”

## Completion gate

The interview is ready for a final brief when:

- The project goal, primary audience, problem, success criteria, and first release are explicit.
- Primary pages/views and user journeys are defined at the depth required by the project.
- Data, identity, permissions, payments, files, and integrations are classified with reasons.
- Material security, privacy, accessibility, performance, SEO, analytics, testing, launch, and operational needs are captured.
- Every remaining `Ainda não decidida` item is either blocking or explicitly safe to defer, with its impact recorded.
- Constraints, assumptions, risks, exclusions, and acceptance conditions are reviewable.

If a blocking item remains, ask about it. If only deferrable decisions remain, create the brief and identify them in its dedicated section.
