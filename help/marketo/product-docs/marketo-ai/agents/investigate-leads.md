---
description: O agente líder de investigação responde às perguntas que os profissionais de marketing fazem com mais frequência. É mais rápido e confiável do que pesquisar manualmente registros de atividades, histórico de campanhas inteligentes e registros de pontuação.
title: Investigar clientes em potencial
source-git-commit: 3f7d17870cf0d60c716095ae200c003fc8ff0e28
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Investigar clientes em potencial {#investigate-leads}

Descubra por que uma pessoa/cliente potencial específico não atingiu um marco (como MQL, qualificação de programa ou uma campanha) e obtenha uma explicação em linguagem simples do que aconteceu.

>[!PREREQUISITES]
>
>* Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>
>* Você deve ter acesso de visualização ao registro de pessoa/cliente potencial e ao programa ou marco que está investigando.

>[!AVAILABILITY]
>
>No momento, esse recurso está na versão beta fechada. Não divulgue esta documentação.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **IA do Marketo**.

1. Na janela do prompt, descreva o que você está investigando. Inclua o cliente potencial (por email ou nome) e o que você esperava que acontecesse.

   >[!NOTE]
   >
   >Exemplos: &quot;Por que `john.smith@example.com` não atingiu o MQL no mês passado?&quot; ou &quot;Por que Sato Hanako não foi adicionado ao programa do webinário do terceiro trimestre?&quot;

1. A IA do Marketo traz o histórico do lead e de relevância.

1. Revise a explicação. A IA do Marketo informa o motivo específico pelo qual a etapa não foi atingida e, quando possível, o que precisaria ser alterado para o lead ser qualificado.

1. Realize uma ação com base na conclusão: corrija um problema de dados, ajuste um filtro, atualize a pontuação do lead ou aceite que o resultado foi correto.

## Casos de uso {#use-cases}

**Limite de MQL não atingido**: um gerente de geração de demanda percebe um cliente potencial que as vendas sinalizaram como interessado, mas que nunca atingiu o MQL. Eles perguntam: &quot;Por que `david.chen@techcorp.com` não chegou ao MQL?&quot; A Marketo AI descobre que a pontuação comportamental do lead é 42 (8 pontos abaixo do limite MQL de 50) e lista as atividades de pontuação que contribuíram. Eles podem ver exatamente quais comportamentos empurrariam o lead acima do limite.

**Ignorar campanha devido à supressão**: um gerente de campanha pergunta por que um contato específico não recebeu um email de convite que foi para o restante da lista. A IA do Marketo descobre que o contato está na lista de marketing suspenso, o que os exclui automaticamente de todos os envios de campanha. O gerente entra em contato com eles diretamente para investigar por que eles foram suprimidos.

**Falha na qualificação do programa**: um especialista em operações de marketing está solucionando o motivo pelo qual um cliente potencial que participou de um webinário não foi adicionado ao programa de acompanhamento pós-evento. A IA do Marketo rastreia o problema: o lead foi registrado, mas foi marcado como &quot;Não aparecer&quot; no programa do evento, e o filtro de campanha de acompanhamento requer o status &quot;Presente&quot;. O status foi definido incorretamente na integração.

## Itens a serem observados {#things-to-note}

* Investigação de lead explica o que aconteceu com base na atividade e configuração registradas da Marketo. Ele não pode explicar decisões tomadas fora do Marketo (por exemplo, por que um lead foi removido manualmente por um colega).
* Se o histórico de atividades de um lead for muito longo, a IA do Marketo se concentra nos eventos mais recentes e relevantes relacionados à sua pergunta.
* A investigação de lead é somente leitura. Ele informa o que aconteceu, mas não faz alterações no registro principal ou na associação ao programa.
* Para problemas que resultam em problemas de qualidade de dados (valores de campo ausentes, fonte de cliente potencial incorreta), a correção deve ser feita manualmente no registro de cliente potencial.
* Se a investigação revelar um problema de lógica de campanha inteligente que afete muitos clientes potenciais, use o Controle de qualidade do programa para analisar a configuração completa do programa.
