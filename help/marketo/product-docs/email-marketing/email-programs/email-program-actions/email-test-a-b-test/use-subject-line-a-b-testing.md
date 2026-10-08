---
unique-page-id: 2359494
description: Saiba como executar testes A/B da linha de assunto em programas de email. Teste diferentes linhas de assunto e escolha um vencedor por desempenho.
title: Usar teste A/B de “Linha de assunto”
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/jF6mldDXXbl9YOWTOfwgvxvbh-QmIH6sqnnELOv1lxQ'
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
source-wordcount: '255'
ht-degree: 4%
---
# Usar teste A/B de “Linha de assunto” {#use-subject-line-a-b-testing}

Você pode facilmente testar seus emails A/B. Um dos testes mais comuns é o teste **[!UICONTROL Linha de assunto]**.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. No **[!UICONTROL Bloco de emails]**, com seu email selecionado, clique em **[!UICONTROL Adicionar Teste A/B]**.

![](assets/image2014-9-12-15-3a6-3a2.png)

1. A janela do editor de teste será aberta. Insira uma ou mais novas linhas de assunto.

   >[!NOTE]
   >
   >A opção **A** será preenchida previamente com as informações contidas no email selecionado.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Você pode clicar em **+** para adicionar mais linhas de assunto.

1. Use o controle deslizante para escolher qual porcentagem do público-alvo você deseja receber o teste A/B e clique em **[!UICONTROL Avançar]**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Recomendamos evitar definir o tamanho da amostra como 100%**. Se você estiver usando uma lista estática, definir o tamanho da amostra como 100% enviaria o email para todos no público-alvo e o vencedor não iria para ninguém. Se você estiver usando uma lista inteligente, definir o tamanho da amostra como 100% enviará o email para todos no público-alvo _nesse momento_. E quando o programa de email for executado novamente em uma data posterior, qualquer nova pessoa que se qualificar para a lista inteligente também receberá o email, já que agora está incluída no público.

   >[!NOTE]
   >
   >As diferentes variações de assunto levarão até mesmo partes do Tamanho da amostra de teste selecionado.

   Ok, estamos quase lá. Agora precisamos [definir o critério do vencedor do teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
