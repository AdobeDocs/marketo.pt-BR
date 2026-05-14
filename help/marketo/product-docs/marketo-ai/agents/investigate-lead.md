---
description: O agente líder de investigação responde às perguntas que os profissionais de marketing fazem com mais frequência. É mais rápido e confiável do que pesquisar manualmente registros de atividades, histórico de campanhas inteligentes e registros de pontuação.
title: Investigar lead
beta: true
hide: true
hidefromtoc: true
source-git-commit: a2c170ced2119a86ffe1f2da1bde212afa4841f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Investigar lead {#investigate-lead}

Descubra por que uma pessoa/cliente potencial específico não atingiu um marco (como MQL, qualificação de programa ou uma campanha) e obtenha uma explicação em linguagem simples do que aconteceu.

>[!PREREQUISITES]
>
>Você deve ter acesso de visualização ao registro de cliente potencial e ao programa ou marco que está investigando.

## Como funciona

Você informa à Marketo AI qual lead você está investigando e qual marco ou resultado você esperava. A Marketo AI verifica o histórico de atividades do lead, o registro de pontuação, a associação ao programa, o histórico de qualificação de campanha inteligente e quaisquer filtros ou regras de supressão relevantes. Em seguida, ele retorna uma explicação clara do que bloqueou ou atrasou o resultado esperado — por exemplo, &quot;A pontuação deste lead atingiu 48, mas o limite MQL é 50&quot; ou &quot;Este lead foi excluído da campanha porque a subscrição foi cancelada em 3 de março&quot;.

## Como usar {#how-to-use}

1. Em Minha Marketo, clique no bloco **Criar com IA**.

1. Na janela do prompt, descreva o que você está investigando. Inclua o cliente potencial (por email ou nome) e o que você esperava que acontecesse.

>[!NOTE]
>
>Exemplos: &quot;Por que `john.smith@example.com` não atingiu o MQL no mês passado?&quot; ou &quot;Por que Brenda Gonzales não foi adicionada ao programa de webinário do terceiro trimestre?&quot;

1. A IA do Marketo traz o histórico do lead e de relevância.

1. Revise a explicação. A IA do Marketo informa o motivo específico pelo qual a etapa não foi atingida e, quando possível, o que precisaria ser alterado para o lead ser qualificado.

1. Realize uma ação com base na conclusão: corrija um problema de dados, ajuste um filtro, atualize a pontuação do lead ou aceite que o resultado foi correto.

## Exemplos

**Limite de MQL não atingido**
Um gerente de geração de demanda percebe um lead que as vendas sinalizaram como interessadas, mas que nunca atingiram a MQL. Ela pergunta: &quot;Por que o david.chen@techcorp.com não chegou ao MQL?&quot; A Marketo AI descobre que a pontuação comportamental do lead é 42 (8 pontos abaixo do limite MQL de 50) e lista as atividades de pontuação que contribuíram. Ela pode ver exatamente quais comportamentos empurrariam a liderança acima do limiar.

**Ignorar campanha devido à supressão**
Um gerente de campanha pergunta por que um contato específico não recebeu um email de convite que foi para o restante da lista. A IA do Marketo descobre que o contato está na lista de marketing suspenso, o que os exclui automaticamente de todos os envios de campanha. O gerente entra em contato diretamente com o contato para investigar por que ele foi suprimido.

**Falha na qualificação do programa**
Um especialista em operações de marketing está solucionando por que um lead que participou de um webinário não foi adicionado ao programa de acompanhamento pós-evento. A IA do Marketo rastreia o problema: o lead foi registrado, mas foi marcado como &quot;Não aparecer&quot; no programa do evento, e o filtro de campanha de acompanhamento requer o status &quot;Presente&quot;. O status foi definido incorretamente na integração.

**Chumbo preso em uma estrutura**
Um gerente de geração de demanda percebe que um lead está na mesma fase de criação por 90 dias, sem progressão. Ela pede que a Marketo AI investigue. Ele descobre que a pontuação de engajamento do lead caiu abaixo do limite necessário para avançar para o próximo estágio e que o lead não abriu um email em 60 dias — qualificando-os para a ramificação de reengajamento.

## Dicas e limitações

* A investigação de lead explica o que aconteceu com base na atividade e configuração gravadas da Marketo — ela não pode explicar as decisões tomadas fora do Marketo (por exemplo, por que um lead foi removido manualmente por um colega).
* Se o histórico de atividades de um lead for muito longo, a IA do Marketo se concentra nos eventos mais recentes e relevantes relacionados à sua pergunta.
* A Investigação de Cliente Potencial é somente leitura. Ela informará o que aconteceu, mas não fará alterações no registro de cliente potencial ou na associação ao programa.
* Para problemas que resultam em problemas de qualidade de dados (valores de campo ausentes, fonte de cliente potencial incorreta), a correção precisará ser feita manualmente no registro de cliente potencial.
* Se a investigação revelar um problema de lógica de campanha inteligente que afete muitos clientes potenciais, use o Controle de qualidade do programa para analisar a configuração completa do programa.
