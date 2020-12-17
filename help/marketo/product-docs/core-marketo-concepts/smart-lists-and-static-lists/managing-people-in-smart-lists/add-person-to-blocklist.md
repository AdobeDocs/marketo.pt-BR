---
unique-page-id: 9438139
description: Adicionar pessoa à Lista de bloqueios - Documentos do Marketing - Documentação do produto
title: Adicionar pessoa à Lista de bloqueios
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Adicionar pessoa à Lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Lista de bloqueios impede que elas recebam sua correspondência.

>[!NOTE]
>
>O Marketo está mudando termos como Blacklist e Whitelist para Lista de bloqueios e Lista de permissões em nosso produto. Durante esta atualização, você pode ver os termos antigos em nossa interface do usuário e nas capturas de tela da documentação, bem como os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

1. [Crie um novo ](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) programa padrão e nomeie-o como  **Adicionar à Lista de bloqueios**.
1. Clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Dê um nome à sua lista e clique em **Criar**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Adicione todas as pessoas à sua **Lista inteligente** que deseja adicionar à sua Lista de bloqueios.

   >[!NOTE]
   >
   >As pessoas na sua Lista de bloqueios não receberão e-mails operacionais.

   ![](assets/three-6.png)

1. Clique em **Novo** e selecione **Nova Campanha inteligente**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Nomeie a **Nova Campanha inteligente**. Clique em **Criar**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arraste e solte **Membro da Lista inteligente**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Selecione a lista inteligente que você acabou de criar.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arraste e solte **Alterar valor de dados**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para o **Fluxo**, digite **Bloquear Listado** para o **Atributo** e defina **Novo Valor** como **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Na guia **Schedule**, selecione **Run Once**.

   ![](assets/ten.png)

1. Selecione **Executar agora** e clique em **Executar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   É! Essas pessoas não receberão mais emails.

   >[!TIP]
   >
   >Crie uma [campanha inteligente de acionamento](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usando **Alterar valor de dados** com **Bloqueio listado é verdadeiro** para todas as pessoas que no futuro têm atributos que podem ser  lista de bloqueios.

