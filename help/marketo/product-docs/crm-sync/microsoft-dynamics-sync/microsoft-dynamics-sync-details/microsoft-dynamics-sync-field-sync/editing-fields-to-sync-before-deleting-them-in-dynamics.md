---
description: Editar campos para sincronização antes de excluí-los no Dynamics - Documentação do Marketo - Documentação do produto
title: Editar campos para sincronização antes de excluí-los no Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Editando Campos para Sincronização Antes de Excluí-los em [!DNL Dynamics] {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Às vezes, você pode querer excluir campos em [!DNL Dynamics]. O Marketo mantém a lista de campos como uma referência para basear a sincronização. Se um campo for excluído em [!DNL Dynamics] enquanto a sincronização estiver ativada, a sincronização poderá encontrar erros. Antes de excluir qualquer campo, siga as etapas abaixo.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Em [!UICONTROL Integração], clique em **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Clique em **[!UICONTROL Desabilitar sincronização]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Em uma nova guia do navegador, faça logon no [!DNL Dynamics] e exclua os campos desejados.

1. De volta ao Marketo, em [!DNL Microsoft Dynamics], clique em **[!UICONTROL Editar]** ao lado de &quot;[!UICONTROL Etapa 2: Selecionar campos para sincronização].&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Revise os campos e clique em **[!UICONTROL Salvar]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>É necessário clicar em **[!UICONTROL Salvar]** para salvar o esquema atualizado para a sincronização, mesmo que nenhuma alteração tenha sido feita.

>[!NOTE]
>
>Se a Sincronização não for interrompida antes da exclusão de um campo em [!DNL Dynamics], a sincronização poderá encontrar erros. Se isso acontecer, a sincronização será interrompida. Antes de continuar, o Administrador do Marketo precisaria revisar &quot;[!UICONTROL Selecionar campos para sincronização]&quot; (discutido acima) e clicar em **[!UICONTROL Salvar]** para que a sincronização aceite as alterações do esquema.

Lembre-se de ativar a sincronização depois que as alterações forem salvas!
