# Web Development Areas

Use this reference to maintain the applicability matrix throughout alignment. Classify every area with one of these labels:

| Status | Meaning |
|---|---|
| `Obrigatória` | The first release cannot meet its confirmed goal, safety needs, or launch requirements without it. |
| `Opcional` | It could add value, but the first release can succeed without it. |
| `Não se aplica` | Confirmed product needs do not require it. |
| `Ainda não decidida` | A missing user or business decision prevents a defensible classification. |

Every row needs a short reason tied to the project type, users, features, or risks. A technology preference alone is not a reason.

## Product and experience

| # | Area | Classification signals |
|---:|---|---|
| 1 | Objetivo do produto | Always `Obrigatória`; define the outcome the site must create. |
| 2 | Público-alvo | Always `Obrigatória`; identify primary users and relevant needs or constraints. |
| 3 | Critérios de sucesso | `Obrigatória` when launch value must be evaluated; define observable outcomes or metrics. |
| 4 | Escopo e versão inicial | Always `Obrigatória`; distinguish the first useful release from later work. |
| 5 | Páginas e estrutura de navegação | `Obrigatória` for multi-page or multi-view experiences; a single page still needs a section hierarchy. |
| 6 | Jornada e experiência do usuário | `Obrigatória` for every user goal; depth scales from one conversion path to multiple role-based flows. |
| 7 | Interface e identidade visual | `Obrigatória` for public-facing experiences; existing brand assets may satisfy part of it. |
| 8 | Conteúdo, imagens e mídia | `Obrigatória` when copy or media communicates the offer; identify source, owner, format, and readiness. |

## Application capabilities

| # | Area | Classification signals |
|---:|---|---|
| 9 | Frontend | `Obrigatória` for any browser interface; requirements concern behavior and presentation, not framework preference. |
| 10 | Backend | `Obrigatória` for server-side rules, private data, secure form processing, accounts, or dynamic operations; often `Não se aplica` to a purely static site. |
| 11 | Banco de dados | `Obrigatória` when durable structured data must be created or queried; `Não se aplica` when nothing is stored by the project. |
| 12 | APIs e integrações | `Obrigatória` when confirmed flows depend on external or internal systems; otherwise optional or not applicable. |
| 13 | Cadastro, login e autenticação | `Obrigatória` only when identified users need protected or personalized access. |
| 14 | Usuários, papéis e permissões | `Obrigatória` when different user types can see or do different things. |
| 15 | Pagamentos e assinaturas | `Obrigatória` for online sales, recurring billing, paid bookings, or other confirmed charging flows. |
| 16 | Painel administrativo | `Obrigatória` when authorized staff must manage changing content, users, orders, or operations; avoid assuming one for static content. |
| 17 | Busca e filtros | `Obrigatória` for catalogs or datasets that users cannot reasonably browse linearly; optional for small collections. |
| 18 | Comunicação por e-mail, WhatsApp ou notificações | Classify from confirmed reminders, leads, receipts, alerts, support, or transactional messages. |
| 19 | Upload e armazenamento de arquivos | `Obrigatória` when users or staff submit or manage documents or media; include file types, size, retention, and access. |

## Quality, risk, and compliance

| # | Area | Classification signals |
|---:|---|---|
| 20 | Segurança | Always `Obrigatória`; depth follows exposure, authentication, payments, integrations, and data sensitivity. |
| 21 | Privacidade, cookies e LGPD | `Obrigatória` when personal data, tracking, cookies, forms, accounts, or regulated information are involved. Confirm jurisdiction rather than assuming LGPD is the only applicable rule. |
| 22 | Acessibilidade | Always `Obrigatória`; define the target level or practical acceptance criteria when relevant. |
| 23 | Responsividade e dispositivos | Always `Obrigatória`; identify priority devices and any unusual contexts. |
| 24 | Compatibilidade entre navegadores | `Obrigatória` for launch; define supported browsers from the audience and organizational constraints. |
| 25 | Performance | Always `Obrigatória`; make targets proportional to content, devices, conversion, and interactivity. |
| 26 | SEO | `Obrigatória` when organic discovery matters; `Não se aplica` to private tools and some authenticated dashboards. |
| 27 | Analytics e conversões | `Obrigatória` when success depends on measurable acquisition, engagement, revenue, or task completion; respect consent requirements. |
| 28 | Testes e critérios de aceitação | Always `Obrigatória`; cover critical journeys, failures, permissions, data integrity, and release conditions as applicable. |

## Delivery and operations

| # | Area | Classification signals |
|---:|---|---|
| 29 | Git e colaboração | `Obrigatória` for maintained custom development or multiple contributors; may be optional for managed no-code work. |
| 30 | CI/CD | `Obrigatória` when repeated releases need automated checks or deployment; optional for a very small managed site. |
| 31 | Hospedagem e deploy | Always `Obrigatória` for a public or organizational launch; align region, budget, access, and operational owner. |
| 32 | Domínio, DNS e HTTPS | `Obrigatória` for public sites and branded access; record existing ownership and who can change DNS. |
| 33 | Variáveis de ambiente e segredos | `Obrigatória` when the project uses credentials, private configuration, integrations, or multiple environments. |
| 34 | Logs, monitoramento e alertas | `Obrigatória` for operational web applications and revenue-critical flows; may be optional for low-risk static pages. |
| 35 | Backup e recuperação | `Obrigatória` for original or changing data that cannot be recreated safely; `Não se aplica` when the project owns no durable data. |
| 36 | Manutenção e evolução | Always `Obrigatória`; identify ownership, update cadence, content maintenance, dependency maintenance, and likely next releases. |

## Reclassification rules

- Revisit dependent areas when a product decision changes. Adding accounts can change backend, database, permissions, security, privacy, testing, secrets, monitoring, and backup.
- Do not mark an area `Não se aplica` merely because the user has not mentioned it. Use that status only when available facts rule it out.
- Do not make every area `Obrigatória`. Scale depth to the simplest release that can meet the confirmed goal.
- Keep a materially consequential unknown as `Ainda não decidida`, state its impact, and route the next questions toward it.
