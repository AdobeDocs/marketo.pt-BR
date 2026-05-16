---
description: Saiba como configurar o rastreamento de domínio personalizado para que os links rastreáveis usem o domínio da sua empresa.
title: Como configurar o rastreamento de domínio personalizado
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/gn3uC4uxpwp35IVYcUs-cZJFqbmPc-7vTmgbIPm8lTk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 197
ht-degree: 7%

---

# Como configurar o rastreamento de domínio personalizado {#how-to-set-up-custom-domain-tracking}

O Rastreamento de domínio personalizado permite que sua equipe use o nome da própria empresa em todos os links rastreáveis adicionados aos emails de vendas. Depois que você configurar isso, incluiremos na lista de permissões qualquer link que você tiver no seu email para que apareça como go.yourcompany.com, para que, quando alguém passar o mouse sobre um link, ele leia go.yourcompany.com em vez de go.toutapp.com.

Você precisará da assistência da sua equipe de TI para configurar um registro CNAME para o seu domínio que aponte para go.toutapp.com. Esse CNAME será o que aparece em todos os links de rastreamento (por exemplo, go.yourcompany.com).

Depois de confirmar com sua equipe de TI que o CNAME está configurado corretamente, você pode adicioná-lo à página [!UICONTROL Rastreamento de domínio personalizado] em Ações.

>[!NOTE]
>
>Se o CNAME não estiver configurado corretamente e você ativá-lo como seu domínio personalizado em Ações, ele poderá quebrar os links e pixels de rastreamento.

## Habilitar o rastreamento de domínio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Privilégios de administrador necessários.**

1. Clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Em [!UICONTROL Configurações de Administração], selecione **[!UICONTROL Rastreamento]**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Na guia [!UICONTROL Rastreamento de domínio personalizado], digite seu CNAME e clique em **[!UICONTROL Conectar]**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
