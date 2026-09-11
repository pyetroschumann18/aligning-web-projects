# aligning-web-projects

Agent Skill para alinhar e levantar requisitos de sites e aplicaÃ§Ãµes web antes do planejamento tÃ©cnico ou da implementaÃ§Ã£o.

Ela transforma ideias vagas ou briefings existentes em uma entrevista adaptativa e, ao final, em um **Web Project Alignment Brief** aprovado. A skill classifica as 36 Ã¡reas do desenvolvimento web, aprofunda somente as relevantes, registra decisÃµes e explica escolhas tÃ©cnicas em linguagem simples.

## Quando usar

- Criar um site, landing page, blog, portal, e-commerce, dashboard, sistema web ou SaaS.
- Reformular completamente um site existente.
- Transformar uma ideia vaga em requisitos claros.
- Identificar quais Ã¡reas tÃ©cnicas um projeto web realmente exige.

Exemplos:

```text
Use $aligning-web-projects para alinhar uma landing page de captaÃ§Ã£o de contatos para uma academia.
```

```text
Use $aligning-web-projects para transformar minha ideia de SaaS com equipes e assinaturas em um briefing aprovado.
```

```text
Use $aligning-web-projects para levantar os requisitos da reformulaÃ§Ã£o completa do meu portfÃ³lio.
```

## O que ela entrega

A skill produz um briefing com objetivo, pÃºblico, escopo inicial, pÃ¡ginas, jornadas, funcionalidades, conteÃºdo, dados, integraÃ§Ãµes, seguranÃ§a, privacidade, acessibilidade, performance, SEO, analytics, testes, infraestrutura, riscos e uma matriz de 36 Ã¡reas do desenvolvimento web.

Ela alinha requisitos. NÃ£o desenvolve o site, nÃ£o cria cÃ³digo de produÃ§Ã£o, nÃ£o instala dependÃªncias, nÃ£o configura serviÃ§os e nÃ£o faz deploy.

## Estrutura

```text
aligning-web-projects/
â”œâ”€â”€ SKILL.md
â”œâ”€â”€ README.md
â”œâ”€â”€ agents/
â”‚   â””â”€â”€ openai.yaml
â””â”€â”€ references/
    â”œâ”€â”€ web-development-areas.md
    â”œâ”€â”€ interview-routing.md
    â””â”€â”€ alignment-brief-template.md
```

## Compatibilidade

O pacote segue o formato de Agent Skills e pode ser usado no Codex e em outros agentes compatÃ­veis com essa especificaÃ§Ã£o. A seleÃ§Ã£o automÃ¡tica estÃ¡ habilitada; a skill tambÃ©m pode ser chamada explicitamente como `$aligning-web-projects`.

## InstalaÃ§Ã£o

Clone o repositÃ³rio para o diretÃ³rio pessoal de skills:

```bash
git clone https://github.com/pyetroschumann18/aligning-web-projects.git ~/.agents/skills/aligning-web-projects
```

No PowerShell do Windows, vocÃª pode usar:

```powershell
git clone https://github.com/pyetroschumann18/aligning-web-projects.git "$env:USERPROFILE\.agents\skills\aligning-web-projects"
```

Depois da instalaÃ§Ã£o, inicie uma nova conversa ou nova execuÃ§Ã£o do agente para atualizar a descoberta de skills.

