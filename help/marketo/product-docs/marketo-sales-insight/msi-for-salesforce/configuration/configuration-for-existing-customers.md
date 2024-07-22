---
unique-page-id: 42762519
description: Configuração para clientes existentes - Documentação do Marketo - Documentação do produto
title: Configuração para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Configuração para clientes existentes {#configuration-for-existing-customers}

Defina a seguinte configuração para começar a usar o novo Painel de insights.

>[!PREREQUISITES]
>
>Atualize seu pacote do Salesforce para a versão mais recente

## Configurar o Sales Insight no Marketo {#configure-sales-insight-in-marketo}

1. Abra uma nova guia em seu navegador para obter as credenciais do Marketo Sales Insights de sua conta da Marketo.

1. Vá para a área **Administrador**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Clique em **Sales Insight**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Clique em **Exibir** para preencher as credenciais da API Rest.

   ![](assets/configuration-for-existing-customers-3.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Configurar**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Procure e selecione **Configurações de Site Remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoRestAPI&quot;) e o URL do site remoto (o URL da API no painel Configuração da API Rest no Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Clique em **Salvar**.

   ![](assets/configuration-for-existing-customers-8.png)

   Agora você criou a configuração de site remoto para a API Rest.

## Acessar Marketo Sales Insight {#access-marketo-sales-insight}

1. Copie as credenciais do painel API Rest na página Admin de insights de vendas da Marketo. Cole-os na seção API Rest na página Configuração do Sales Insight do Salesforce.

1. Insira a chave secreta da API.

   ![](assets/configuration-for-existing-customers-9.png)
