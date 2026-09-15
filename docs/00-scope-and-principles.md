# Escopo e Princípios

Este documento define os limites, critérios e princípios que guiam o desenvolvimento do `GitHub Project Playbook`.

## O que está dentro do escopo
* Utilização de ferramentas nativas do GitHub (Issues, Projects, Milestones, PRs).
* Metodologias ágeis simplificadas adaptadas para ferramentas da plataforma.
* Fluxo de trabalho de versionamento usando Git (baseado no Git Flow e adaptações modernas).
* Exemplos claros de gestão de demandas (do levantamento até o Release).
* Configurações manuais (foco no aprendizado passo a passo na fase inicial).

## O que está fora do MVP
* Scripts de automação ou uso de GitHub Actions.
* Transformação do projeto em Template Repository automático.
* Integrações com plataformas externas (Jira, Trello, Slack).
* Regras rígidas e inflexíveis de metodologia ágil (ex: Scrum "by the book").

## Princípios de Simplicidade
O principal princípio do playbook é a ausência de burocracia desnecessária. Todo processo sugerido aqui será acompanhado das seguintes explicações:
1. Qual problema ele resolve.
2. Qual benefício oferece.
3. Qual custo ou trabalho adicional gera.
4. Quando deve ser utilizado.
5. Quando pode ser dispensado.

## Critérios para adição de novas práticas
Para uma nova prática de gestão ser incluída neste playbook, ela deve:
* Poder ser nativamente suportada pelo GitHub.
* Possuir valor comprovável em projetos reais (seja individual ou para pequenas equipes).
* Não aumentar significativamente a sobrecarga do desenvolvedor.

## Política de Anonimização (Caso SADE)
O playbook utiliza aprendizados reais de engenharia e gestão retirados do desenvolvimento do sistema **SADE**. Contudo, é rigorosamente proibida a menção de dados, trechos de código-fonte reais, nomes de arquiteturas exclusivas ou informações privadas referentes ao projeto SADE. Todos os exemplos citados ao longo do guia deverão ser fictícios ou adaptados com dados públicos de casos genéricos.

## Fluxo Mínimo vs Fluxo Completo
* **Fluxo Mínimo:** Direcionado a projetos pessoais ou acadêmicos solitários. Foco apenas no controle de tarefas e versionamento sem bloqueios (apenas Issues, Branch `main` e Commits).
* **Fluxo Completo:** Para equipes ou projetos maduros. Inclui o Kanban (Projetos), regras de revisão em PRs, limites de tarefas simultâneas (WIP), e uso da estrutura completa de Milestone e Release.

## Definição de Pronto do MVP
O MVP deste repositório será considerado pronto (para atingir seu marco inicial) quando:
1. A fundação estrutural (incluindo README e este documento) estiver implementada.
2. Houver um guia ensinando a configurar manualmente o Kanban (GitHub Projects) e a primeira Milestone.
3. Não existir ferramentas automatizadas ou ações geradas por bots (o usuário deve fazer e compreender o passo a passo manual).
4. O processo inicial puder ser facilmente replicado lendo o repositório.
