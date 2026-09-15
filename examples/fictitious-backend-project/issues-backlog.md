# Backlog de Issues: Milestone v1.0.0

Abaixo esta o detalhamento de cada Issue planejada para o MVP da TaskFlow API.

---

## Issue #1: feat: criar estrutura inicial do projeto
**Responsavel:** Ana
**Labels:** `enhancement`
**Estimativa:** P (Pequeno)

**Descricao:**
Inicializar o projeto Node.js com as dependencias basicas (Express, dotenv) e criar a estrutura de pastas (src/, routes/, controllers/).

**Criterios de Aceite:**
- [ ] O comando `npm install` roda sem erros.
- [ ] A pasta `src/` contem os diretorios `routes/` e `controllers/`.
- [ ] O servidor sobe na porta configurada via `.env`.

---

## Issue #2: feat: implementar endpoint de criacao de tarefas
**Responsavel:** Bruno
**Labels:** `enhancement`
**Estimativa:** M (Medio)

**Descricao:**
Criar o endpoint `POST /tasks` que recebe um JSON com `title` e `description` e armazena a tarefa em memoria (array simples, sem banco de dados no MVP).

**Criterios de Aceite:**
- [ ] O endpoint retorna status `201 Created` com o objeto da tarefa criada.
- [ ] A tarefa possui um `id` unico gerado automaticamente.
- [ ] O endpoint retorna `400 Bad Request` se o campo `title` estiver ausente.

---

## Issue #3: feat: implementar endpoint de listagem de tarefas
**Responsavel:** Carla
**Labels:** `enhancement`
**Estimativa:** P (Pequeno)

**Descricao:**
Criar o endpoint `GET /tasks` que retorna todas as tarefas armazenadas em memoria.

**Criterios de Aceite:**
- [ ] O endpoint retorna status `200 OK` com um array de tarefas.
- [ ] Se nao houver tarefas, retorna um array vazio.

---

## Issue #4: feat: implementar endpoint de edicao de tarefas
**Responsavel:** Ana
**Labels:** `enhancement`
**Estimativa:** M (Medio)

**Descricao:**
Criar o endpoint `PUT /tasks/:id` que atualiza os campos `title` e `description` de uma tarefa existente.

**Criterios de Aceite:**
- [ ] O endpoint retorna status `200 OK` com o objeto atualizado.
- [ ] O endpoint retorna `404 Not Found` se o `id` nao existir.

---

## Issue #5: feat: implementar endpoint de exclusao de tarefas
**Responsavel:** Bruno
**Labels:** `enhancement`
**Estimativa:** P (Pequeno)

**Descricao:**
Criar o endpoint `DELETE /tasks/:id` que remove uma tarefa existente.

**Criterios de Aceite:**
- [ ] O endpoint retorna status `204 No Content` apos a exclusao.
- [ ] O endpoint retorna `404 Not Found` se o `id` nao existir.

---

## Issue #6: docs: documentar endpoints da API no README
**Responsavel:** Carla
**Labels:** `documentation`
**Estimativa:** P (Pequeno)

**Descricao:**
Atualizar o README do projeto com a lista de endpoints disponiveis, seus metodos HTTP, parametros esperados e exemplos de resposta.

**Criterios de Aceite:**
- [ ] Todos os 4 endpoints (POST, GET, PUT, DELETE) estao documentados.
- [ ] Cada endpoint possui pelo menos um exemplo de requisicao e resposta.
