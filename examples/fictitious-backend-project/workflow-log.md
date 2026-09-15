# Registro do Fluxo de Trabalho: Milestone v1.0.0

Este documento simula o dia a dia da equipe ficticia durante o desenvolvimento do MVP, demonstrando como cada pratica do Playbook foi aplicada.

---

## Semana 1

### Ana inicia a Issue #1
1. Ana atribui a Issue #1 a si mesma e move o card para "In Progress".
2. Cria a branch: `git checkout -b feature/project-setup`
3. Configura a estrutura inicial do projeto.
4. Commit: `git commit -m "feat: add initial project structure with express"`
5. Sobe a branch: `git push -u origin feature/project-setup`
6. Abre o PR com a descricao: "Closes #1"
7. Move o card para "In Review".

### Bruno revisa o PR da Ana
1. Bruno analisa o codigo no PR.
2. Sugere adicionar um arquivo `.env.example` para facilitar a configuracao.
3. Ana aplica a sugestao e faz novo commit: `git commit -m "chore: add .env.example file"`
4. Bruno aprova o PR.
5. Ana faz o merge na `main`. A Issue #1 e fechada automaticamente.
6. O card vai para "Done".

---

## Semana 2

### Bruno inicia a Issue #2
1. Bruno move a Issue #2 para "In Progress".
2. Cria a branch: `git checkout -b feature/create-task-endpoint`
3. Implementa o endpoint POST /tasks.
4. Commit: `git commit -m "feat: add POST /tasks endpoint with validation"`
5. Abre o PR: "Closes #2"

### Carla inicia a Issue #3 (em paralelo)
1. Carla move a Issue #3 para "In Progress".
2. Cria a branch: `git checkout -b feature/list-tasks-endpoint`
3. Implementa o endpoint GET /tasks.
4. Commit: `git commit -m "feat: add GET /tasks endpoint"`
5. Abre o PR: "Closes #3"

### Revisoes cruzadas
- Carla revisa o PR do Bruno (Issue #2). Aprovado.
- Bruno revisa o PR da Carla (Issue #3). Aprovado.
- Ambos os PRs sao integrados na `main`.

**Observacao:** Note que nenhum desenvolvedor ficou com mais de 1 issue em "In Progress". Isso respeita o limite de WIP acordado.

---

## Semana 3

### Ana inicia a Issue #4
1. Branch: `git checkout -b feature/edit-task-endpoint`
2. Commit: `git commit -m "feat: add PUT /tasks/:id endpoint"`
3. PR: "Closes #4". Revisado e aprovado por Carla.

### Bruno inicia a Issue #5
1. Branch: `git checkout -b feature/delete-task-endpoint`
2. Commit: `git commit -m "feat: add DELETE /tasks/:id endpoint"`
3. PR: "Closes #5". Revisado e aprovado por Ana.

---

## Semana 4

### Carla inicia a Issue #6
1. Branch: `git checkout -b docs/api-documentation`
2. Commit: `git commit -m "docs: add API endpoints documentation to README"`
3. PR: "Closes #6". Revisado e aprovado por Bruno.

### Encerramento da Milestone
1. Todas as 6 Issues estao fechadas.
2. A barra de progresso da Milestone marca 100%.
3. A equipe fecha a Milestone no GitHub.

### Geracao da Release
1. Ana cria a tag: `git tag v1.0.0`
2. Sobe a tag: `git push origin v1.0.0`
3. Na aba "Releases" do GitHub, cria a Release `v1.0.0 - MVP` com as seguintes notas:

```
## v1.0.0 - MVP

### Adicionado
- Endpoint POST /tasks para criacao de tarefas.
- Endpoint GET /tasks para listagem de tarefas.
- Endpoint PUT /tasks/:id para edicao de tarefas.
- Endpoint DELETE /tasks/:id para exclusao de tarefas.
- Documentacao dos endpoints no README.

### Contribuidores
- Ana (setup, edicao)
- Bruno (criacao, exclusao)
- Carla (listagem, documentacao)
```

---

**Fim do ciclo.** A equipe esta pronta para planejar a Milestone v1.1.0, que incluira autenticacao de usuarios e filtros avancados.
