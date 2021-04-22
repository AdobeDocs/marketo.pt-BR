---
unique-page-id: 2360291
description: Bloquear atualizações de um campo - Documentos do Marketo - Documentação do produto
title: Bloquear atualizações de um campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Bloquear atualizações para um campo {#block-updates-to-a-field}

Bloquear atualizações em um campo permite gravar no campo uma vez e, em seguida, manter o valor original durante a vida útil do campo. Isso pode ser útil para um campo como Fonte de pessoa.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **Admin** e clique em **Gerenciamento de Campo**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Localize o campo, selecione-o e, em **Ações do campo**, clique em **Bloquear atualizações de campo**.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Também é possível bloquear atualizações para [Campos Personalizados do Membro do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Selecione as **Fontes de Entrada** que deseja bloquear e clique em **Aplicar**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Ao executar uma importação de lista, o status de um campo bloqueado na Visualização de Importação só será exibido se o campo for automaticamente reconhecido pelo Marketo com base no nome do campo correspondente a _exatamente_ (ou se aliases forem estabelecidos). Se o campo for escolhido manualmente no menu suspenso Campo do Marketo , o status de bloqueado não será exibido na Visualização de importação, mas o bloqueio de atualização desse campo ainda será implementado.
