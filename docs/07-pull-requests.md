# 7. Pull Requests e Revisão de Código

Desenvolver de forma isolada em uma branch é o primeiro passo. O segundo é integrar esse código ao projeto principal com segurança. O Pull Request (PR) é o portão de entrada.

## O problema
Código que entra na branch principal sem revisão geralmente carrega vulnerabilidades, dívidas técnicas ou não atende aos critérios da Issue. Além disso, quando apenas uma pessoa conhece um módulo específico, o projeto sofre se essa pessoa não estiver disponível.

## A solução: PRs como Documentação e Code Review

O PR não deve ser visto apenas como uma etapa burocrática para enviar o código, mas como um pedido de discussão e revisão pelos pares.

### 7.1 Estrutura de um bom Pull Request
Um PR de qualidade deve conter:
1. **Título claro:** Refletindo o impacto final da mudança.
2. **Descrição do que foi feito:** Explicando as decisões técnicas não óbvias.
3. **Vínculo com a Issue:** Utilizar palavras-chave (exemplo: `Closes #12`) para manter o Kanban sincronizado automaticamente.
4. **Evidências:** Imagens, logs ou instruções de como testar a alteração.

### 7.2 O Fluxo de Code Review (Revisão de Código)
O momento da revisão é onde o conhecimento é nivelado entre a equipe.
* **Quem revisa:** Qualquer desenvolvedor pode e deve revisar o código de outro.
* **Postura:** A revisão foca no código, não na pessoa. O objetivo é garantir qualidade, segurança e aprendizado mútuo.
* **Aprovação:** Um PR só pode ser integrado (Merge) após receber o número mínimo de aprovações (Approve) definidos na configuração do repositório.

### Benefícios x Custos
* **Benefícios:** Aumento drástico na qualidade do código, nivelamento de conhecimento da equipe e prevenção de bugs antes da integração.
* **Custos:** Adiciona tempo de espera entre a finalização do código e a entrega efetiva (Lead Time).
* **Quando dispensar:** Em projetos estritamente individuais. No entanto, mesmo sozinho, abrir um PR e ler o próprio código através da tela de revisão ("diff") é uma excelente prática para encontrar erros antes do merge.
