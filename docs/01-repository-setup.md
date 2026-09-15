# 1. Preparação do Repositório

Antes de escrever qualquer linha de código, um projeto precisa de uma fundação sólida. Configurar corretamente o repositório garante que o time (ou você mesmo no futuro) tenha clareza sobre como trabalhar, quais são as regras e como o código será integrado.

## O problema
Repositórios criados às pressas tendem a virar "depósitos de código". Sem um `README` claro, sem regras de contribuição e sem proteção de branch, torna-se fácil subir código quebrado para produção ou dificultar a entrada de novos colaboradores.

## A solução nativa no GitHub
O GitHub oferece ferramentas nativas de configuração que resolvem isso em poucos minutos.

### 1.1 Arquivos essenciais
Todo repositório profissional deve conter, no mínimo:
* **README.md:** A porta de entrada. Deve explicar o que é o projeto, como instalá-lo e para que serve.
* **CONTRIBUTING.md:** Define as regras de como enviar código, padrão de commits e uso de branches.
* **LICENSE:** Define os termos de uso do seu código.
* **.gitignore:** Evita que arquivos temporários, senhas e pastas de sistema operacional subam para o repositório.

### 1.2 Proteção da Branch Principal (Branch Protection Rules)
Para evitar incidentes, a branch principal (geralmente `main`) nunca deve receber código diretamente (o famoso *commit na main*).

**Como configurar (Adoção para Equipes):**
1. Vá em `Settings > Branches`.
2. Adicione uma regra para a branch `main`.
3. Marque **Require a pull request before merging**.
4. (Opcional, mas recomendado): Marque **Require approvals** para exigir revisão de código.

### Benefícios x Custos
* **Benefícios:** Organização imediata, redução de erros em produção e integração facilitada de novos membros.
* **Custos:** Leva cerca de 10 a 20 minutos de configuração inicial.
* **Quando dispensar:** Você pode dispensar a proteção de branch (Branch Protection) caso seja um projeto estritamente individual ou acadêmico temporário, onde a agilidade imediata supera o risco de quebra.
