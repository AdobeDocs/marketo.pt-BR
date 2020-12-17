---
unique-page-id: 2360291
description: Bloquear atualizações em um campo - Documentos do Marketing - Documentação do produto
title: Bloquear atualizações de um campo
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# Bloquear atualizações em um campo {#block-updates-to-a-field}

Bloquear atualizações em um campo permite gravar no campo uma vez e, em seguida, reter o valor original durante a vida útil do campo. Isso pode ser útil para um campo como Origem da pessoa.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **Admin** e clique em **Gerenciamento de campo**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Localize o campo, selecione-o e, em **Ações de campo**, clique em **Bloquear atualizações de campo**.

   ![](assets/two-1.png)

1. Selecione as **Fontes de Entrada** que pretende bloquear e clique em **Aplicar**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Ao executar uma importação de lista, o status de um campo que está sendo bloqueado na Pré-visualização Importar só será exibido se o campo for automaticamente reconhecido pelo Marketo com base no nome do campo que corresponde a **exatas** (ou se os aliases forem estabelecidos). Se o campo for escolhido manualmente no menu suspenso Campo de marketing, o status bloqueado não será exibido na Pré-visualização Importar, mas o bloqueio de atualizações desse campo ainda será implementado.

