---
unique-page-id: 9438139
description: Adicionar pessoa ao Incluo na lista de bloqueios - Documentação do Marketo - Documentação do produto
title: Adicionar pessoa à Inclui na lista de bloqueios
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Adicionar pessoa à Inclui na lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Inclui na lista de bloqueios as impede de receber sua correspondência.

1. Criar um novo [programa padrão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} e nomeie-o como &quot;Adicionar à Inclui na lista de bloqueios&quot;.

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Selecionar **[!UICONTROL Lista inteligente]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Dê um nome à lista e clique em **[!UICONTROL Criar]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Adicione todas as pessoas à lista inteligente que você deseja adicionar ao seu Incluo na lista de bloqueios.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >As pessoas na sua Inclui na lista de bloqueios não receberão emails operacionais.

1. Volte para o seu programa.

   ![](assets/add-person-to-blocklist-5.png)

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Nova campanha inteligente]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Dê um nome à nova Campanha inteligente. Clique em **[!UICONTROL Criar]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Arrastar e soltar **[!UICONTROL Membro da lista inteligente]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Selecione a lista inteligente que acabou de criar.

   ![](assets/add-person-to-blocklist-9.png)

1. Clique em **[!UICONTROL Fluxo]** guia. Arraste e solte a **[!UICONTROL Alterar valor dos dados]** Ação de fluxo.

   ![](assets/add-person-to-blocklist-10.png)

1. No **[!UICONTROL Atributo]** seleção suspensa **[!UICONTROL Bloco listado]** e defina **[!UICONTROL Novo Valor]** para **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Clique em **[!UICONTROL Agendar]** e selecione **[!UICONTROL Executar uma vez]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Selecionar **[!UICONTROL Executar agora]** e clique em **[!UICONTROL Executar]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clique em **[!UICONTROL Executar]** novamente.

   ![](assets/add-person-to-blocklist-14.png)

Essas pessoas não receberão mais emails.

>[!TIP]
>
>Criar um [Acionar o Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} usar **Alterar valor dos dados** com **Bloco listado é verdadeiro** para todas as pessoas no futuro que tiverem atributos habilitados para inclui na lista de bloqueios.
