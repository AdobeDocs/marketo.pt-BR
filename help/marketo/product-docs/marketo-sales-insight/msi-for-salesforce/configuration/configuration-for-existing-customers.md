---
unique-page-id: 42762519
description: Configuração para clientes existentes - Documentos do Marketo - Documentação do produto
title: Configuração para clientes existentes
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 2%

---

# Configuração para clientes existentes {#configuration-for-existing-customers}

Configure a seguinte configuração para começar a usar o novo Painel de insights.

>[!PREREQUISITES]
>
>Certifique-se de que você atualizou seu pacote do Salesforce para a versão mais recente

## Configurar o Sales Insight no Marketo {#configure-sales-insight-in-marketo}

1. Abra uma nova guia no navegador para obter as credenciais do Marketo Sales Insights da conta do Marketo.

1. Vá para o **Administrador** área.

   ![](assets/configuration-for-existing-customers-1.png)

1. Clique em **Insight de vendas**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Clique em **Exibir** para preencher as credenciais da Rest API.

   ![](assets/configuration-for-existing-customers-3.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Configuração**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Procure e selecione **Configurações de local remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Clique em **Novo local remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoRestAPI&quot;) e o URL do site remoto (o URL da API no painel Configuração da API restante no Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Clique em **Salvar**.

   ![](assets/configuration-for-existing-customers-8.png)

   Agora você criou uma configuração de site remoto para a API Rest.

## Acessar Marketo Sales Insight {#access-marketo-sales-insight}

1. Copie as credenciais do painel da Rest API na página de administração do Insight de vendas da Marketo. Cole-os na seção Rest API da página Sales Insight Configuration do Salesforce.

1. Insira a chave secreta da API.

   ![](assets/configuration-for-existing-customers-9.png)
