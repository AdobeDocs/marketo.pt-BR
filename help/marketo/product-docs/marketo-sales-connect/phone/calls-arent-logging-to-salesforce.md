---
unique-page-id: 14352435
description: Chamadas não estão fazendo logon no Salesforce - Documentos do Marketo - Documentação do produto
title: Chamadas não estão fazendo logon no Salesforce
exl-id: 99528c1a-7398-442b-81d1-9b5908e35e2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Chamadas não estão fazendo logon no Salesforce {#calls-arent-logging-to-salesforce}

Se você quiser que suas chamadas do Telefone de Vendas sejam registradas automaticamente no Salesforce, verifique se o seguinte está em vigor.

Você precisará que sua conta do Sales Connect esteja conectada a seu [Conta do Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md) por meio da conexão da API.

Se você chamar do [aplicação web](https://toutapp.com/login), você precisará de uma ID do Salesforce salva nesse contato. [Clique aqui](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/import-a-salesforce-id-into-sales-connect.md) para ver como você pode garantir que todos os contatos do Sales Connect tenham uma ID do Salesforce associada a eles.

>[!NOTE]
>
>Certifique-se de ter &quot;Chamada&quot; na lista de seleção de tipo de tarefa para obter relatórios precisos e fáceis no Salesforce.

Depois que isso estiver em vigor, você verá uma Tarefa criada na seção Histórico de atividades do Salesforce.
