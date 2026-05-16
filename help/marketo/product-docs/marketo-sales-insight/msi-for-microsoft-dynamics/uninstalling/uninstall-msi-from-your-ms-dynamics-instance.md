---
unique-page-id: 37355600
description: Saiba como desinstalar o Marketo Sales Insight da instância do MS Dynamics. Remova a solução e limpe-a quando necessário.
title: 'Desinstalar o MSI da instância do MS [!DNL Dynamics] '
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/tv5uoDyp6czOdjx3D1RDZUtoDTaaZniVF5fZDWnxPPk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 155
ht-degree: 0%

---

# Desinstalar o MSI da instância do MS [!DNL Dynamics] {#uninstall-msi-from-your-ms-dynamics-instance}

Para desinstalar o MSI da instância do MS [!DNL Dynamics], você precisará executar etapas no Marketo e no MS [!DNL Dynamics].

>[!PREREQUISITES]
>
>[Desabilitar MS [!DNL Dynamics] Sincronização](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) Global

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Clique em **[!UICONTROL Sales Insight]**.

   ![](assets/six.png)

1. Clique em **[!UICONTROL Editar sincronização de campo]**.

   ![](assets/seven.png)

1. Marque a caixa de seleção **[!UICONTROL Desabilitar sincronização]** e clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >Certifique-se de [desabilitar a Sincronização Global do MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) antes de desabilitar a sincronização de campo.

   ![](assets/eight.png)

## As seguintes etapas ocorrem na instância do MS [!DNL Dynamics]: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Clique em **[!UICONTROL Configurações avançadas]**.

1. Clique em **[!UICONTROL Soluções]**.

1. Selecione **[!UICONTROL Marketo Sales Insight]** e clique no ícone excluir.

1. Quando o modal Desinstalar Solução aparecer, clique em **[!UICONTROL OK]**.

   Geralmente leva cerca de 20 minutos para que a solução MS [!DNL Dynamics] seja totalmente desinstalada. No entanto, se você tiver uma instância grande do MS [!DNL Dynamics], pode demorar um pouco mais.

   >[!NOTE]
   >
   >Lembre-se de ativar a sincronização Global do MS [!DNL Dynamics] depois de desinstalar o MSI.
