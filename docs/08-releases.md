# 8. Releases e Versionamento

Depois que o código foi revisado e integrado à branch principal, o processo ainda não acabou. A entrega precisa ser empacotada e comunicada para os usuários ou para a equipe de infraestrutura. No GitHub, fazemos isso através das Releases.

## O problema
Empresas e equipes frequentemente não sabem exatamente o que foi entregue em um determinado momento. Se um bug crítico surge em produção, fica difícil identificar qual alteração causou o problema se o código não possui uma versão nomeada e congelada.

## A solução: GitHub Releases e SemVer

Uma Release é um "retrato" do código em um ponto específico no tempo, acompanhado de notas sobre o que mudou.

### 8.1 Versionamento Semântico (SemVer)
Recomendamos o uso estrito do Versionamento Semântico (SemVer), que utiliza o formato `MAJOR.MINOR.PATCH` (exemplo: `v2.1.4`).
* **MAJOR (Maior):** Quando você faz mudanças incompatíveis com versões anteriores.
* **MINOR (Menor):** Quando você adiciona funcionalidades de maneira retrocompatível.
* **PATCH (Correção):** Quando você faz correções de bugs retrocompatíveis.

### 8.2 O Processo de Release
1. A equipe encerra a Milestone atual (todas as Issues concluídas).
2. O responsável gera uma nova Release na página inicial do repositório no GitHub.
3. Cria-se uma Tag apontando para o estado atual da `main` (ex: `v1.0.0`).
4. Um Changelog (registro de alterações) é gerado automaticamente ou escrito manualmente, listando as funcionalidades entregues, correções de bugs e contribuintes daquela versão.

### Benefícios x Custos
* **Benefícios:** Comunicação clara com clientes e stakeholders sobre o que há de novo no sistema. Facilidade para reverter (rollback) o sistema inteiro para a versão anterior em caso de falha crítica.
* **Custos:** Demanda que a equipe mantenha o histórico de commits organizado (Conventional Commits ajudam na geração automática de notas da release).
* **Quando dispensar:** Projetos estritamente acadêmicos sem usuários reais e sem necessidade de implantação em servidores.
