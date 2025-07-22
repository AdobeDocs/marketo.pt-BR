---
unique-page-id: 42762519
description: Configuração para clientes existentes - Documentação do Marketo - Documentação do produto
title: Configuração para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 4%

---

# Configuração para clientes existentes {#configuration-for-existing-customers}

Defina a seguinte configuração para começar a usar o novo Painel de insights.

>[!PREREQUISITES]
>
>Verifique se você atualizou seu pacote [!DNL Salesforce] para a versão mais recente

## Configurar o [!DNL Sales Insight] no Marketo {#configure-sales-insight-in-marketo}

1. Abra uma nova guia no navegador para obter as credenciais do [!DNL Marketo Sales Insights] da sua conta da Marketo.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Clique em **[!UICONTROL Sales Insight]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Clique em **[!UICONTROL Exibir]** para preencher as credenciais da API Rest.

   ![](assets/configuration-for-existing-customers-3.png)

1. Você verá um pop-up de confirmação. Clique em **[!UICONTROL OK]**.

## Configurar [!DNL Sales Insight] em [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **[!UICONTROL Instalação]**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Procure e selecione **[!UICONTROL Configurações de Site Remoto]**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Clique em **[!UICONTROL Novo Site Remoto]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Insira o [!UICONTROL Nome do Site Remoto] (pode ser algo como &quot;MarketoRestAPI&quot;) e o [!UICONTROL URL do Site Remoto] (o URL da API do painel Configuração da API Rest no Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/configuration-for-existing-customers-8.png)

   Agora você criou a configuração de site remoto para a API Rest.

## Acessar Marketo Sales Insight {#access-marketo-sales-insight}

1. Copie as credenciais do painel API Rest na página de Administrador [!DNL Marketo’s Sales Insight]. Cole-os na seção API Rest na página Configuração [!DNL Sales Insight] da Salesforce.

1. Insira a [!UICONTROL Chave secreta da API].

   ![](assets/configuration-for-existing-customers-9.png)
