---
unique-page-id: 2359520
description: Use o teste A/B "Data/Hora" - Documentos da Marketo - Documentação do produto
title: Usar o teste A/B de "Data/Hora"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Usar o teste A/B de &quot;Data/Hora&quot; {#use-date-time-a-b-testing}

Você pode facilmente testar seus emails em A/B. Um teste é **Data/Hora** teste. Isso testa a hora do dia ou o dia da semana que é melhor para enviar emails. Veja como configurar.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Em **Email** bloco, clique em **Adicionar teste A/B**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Uma nova janela é aberta. Selecionar **Data/Hora** para **Tipo de teste**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Se você tiver informações de teste anteriores (como um teste de assunto), poderá clicar com segurança em **Redefinir teste**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Selecione a data da primeira data/hora.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Selecione a hora da primeira data/hora.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Faça o mesmo para a segunda data/hora.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Use o controle deslizante para escolher qual porcentagem do público-alvo deseja em seu teste A/B e clique em **Próximo**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >As diferentes variações aplicar-se-ão a partes iguais do tamanho de amostra de ensaio escolhido.

   >[!CAUTION]
   >
   >**Recomendamos que você evite definir o tamanho da amostra como 100%**. Se você estiver usando uma lista estática, definir o tamanho da amostra como 100% envia o email para todos no público-alvo e o vencedor não vai para ninguém. Se estiver usando um **inteligente** , definir o tamanho da amostra como 100% envia o email para todos no público-alvo _nessa altura_. Quando o programa de email for executado novamente em uma data posterior, qualquer pessoa nova qualificada para a lista inteligente também receberá o email, pois agora está incluída no público.

   Ok, estamos um passo mais perto. Agora precisamos [definir os critérios do vencedor do teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
