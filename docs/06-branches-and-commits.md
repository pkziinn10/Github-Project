# 6. Branches e Commits

O versionamento de código é o coração do trabalho em equipe. Sem padrões, o repositório se torna um labirinto impossível de rastrear.

## O problema
Equipes que comitam tudo diretamente na branch principal enfrentam conflitos constantes, código quebrado em produção e dificuldade para reverter erros. Além disso, mensagens de commit vagas ("arrumei a tela", "teste", "wip") impedem que outros desenvolvedores entendam o histórico do projeto.

## A solução: Git Flow Simplificado e Conventional Commits

Para resolver isso, isolamos o trabalho em desenvolvimento e padronizamos como descrevemos nossas entregas.

### 6.1 Padrão de Branches
O fluxo recomendado é derivado do Git Flow, adaptado para manter a agilidade:

1. A branch `main` representa o código em produção. Ela deve ser bloqueada para commits diretos.
2. Todo desenvolvimento inicia com a criação de uma branch a partir da `main`.
3. Padrão de nomenclatura:
   - `feature/nome-da-tarefa` (para novas funcionalidades)
   - `bugfix/nome-do-erro` (para correções de bugs em desenvolvimento)
   - `hotfix/nome-do-erro` (para correções urgentes diretamente de produção)
   - `docs/nome-da-documentacao` (para alterações exclusivas em documentação)

### 6.2 Padrão de Commits (Conventional Commits)
A mensagem do commit deve explicar o "por quê" e o "o quê", nunca apenas o "como". O padrão de Conventional Commits força essa clareza.

Estrutura básica: `tipo(escopo opcional): descricao breve`

Exemplos:
- `feat: adiciona componente de login na tela inicial`
- `fix: corrige quebra de layout no mobile`
- `docs: atualiza guia de contribuicao`
- `chore: atualiza dependencias do projeto`

### Benefícios x Custos
* **Benefícios:** Histórico claro, facilidade na geração de changelogs automatizados e possibilidade de reverter alterações específicas sem afetar o resto do sistema.
* **Custos:** O desenvolvedor precisa pensar antes de digitar o commit e aprender os prefixos.
* **Quando dispensar:** Não dispensar. Mesmo projetos individuais se beneficiam enormemente de um histórico profissional quando lidos meses depois.
