---
unique-page-id: 9438139
description: Adicionar pessoa ao Incluo na lista de bloqueios - Documentação do Marketo - Documentação do produto
title: Adicionar pessoa à Inclui na lista de bloqueios
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Adicionar pessoa à Inclui na lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Inclui na lista de bloqueios as impede de receber sua correspondência.

>[!NOTE]
>
>A Marketo está mudando termos como lista negra e lista de permissões para Incluir na lista de bloqueios e Incluir na lista de permissões em nosso produto. Durante essa atualização, você pode ver os termos antigos em nossa interface do usuário e capturas de tela da documentação, e os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

1. [Criar um novo programa padrão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) e nomeie-o **Adicionar à Inclui na lista de bloqueios**.

1. Clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Dê um nome à lista e clique em **Criar**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Adicione todas as pessoas ao seu **Lista inteligente** que você deseja adicionar ao seu Incluo na lista de bloqueios.

   >[!NOTE]
   >
   >As pessoas na sua Inclui na lista de bloqueios não receberão emails operacionais.

   ![](assets/three-6.png)

1. Clique em **Novo** e selecione **Nova campanha inteligente**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Nomeie o **Nova campanha inteligente**. Clique em **Criar**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Arrastar e soltar **Membro da lista inteligente**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Selecione a lista inteligente que acabou de criar.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Arrastar e soltar **Alterar valor dos dados**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Para o **Fluxo**, insira **Bloco listado** para o **Atributo** e defina **Novo Valor** para **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. No **Agendar** selecione **Executar uma vez**.

   ![](assets/ten.png)

1. Selecionar **Executar agora** e clique em **Executar**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   É! Essas pessoas não receberão mais emails.

   >[!TIP]
   >
   >Criar um [acionar campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usar **Alterar valor dos dados** com **Bloco listado é verdadeiro** para todas as pessoas no futuro que tiverem atributos habilitados para inclui na lista de bloqueios.
