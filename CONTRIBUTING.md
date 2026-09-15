# Como Contribuir

Obrigado pelo seu interesse em melhorar o `GitHub Project Playbook`! Queremos que colaborar com este projeto seja uma experiência simples e educativa.

Para manter o fluxo organizado e nos padrões do repositório, por favor, siga o guia de colaboração abaixo:

## Fluxo de Contribuição Inicial

**1. Escolher ou criar uma Issue**
Antes de iniciar qualquer código ou modificação documental, verifique se já existe uma [Issue](https://github.com/pkziinn10/Github-Project/issues) relatando o que você deseja fazer. Se não houver, crie uma nova Issue explicando o problema ou melhoria proposta. Aguarde o alinhamento com a manutenção do repositório.

**2. Criar uma Branch**
Para iniciar seu trabalho, crie uma branch a partir da branch principal (`main`). Dê um nome descritivo para sua branch.
```bash
git checkout main
git pull origin main
git checkout -b feature/sua-melhoria
```
*(Nota: Sempre priorizaremos o uso de práticas profissionais de versionamento, inspiradas nos conceitos de Git Flow).*

**3. Fazer Commits Claros**
Seus commits devem ser atômicos (um assunto por vez) e seguir um padrão descritivo e claro, preferencialmente utilizando [Conventional Commits](https://www.conventionalcommits.org/).
Exemplo:
```bash
git commit -m "docs: adiciona secao sobre limites de wip no README"
```

**4. Abrir um Pull Request (PR)**
Quando terminar, suba a branch para o repositório remoto e abra um Pull Request detalhado. Explique o contexto, o que foi alterado e como a alteração soluciona a Issue proposta.

**5. Vincular o PR à Issue**
No corpo do seu Pull Request, utilize as palavras-chave do GitHub para fechar automaticamente a Issue correspondente assim que o PR for aprovado e mergeado.
Exemplo: `Closes #12`.

---
Qualquer alteração será avaliada com base nos nossos princípios de simplicidade e na política de privacidade de nossos casos de estudo base. Agradecemos sua ajuda!
