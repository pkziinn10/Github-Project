# 3. GitHub Projects e Kanban

Apenas listar tarefas em uma interface não é gestão ágil. Para realmente entender o ritmo do projeto e onde os gargalos estão, precisamos de visibilidade. O GitHub Projects fornece um Kanban integrado que resolve isso.

## O problema
Equipes perdem o controle do que está sendo feito. Desenvolvedores assumem múltiplas tarefas simultaneamente (o que causa perda de foco e atrasos), e gerentes não conseguem saber o que está travado ou aguardando revisão.

## A solução: Board Visual e Fluxo Simples
Um Kanban bem configurado no GitHub atua como o ponto central de verdade (Single Source of Truth) do projeto.

### 3.1 Estrutura de Colunas (Fluxo para Equipes)
Para uma equipe pequena ou média, sugerimos o fluxo de 6 etapas:

1. **Backlog:** Ideias, bugs relatados e tarefas futuras. Não possuem prazo imediato.
2. **Ready (Pronto para Iniciar):** Tarefas que já foram analisadas, priorizadas e estão ligadas à Milestone atual.
3. **In Progress (Em Andamento):** O desenvolvedor assumiu a tarefa e está codificando.
4. **In Review (Em Revisão):** O código foi enviado via Pull Request e aguarda análise de outro membro.
5. **Blocked (Bloqueado):** Tarefas que não podem avançar devido a uma dependência externa ou dúvida técnica pendente.
6. **Done (Concluído):** A tarefa está finalizada e integrada na branch principal.

### 3.2 O Limite de WIP (Work in Progress)
O conceito mais importante do Kanban não é mover cartões, mas sim **limitar o trabalho em andamento**.
* **A regra:** Cada desenvolvedor só pode ter **1 (uma)** Issue na coluna "In Progress" por vez.
* **Por que?** Iniciar muitas tarefas dá a falsa sensação de velocidade. Terminar tarefas é o que entrega valor. Se um desenvolvedor está travado, ele deve ajudar a destravar tarefas em "In Review" ou "Blocked" antes de puxar algo novo do "Ready".

### Benefícios x Custos
* **Benefícios:** Redução drástica no tempo de entrega (Lead Time), equipe mais focada e prevenção de sobrecarga individual.
* **Custos:** Exige disciplina da equipe para não furar o limite de WIP e manter os cartões atualizados.
* **Quando dispensar:** Projetos estritamente individuais podem simplificar o board apenas para "To Do", "In Progress" e "Done", dispensando as colunas de bloqueio e revisão.
