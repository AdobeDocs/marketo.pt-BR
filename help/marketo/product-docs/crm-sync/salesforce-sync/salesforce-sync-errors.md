---
description: Saiba como visualizar e filtrar erros de sincronização do Salesforce no Marketo. Consulte falhas no nível de registro e no nível de trabalho e use detalhes de erros para solucionar problemas de sincronização.
title: Erros de sincronização do Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/vEPgjXh8QKyzC1AiAhRqf4tF-MZpu9GETxrRAJHYVIo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 197
ht-degree: 7%

---

# [!DNL Salesforce] Erros de sincronização {#salesforce-sync-errors}

Visualize um resumo dos erros encontrados durante o processo de sincronização. Isso inclui erros causados por falhas na sincronização de dados incompatíveis.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

## Exibir Erros de Sincronização {#view-sync-errors}

1. Clique em **[!UICONTROL Administrador]**.

   ![](assets/salesforce-sync-errors-1.png)

1. Em Integração, clique em **Salesforce** e, em seguida, na guia **[!UICONTROL Erros de Sincronização]**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Os erros listados variam da hora atual até cinco dias antes da sincronização atual.

| Campo | Descrição |
|---|---|
| Falha em | Nível de Registro _ou_ Nível de Trabalho |
| Data/hora da falha | Detalhes do erro |
| Tipo de erro | Mensagem de retorno do SFDC |

>[!TIP]
>
>Clicar no registro de nível de registro mostra a Marketo e as [!DNL Salesforce] IDs do objeto relacionado. Em alguns casos, a mensagem no registro e os erros de nível de trabalho são diretamente de [!DNL Salesforce]. A pesquisa on-line pode fornecer detalhes adicionais.

## Filtrar erros de sincronização {#filter-sync-errors}

1. Para filtrar os dados, clique no ícone de filtro na extremidade direita da página.

   ![](assets/salesforce-sync-errors-3.png)

1. Selecione o intervalo de data e hora e filtre por Tipo de erro (Nível da tarefa ou Nível de registro). Clique em **[!UICONTROL Aplicar]** quando terminar.

   ![](assets/salesforce-sync-errors-4.png)

**ETAPA OPCIONAL**: para exportar erros de sincronização, clique em **[!UICONTROL Exportar]**. Os dados serão exportados como um CSV.

![](assets/salesforce-sync-errors-5.png)
