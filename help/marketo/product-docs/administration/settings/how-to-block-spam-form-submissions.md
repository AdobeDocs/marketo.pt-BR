---
description: Como bloquear envios de formulários de spam - Documentos do Marketo - Documentação do produto
title: Como bloquear envios de formulários de spam
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Como bloquear envios de formulários de spam {#how-to-block-spam-form-submissions}

Geralmente, os envios de formulários com uma soma de verificação inválida ou ausente (geralmente de bots) podem produzir estatísticas falsas. Aqui está como evitar isso.

>[!CAUTION]
>
>Esse recurso rejeita envios de formulários feitos usando POSTs programáticos para o endpoint leadCapture/save2. Se a sua empresa utilizar uma integração que envie formulários para a Marketo com esse método, habilitar esse recurso bloqueará esses envios. Não é possível usar o leadCapture/save2 como uma API ou executar envios de formulários programáticos diretamente para ele, assim como proibir. Certifique-se de que sua empresa só envie formulários usando: Ativos de formulário, código de formulários incorporados, API Forms2.js ou a API REST de envio de formulário.

1. Clique em **Admin**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Clique em **Treasure Chest**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. Ao lado de **Captura de Pessoa - Rejeitar Valores de Soma de Verificação Inválidos**, clique em **Editar**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Marque a caixa de seleção **Enabled** e clique em **Save**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>Ao ativar esse recurso, é possível observar uma queda na atividade do formulário à medida que números falsos são filtrados.
