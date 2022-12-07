---
unique-page-id: 2360291
description: Bloquear atualizações de um campo - Documentos do Marketo - Documentação do produto
title: Bloquear atualizações de um campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Bloquear atualizações de um campo {#block-updates-to-a-field}

Bloquear atualizações em um campo permite gravar no campo uma vez e, em seguida, manter o valor original durante a vida útil do campo. Isso pode ser útil para um campo como Fonte de pessoa.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para o **Administrador** área.

   ![](assets/block-updates-to-a-field-1.png)

1. Clique em **Gerenciamento de campos**.

   ![](assets/block-updates-to-a-field-2.png)

1. Encontre o campo , selecione-o e, em seguida, em **Ações do campo**, clique em **Bloquear Atualizações de Campo**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Você pode bloquear atualizações para [Campos personalizados do membro do programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) também.

1. Selecione o **Fontes de entrada** você deseja bloquear e clicar em **Aplicar**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Ao executar uma importação de lista, o status de um campo bloqueado na Visualização de importação será exibido somente se o campo for automaticamente reconhecido pelo Marketo com base no nome do campo correspondente _exatamente_ (ou se forem estabelecidos aliases). Se o campo for escolhido manualmente no menu suspenso Campo do Marketo , o status bloqueado não será exibido na Visualização de importação, mas o bloqueio de atualização desse campo ainda será implementado.
