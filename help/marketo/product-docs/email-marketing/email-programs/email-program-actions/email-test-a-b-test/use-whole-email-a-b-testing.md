---
unique-page-id: 2359502
description: Saiba como executar testes A/B de email completo. Teste diferentes versões de email e escolha um vencedor de acordo com os critérios escolhidos.
title: Usar teste A/B de “Email inteiro”
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/P6YTdfoKe0D8egqK5amG2GTM92U7RZ1AWoQh6NcZpeQ'
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
source-wordcount: '286'
ht-degree: 4%
---
# Usar teste A/B de “Email inteiro” {#use-whole-email-a-b-testing}

Você pode facilmente testar seus emails A/B. Um grande teste é o teste **Todo o email**. Veja como configurar isso.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. No bloco Email, com seu email selecionado, clique em **[!UICONTROL Adicionar Teste A/B]**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Uma nova janela é aberta. Clique no menu suspenso **[!UICONTROL Tipo de teste]** e selecione **[!UICONTROL Emails inteiros]**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Se você tiver informações de teste anteriores (como um teste de assunto), clique com segurança em **[!UICONTROL Redefinir Teste]**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Selecione seu primeiro email.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Clique em **[!UICONTROL Adicionar]** para aplicar o email.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Você pode adicionar vários emails. No entanto, se você adicionar muitos, isso poderá retardar o processo de teste.

1. Selecione o segundo email.

   [&#128279;](assets/image2014-9-12-15-3a23-3a49.png)

1. Clique em **[!UICONTROL Adicionar]** para aplicar o segundo email. Arraste o controle deslizante para escolher qual porcentagem do público-alvo você deseja receber o teste A/B e clique em **[!UICONTROL Avançar]**.

   [&#128279;](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >As diferentes variações enviarão partes iguais do **Tamanho da Amostra de Teste** escolhido.

   >[!CAUTION]
   >
   >**Recomendamos evitar definir o tamanho da amostra como 100%**. Se você estiver usando uma lista estática, definir o tamanho da amostra como 100% enviará o email para todos no público-alvo e o vencedor não descontará para ninguém. Se você estiver usando uma lista **inteligente**, definir o tamanho da amostra como 100% enviará o email para todos no público-alvo _nesse momento_. Quando o programa de email for executado novamente em uma data posterior, qualquer nova pessoa qualificada para a lista inteligente também receberá o email, pois agora está incluída no público.

   Ok, estamos quase lá. Agora precisamos [definir o critério do vencedor do teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
