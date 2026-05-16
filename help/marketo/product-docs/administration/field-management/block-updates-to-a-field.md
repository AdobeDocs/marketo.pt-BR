---
unique-page-id: 2360291
description: Bloqueie atualizações em um campo para que o primeiro valor gravado seja retido pelo tempo de vida do registro.
title: Bloquear atualizações em um campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
TQID: https://experienceleague.adobe.com/XHwNOU3s7CWDUp21LaxOTo--NA1nYZvCL7G4y5AjUFg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 7%

---

# Bloquear atualizações em um campo {#block-updates-to-a-field}

O bloqueio de atualizações em um campo permite gravar no campo uma vez e, em seguida, reter o valor original por toda a vida útil do registro. Isso pode ser útil para um campo como [!UICONTROL Source de pessoa].

>[!NOTE]
>
>**Permissões de administrador são necessárias**

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
