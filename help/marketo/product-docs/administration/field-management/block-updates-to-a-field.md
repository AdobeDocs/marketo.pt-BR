---
unique-page-id: 2360291
description: Bloquear atualizações em um campo - Documentação do Marketo - Documentação do produto
title: Bloquear atualizações em um campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Bloquear atualizações em um campo {#block-updates-to-a-field}

O bloqueio de atualizações em um campo permite gravar no campo uma vez e, em seguida, reter o valor original por toda a vida útil do campo. Isso pode ser útil para um campo como [!UICONTROL Source de pessoa].

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Clique em **[!UICONTROL Gerenciamento de campos]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Localize o campo, selecione-o e, em **[!UICONTROL Ações do Campo]**, clique em **[!UICONTROL Bloquear Atualizações do Campo]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Você também pode bloquear atualizações para [Campos Personalizados de Membros do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Selecione as **[!UICONTROL Fontes de Entrada]** que deseja bloquear e clique em **[!UICONTROL Aplicar]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Ao executar uma importação de lista, o status de um campo que está sendo bloqueado na Visualização da importação só será exibido se o campo for reconhecido automaticamente pelo Marketo com base no nome do campo correspondente a _exatamente_ (ou se forem estabelecidos aliases). Se o campo for escolhido manualmente no menu suspenso Campo do Marketo, o status bloqueado não será exibido na Pré-visualização de importação, mas o bloqueio de atualizações a esse campo ainda será implementado.
