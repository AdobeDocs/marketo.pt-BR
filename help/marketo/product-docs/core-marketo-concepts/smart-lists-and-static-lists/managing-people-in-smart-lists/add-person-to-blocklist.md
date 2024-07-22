---
unique-page-id: 9438139
description: Adicionar pessoa ao Incluo na lista de bloqueios - Documentação do Marketo - Documentação do produto
title: Adicionar pessoa à Inclui na lista de bloqueios
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Adicionar pessoa à Inclui na lista de bloqueios {#add-person-to-blocklist}

Adicionar pessoas à sua Inclui na lista de bloqueios as impede de receber sua correspondência.

1. Crie um novo [programa padrão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} e nomeie-o como &quot;Adicionar ao arquivo de Inclui na lista de bloqueios&quot;.

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Selecione **[!UICONTROL Smart List]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Nomeie sua lista e clique em **[!UICONTROL Criar]**.

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

1. Arraste e solte **[!UICONTROL Membro da Smart List]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Selecione a lista inteligente que acabou de criar.

   ![](assets/add-person-to-blocklist-9.png)

1. Clique na guia **[!UICONTROL Fluxo]**. Arraste e solte a Ação de Fluxo **[!UICONTROL Alterar Valor de Dados]**.

   ![](assets/add-person-to-blocklist-10.png)

1. No menu suspenso **[!UICONTROL Atributo]**, selecione **[!UICONTROL Bloqueio Listado]** e defina **[!UICONTROL Novo Valor]** como **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Clique na guia **[!UICONTROL Agendar]** e selecione **[!UICONTROL Executar Uma Vez]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Selecione **[!UICONTROL Executar agora]** e clique em **[!UICONTROL Executar]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clique em **[!UICONTROL Executar]** novamente.

   ![](assets/add-person-to-blocklist-14.png)

Essas pessoas não receberão mais emails.

>[!TIP]
>
>Crie uma [Campanha de Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} usando **Alterar Valor de Dados** com **A Lista de Bloqueios é verdadeira** para todas as pessoas no futuro que tiverem atributos habilitados para inclui na lista de bloqueios.
