# 9. Fluxo de Trabalho Completo

Este documento serve como um mapa mental (cheat sheet) de tudo o que foi abordado no Playbook, unificando as práticas em um único fluxo temporal lógico.

## O Ciclo de Vida de uma Tarefa

Abaixo, detalhamos o fluxo desde a concepção de uma ideia até a sua entrega ao usuário final.

### Passo 1: Planejamento (Planejar)
1. O gestor ou equipe define uma **Milestone** com objetivo claro e prazo fechado.
2. Requisitos são decompostos em **Issues** atômicas (esforço máximo de 2 dias).
3. As Issues ganham **Labels** (`enhancement`, `bug`) e são vinculadas à Milestone.
4. As Issues repousam na coluna "Backlog" ou "Ready" do **GitHub Projects (Kanban)**.

### Passo 2: Execução (Desenvolver)
1. O desenvolvedor atribui a Issue a si mesmo (Assignee) e a move para a coluna "In Progress".
2. Verifica-se o **Limite de WIP**: o desenvolvedor só pode ter uma tarefa nesta coluna.
3. Cria-se uma branch específica usando o padrão Git Flow: `git checkout -b feature/nome-da-tarefa`.
4. O código é escrito.
5. Os commits são salvos utilizando **Conventional Commits**: `git commit -m "feat: adiciona..."`.

### Passo 3: Revisão (Inspecionar)
1. O desenvolvedor sobe a branch e abre um **Pull Request (PR)** contra a branch `main`.
2. A descrição do PR contém o fechamento automático: `Closes #numero_da_issue`.
3. O card no Kanban é movido para "In Review".
4. Outro membro da equipe faz o **Code Review**. Sugere mudanças ou aprova.

### Passo 4: Integração e Entrega (Lançar)
1. O PR é aprovado e o **Merge** é executado na branch `main`.
2. A Issue vinculada é fechada automaticamente e o card vai para a coluna "Done" no Kanban.
3. Ao fim da iteração, quando todas as tarefas da Milestone estão prontas, a Milestone é fechada.
4. Gera-se uma **Release** seguindo o **SemVer** (ex: `v1.1.0`), encapsulando todas as entregas do ciclo.

---
**Fim do ciclo.** A equipe está pronta para debater a próxima Milestone e repetir o fluxo, com total visibilidade, segurança e ausência de burocracias externas.
