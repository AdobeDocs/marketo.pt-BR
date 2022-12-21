---
unique-page-id: 9438139
description: Adicionar pessoa ao Lista de bloqueios - Documentos da Marketo - Documentação do produto
title: Adicionar Pessoa à  Lista de bloqueios
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Adicionar Pessoa à  Lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Lista de bloqueios impede que elas recebam sua correspondência.

>[!NOTE]
>
>A Marketo está mudando termos como Blacklist e Whitelist para Lista de bloqueios e Lista de permissões em nosso produto. Durante essa atualização, você pode ver os termos antigos em nossa interface do usuário e capturas de tela da documentação, bem como os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

1. [Criar um novo programa padrão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) e nomeá-lo **Adicionar à  Lista de bloqueios**.

1. Clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Dê um nome à lista e clique em **Criar**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Adicionar todas as pessoas à sua **Lista inteligente** você deseja adicioná-lo à sua Lista de bloqueios.

   >[!NOTE]
   >
   >As pessoas na sua Lista de bloqueios não receberão emails operacionais.

   ![](assets/three-6.png)

1. Clique em **Novo** e selecione **Nova Campanha Inteligente**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Nomeie a função **Nova Campanha Inteligente**. Clique em **Criar**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arrastar e soltar **Membro da Smart List**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Selecione a lista inteligente que acabou de criar.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arrastar e soltar **Alterar valor de dados**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para o **Fluxo**, insira **Bloqueio listado** para **Atributo** e definir **Novo valor** para **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. No **Agendar** guia , selecione **Executar uma vez**.

   ![](assets/ten.png)

1. Selecionar **Executar agora** e clique em **Executar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Essas pessoas não receberão mais emails.

   >[!TIP]
   >
   >Crie um [acionar campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usar **Alterar valor de dados** com **Bloqueio Listado é verdadeiro** para todas as pessoas no futuro que tenham atributos com capacidade de  lista de bloqueios.
