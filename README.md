# aligning-web-projects

Agent Skill para alinhar e levantar requisitos de sites e aplicações web antes do planejamento técnico ou da implementação.

Ela transforma ideias vagas ou briefings existentes em uma entrevista adaptativa e, ao final, em um **Web Project Alignment Brief** aprovado. A skill classifica as 36 áreas do desenvolvimento web, aprofunda somente as relevantes, registra decisões e explica escolhas técnicas em linguagem simples.

## Quando usar

- Criar um site, landing page, blog, portal, e-commerce, dashboard, sistema web ou SaaS.
- Reformular completamente um site existente.
- Transformar uma ideia vaga em requisitos claros.
- Identificar quais áreas técnicas um projeto web realmente exige.

Exemplos:

```text
Use $aligning-web-projects para alinhar uma landing page de captação de contatos para uma academia.
```

```text
Use $aligning-web-projects para transformar minha ideia de SaaS com equipes e assinaturas em um briefing aprovado.
```

```text
Use $aligning-web-projects para levantar os requisitos da reformulação completa do meu portfólio.
```

## O que ela entrega

A skill produz um briefing com objetivo, público, escopo inicial, páginas, jornadas, funcionalidades, conteúdo, dados, integrações, segurança, privacidade, acessibilidade, performance, SEO, analytics, testes, infraestrutura, riscos e uma matriz de 36 áreas do desenvolvimento web.

Ela alinha requisitos. Não desenvolve o site, não cria código de produção, não instala dependências, não configura serviços e não faz deploy.

## Estrutura

```text
aligning-web-projects/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
└── references/
    ├── web-development-areas.md
    ├── interview-routing.md
    └── alignment-brief-template.md
```

## Compatibilidade

O pacote segue o formato de Agent Skills e pode ser usado no Codex e em outros agentes compatíveis com essa especificação. A seleção automática está habilitada; a skill também pode ser chamada explicitamente como `$aligning-web-projects`.

## Instalação

Clone o repositório para o diretório pessoal de skills:

```bash
git clone https://github.com/pyetroschumann18/aligning-web-projects.git ~/.agents/skills/aligning-web-projects
```

No PowerShell do Windows, você pode usar:

```powershell
git clone https://github.com/pyetroschumann18/aligning-web-projects.git "$env:USERPROFILE\.agents\skills\aligning-web-projects"
```

Depois da instalação, inicie uma nova conversa ou nova execução do agente para atualizar a descoberta de skills.

