# 5. Issues e Decomposição de Tarefas

Se as Milestones definem a visão estratégica, as Issues são o campo de batalha. É aqui que o trabalho real é documentado, debatido e rastreado.

## O problema
Tarefas descritas de forma vaga (ex: "Arrumar tela de login") ou tarefas gigantes que duram semanas sem gerar entrega (ex: "Refazer todo o backend"). Isso paralisa o Kanban e torna impossível a revisão de código.

## A solução: Decomposição e Clareza
Uma Issue deve ser pequena o suficiente para ser compreendida em minutos e executada em poucas horas ou poucos dias.

### 5.1 A Estrutura de uma Boa Issue
1. **Título direto:** O que precisa ser feito.
2. **Contexto:** Por que isso é necessário.
3. **Critérios de Aceite:** Um checklist simples do que deve funcionar para a tarefa ser considerada concluída.

### 5.2 Regras de Ouro para a Equipe
* **Uma Issue, um Pull Request:** O trabalho deve ser atômico. Não resolva três Issues no mesmo código.
* **Tamanho Máximo:** Se uma Issue parece que levará mais de 2 ou 3 dias, quebre-a em duas Issues menores. Entregas pequenas e constantes trazem menos bugs.
* **Tudo nasce como Issue:** Se não há Issue, não deve haver branch sendo desenvolvida.

### 5.3 O Uso de Labels
As labels organizam as Issues no Kanban. Recomendamos um padrão minimalista:
* `bug`: Algo está quebrado.
* `enhancement`: Nova funcionalidade ou melhoria.
* `documentation`: Alterações em manuais e READMEs.
* `good first issue`: Tarefas fáceis para novos contribuidores.

### Benefícios x Custos
* **Benefícios:** Transparência total. Qualquer membro sabe o que fazer e qual o critério de pronto. Facilita o code review.
* **Custos:** Requer dedicação na escrita antes de programar.
* **Quando dispensar:** Jamais dispense. Mesmo em projetos de uma só pessoa, registrar o que precisa ser feito mantém a sanidade ao longo dos meses.
