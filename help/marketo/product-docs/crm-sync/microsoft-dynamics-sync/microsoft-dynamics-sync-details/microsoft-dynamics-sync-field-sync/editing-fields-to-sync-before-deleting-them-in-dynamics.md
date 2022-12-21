---
description: Editar campos para sincronização antes de excluí-los no Dynamics - Marketo Docs - Documentação do produto
title: Editar campos para sincronização antes de excluí-los no Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Editar campos para sincronização antes de excluí-los no Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Às vezes, talvez você queira excluir campos no Dynamics. O Marketo mantém a lista de campos como uma referência para basear a sincronização. Se um campo for excluído no Dynamics enquanto a sincronização estiver ativada, a sincronização poderá encontrar erros. Antes de excluir qualquer campo, siga as etapas abaixo.

1. No Marketo, clique em **Administrador**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Em Integração, clique em **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Clique em **Desativar Sincronização**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Em uma nova guia no navegador, faça logon no Dynamics e exclua os campos desejados.

1. De volta ao Marketo, em Microsoft Dynamics, clique em **Editar** ao lado de &quot;Etapa 2: Selecione Campos a serem sincronizados.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Revise os campos e clique em **Salvar**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Clicar **Salvar** O é necessário para salvar o schema atualizado para a sincronização, mesmo se nenhuma alteração for feita.

>[!NOTE]
>
>Se a Sincronização não for interrompida antes de excluir um campo no Dynamics, ela poderá encontrar erros. Se isso acontecer, a sincronização será interrompida. Antes de retomar, o Administrador do Marketo precisaria revisar &quot;Selecionar campos para sincronização&quot; (discutido acima) e clicar em **Salvar** para que a sincronização aceite as alterações do esquema.

Lembre-se de ativar a sincronização depois que as alterações forem salvas!
