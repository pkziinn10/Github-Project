# Template: Colunas do Kanban (GitHub Projects)

Use este documento como referencia para configurar o board do seu projeto no GitHub Projects. As colunas abaixo representam o fluxo recomendado pelo Playbook, mas podem ser adaptadas conforme a realidade da sua equipe.

---

## Fluxo Completo (Equipes)

| Coluna | Descricao | Regra |
|--------|-----------|-------|
| **Backlog** | Ideias, bugs e tarefas futuras que ainda nao foram priorizadas. | Sem limite. Qualquer membro pode adicionar. |
| **Ready** | Issues analisadas, priorizadas e vinculadas a Milestone atual. Prontas para serem iniciadas. | Manter no maximo 2x o numero de desenvolvedores. |
| **In Progress** | O desenvolvedor assumiu a tarefa e esta trabalhando nela. | Limite de WIP: 1 issue por desenvolvedor. |
| **In Review** | O codigo foi enviado via Pull Request e aguarda revisao. | O autor nao deve revisar o proprio PR (exceto em projetos individuais). |
| **Blocked** | A tarefa nao pode avancar por causa de uma dependencia externa ou duvida tecnica. | Adicionar um comentario na Issue explicando o motivo do bloqueio. |
| **Done** | A tarefa foi concluida, o PR foi integrado e a Issue foi fechada. | Nao mover manualmente; o GitHub fecha automaticamente ao usar `Closes #N`. |

---

## Fluxo Minimo (Individual)

| Coluna | Descricao |
|--------|-----------|
| **To Do** | Tarefas planejadas para a iteracao atual. |
| **In Progress** | Tarefa em andamento. Limite: 1 por vez. |
| **Done** | Tarefa concluida. |

---

## Campos Personalizados Recomendados

Alem das colunas, o GitHub Projects permite adicionar campos personalizados. Sugerimos:

| Campo | Tipo | Descricao |
|-------|------|-----------|
| **Prioridade** | Single Select | Alta, Media, Baixa |
| **Estimativa** | Single Select | P (Pequeno), M (Medio), G (Grande) |
| **Tipo** | Single Select | Bug, Feature, Docs, Chore |
