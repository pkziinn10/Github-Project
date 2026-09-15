# GitHub Project Playbook

Um guia publico, educacional e pratico sobre como organizar e gerenciar projetos de software usando exclusivamente os recursos nativos do GitHub.

---

## Sumario

- [O Problema](#o-problema)
- [Publico-alvo](#publico-alvo)
- [Objetivos](#objetivos)
- [Visao Geral do Fluxo](#visao-geral-do-fluxo)
- [Adocao: Individual vs. Equipe](#adocao-individual-vs-equipe)
- [Principios](#principios)
- [Documentacao](#documentacao)
- [Estrutura do Repositorio](#estrutura-do-repositorio)
- [Status do Projeto](#status-do-projeto)
- [Roadmap](#roadmap)
- [Como Contribuir](#como-contribuir)
- [Licenca](#licenca)
- [Aviso sobre os Exemplos](#aviso-sobre-os-exemplos)

---

## O Problema

Muitos desenvolvedores, equipes e estudantes utilizam o GitHub apenas como uma plataforma de armazenamento de codigo, sem aproveitar seu potencial para o gerenciamento de demandas. O resultado, frequentemente, e a falta de visibilidade, dificuldade de colaboracao e dependencia de ferramentas externas complexas e burocraticas.

Este projeto demonstra que e possivel planejar, executar e entregar software de ponta a ponta sem sair do GitHub.

## Publico-alvo

| Perfil | Exemplo de uso |
|--------|----------------|
| Estudantes universitarios | Projetos academicos e trabalhos de conclusao de curso |
| Desenvolvedores autonomos | Organizacao de projetos pessoais e portfolios |
| Pequenas equipes e startups | Desenvolvimento de MVPs com processos leves |
| Grupos de pesquisa e extensao | Gestao de projetos colaborativos com rastreabilidade |
| Iniciantes no GitHub | Transicao de "repositorio como storage" para gestao completa |

## Objetivos

1. **Educar atraves da pratica:** Ensinar o fluxo de gestao de forma concreta, com exemplos ficticios aplicaveis.
2. **Reduzir ferramentas:** Demonstrar o poder de manter codigo e planejamento no mesmo ecossistema.
3. **Oferecer flexibilidade:** Prover modelos de processos adaptaveis a diferentes tamanhos de equipe.

## Visao Geral do Fluxo

O playbook conecta de forma logica os seguintes elementos nativos do GitHub:

```
Projeto --> Roadmap --> Milestones --> Issues --> GitHub Projects (Kanban) --> Branches --> Pull Requests --> Releases
```

Cada etapa possui um guia dedicado na pasta [`docs/`](./docs), explicando o problema que resolve, o beneficio que oferece, o custo que gera e quando pode ser dispensada.

## Adocao: Individual vs. Equipe

O material oferece dois niveis de adocao para atender diferentes contextos:

| Aspecto | Fluxo Minimo (Individual) | Fluxo Completo (Equipe) |
|---------|---------------------------|-------------------------|
| **Kanban** | To Do, In Progress, Done | Backlog, Ready, In Progress, In Review, Blocked, Done |
| **Branches** | Trabalho direto na `main` ou branches simples | Git Flow com prefixos (`feature/`, `bugfix/`, `hotfix/`) |
| **Commits** | Mensagens claras e descritivas | Conventional Commits obrigatorios |
| **Code Review** | Self-review opcional | Revisao por pares obrigatoria |
| **WIP** | Sem limite formal | 1 issue em andamento por desenvolvedor |
| **Releases** | Opcional | Versionamento Semantico (SemVer) |

## Principios

- **Sem burocracia:** O processo deve facilitar o trabalho, nao atrapalhar.
- **Pragmatismo:** Toda pratica sugerida deve ter uma razao clara para existir.
- **Evolucao continua:** Comece pequeno e adote praticas conforme a necessidade aumenta.
- **Transparencia:** Para cada pratica, o Playbook explica o problema, o beneficio, o custo e quando dispensar.

## Documentacao

### Guias

| # | Documento | Descricao |
|---|-----------|-----------|
| 00 | [Escopo e Principios](./docs/00-scope-and-principles.md) | Limites do MVP, politica de anonimizacao e criterios de inclusao de praticas |
| 01 | [Preparacao do Repositorio](./docs/01-repository-setup.md) | Arquivos essenciais e protecao da branch principal |
| 02 | [Roadmap e Planejamento](./docs/02-project-planning.md) | Como definir o roadmap e usar Milestones para fatiar entregas |
| 03 | [GitHub Projects e Kanban](./docs/03-github-projects.md) | Configuracao do board visual e limites de WIP |
| 04 | [Milestones](./docs/04-milestones.md) | Ciclos de entrega e acompanhamento de progresso |
| 05 | [Issues](./docs/05-issues.md) | Decomposicao de tarefas, labels e regras de ouro |
| 06 | [Branches e Commits](./docs/06-branches-and-commits.md) | Git Flow simplificado e Conventional Commits |
| 07 | [Pull Requests](./docs/07-pull-requests.md) | Estrutura de PRs e fluxo de Code Review |
| 08 | [Releases](./docs/08-releases.md) | Versionamento Semantico e processo de lancamento |
| 09 | [Fluxo Completo](./docs/09-complete-workflow.md) | Mapa unificado do ciclo de vida de uma tarefa |

### Templates

Modelos prontos para copiar e adaptar no seu projeto:

- [`templates/issue/`](./templates/issue/) -- Modelos para reportar bugs e solicitar funcionalidades.
- [`templates/pull-request/`](./templates/pull-request/) -- Modelo de Pull Request com checklist.
- [`templates/milestone/`](./templates/milestone/) -- Guia para planejar e documentar Milestones.
- [`templates/project-fields/`](./templates/project-fields/) -- Colunas e campos recomendados para o Kanban.

### Exemplo Pratico

- [`examples/fictitious-backend-project/`](./examples/fictitious-backend-project/) -- Caso de estudo ficticio completo (TaskFlow API), simulando o fluxo de uma equipe de 3 desenvolvedores ao longo de 4 semanas.

## Estrutura do Repositorio

```
github-project-playbook/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── workflows/
├── assets/
│   └── diagrams/
├── docs/
│   ├── 00-scope-and-principles.md
│   ├── 01-repository-setup.md
│   ├── 02-project-planning.md
│   ├── 03-github-projects.md
│   ├── 04-milestones.md
│   ├── 05-issues.md
│   ├── 06-branches-and-commits.md
│   ├── 07-pull-requests.md
│   ├── 08-releases.md
│   └── 09-complete-workflow.md
├── examples/
│   └── fictitious-backend-project/
├── templates/
│   ├── issue/
│   ├── milestone/
│   ├── project-fields/
│   └── pull-request/
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

## Como Contribuir

Contribuicoes sao bem-vindas. Consulte o arquivo [CONTRIBUTING.md](./CONTRIBUTING.md) para entender o fluxo de envio de melhorias. Leia tambem o nosso [Codigo de Conduta](./CODE_OF_CONDUCT.md) antes de interagir com o projeto.

## Licenca

Este projeto esta licenciado sob a [MIT License](./LICENSE).

---

**Aviso sobre os Exemplos**

Todas as praticas documentadas neste repositorio baseiam-se em aprendizados reais de engenharia e gestao de software. No entanto, todos os dados, codigos e issues apresentados como exemplo sao estritamente ficticios. Nenhuma informacao privada de projetos reais foi utilizada.
