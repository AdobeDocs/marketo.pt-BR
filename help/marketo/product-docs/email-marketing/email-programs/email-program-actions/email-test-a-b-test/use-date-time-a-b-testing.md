---
unique-page-id: 2359520
description: Saiba como executar testes A/B de data/hora para programas de email. Teste diferentes horários de envio e escolha um vencedor por desempenho.
title: Usar teste A/B de “Data/Hora”
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/V3lRJlUSegVZJbrhyPJRAKopziqMdmpseC16EFLGzrU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: 69a7f8d6-582c-5b66-841e-32cf07fd164c
    internal-label: A/B Testing
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 4%
---
# Usar teste A/B de “Data/Hora” {#use-date-time-a-b-testing}

Você pode facilmente testar seus emails A/B. Um teste é o teste **[!UICONTROL Date/Time]**. Isso testa a hora do dia ou o dia da semana mais adequada para enviar emails. Veja como configurar isso.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. No bloco **[!UICONTROL Email]**, clique em **[!UICONTROL Adicionar Teste A/B]**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Uma nova janela é aberta. Selecione **[!UICONTROL Data/Hora]** para **[!UICONTROL Tipo de Teste]**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Se você tiver informações de teste anteriores (como um teste de assunto), clique com segurança em **[!UICONTROL Redefinir Teste]**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Selecione a data da primeira data/hora.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Selecione a hora para sua primeira data/hora.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Faça o mesmo para a segunda data/hora.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Use o controle deslizante para escolher qual porcentagem do público-alvo você deseja no teste A/B e clique em **[!UICONTROL Avançar]**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >As diferentes variações aplicam-se a porções iguais do tamanho escolhido da amostra para ensaio.

   >[!CAUTION]
   >
   >**Recomendamos evitar definir o tamanho da amostra como 100%**. Se você estiver usando uma lista estática, definir o tamanho da amostra como 100% enviará o email para todos no público-alvo e o vencedor não descontará para ninguém. Se você estiver usando uma lista **inteligente**, definir o tamanho da amostra como 100% enviará o email para todos no público-alvo _nesse momento_. Quando o programa de email for executado novamente em uma data posterior, qualquer nova pessoa qualificada para a lista inteligente também receberá o email, pois agora está incluída no público.

   Certo, estamos um passo mais perto. Agora precisamos [definir o critério do vencedor do teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
