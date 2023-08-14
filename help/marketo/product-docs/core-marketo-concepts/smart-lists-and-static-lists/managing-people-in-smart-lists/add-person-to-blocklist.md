---
unique-page-id: 9438139
description: Adicionar pessoa ao Incluo na lista de bloqueios - Documentação do Marketo - Documentação do produto
title: Adicionar pessoa à Inclui na lista de bloqueios
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# Adicionar pessoa à Inclui na lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Inclui na lista de bloqueios as impede de receber sua correspondência.

1. [Criar um novo programa padrão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) e nomeie-o **Adicionar à Inclui na lista de bloqueios**.

1. Clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/add-person-to-blocklist-1.png)

1. Selecionar **Lista inteligente**.

   ![](assets/add-person-to-blocklist-2.png)

1. Dê um nome à lista e clique em **Criar**.

   ![](assets/add-person-to-blocklist-3.png)

1. Adicione todas as pessoas ao seu **Lista inteligente** que você deseja adicionar ao seu Incluo na lista de bloqueios.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >As pessoas na sua Inclui na lista de bloqueios não receberão emails operacionais.

1. Volte para o seu programa.

   ![](assets/add-person-to-blocklist-5.png)

1. Clique em **Novo** e selecione **Nova campanha inteligente**.

   ![](assets/add-person-to-blocklist-6.png)

1. Nomeie o **Nova campanha inteligente**. Clique em **Criar**.

   ![](assets/add-person-to-blocklist-7.png)

1. Arrastar e soltar **Membro da lista inteligente**.

   ![](assets/add-person-to-blocklist-8.png)

1. Selecione a lista inteligente que acabou de criar.

   ![](assets/add-person-to-blocklist-9.png)

1. Clique em **Fluxo** guia. Arraste e solte a **Alterar valor dos dados** Ação de fluxo.

   ![](assets/add-person-to-blocklist-10.png)

1. No **Atributo** seleção suspensa **Bloco listado** e defina **Novo Valor** para **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Clique em **Agendar** e selecione **Executar uma vez**.

   ![](assets/add-person-to-blocklist-12.png)

1. Selecionar **Executar agora** e clique em **Executar**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clique em **Executar** novamente.

   ![](assets/add-person-to-blocklist-14.png)

Essas pessoas não receberão mais emails.

>[!TIP]
>
>Criar um [acionar campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) usar **Alterar valor dos dados** com **Bloco listado é verdadeiro** para todas as pessoas no futuro que tiverem atributos habilitados para inclui na lista de bloqueios.
