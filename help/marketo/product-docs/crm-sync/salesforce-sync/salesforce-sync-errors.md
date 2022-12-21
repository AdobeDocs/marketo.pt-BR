---
description: Erros de sincronização do Salesforce - Documentos do Marketo - Documentação do produto
title: Erros de Sincronização do Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 3%

---

# Erros de Sincronização do Salesforce {#salesforce-sync-errors}

Visualize um resumo dos erros enfrentados durante o processo de sincronização. Isso inclui erros causados por falhas de sincronização de dados incompatíveis.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Exibir erros de sincronização {#view-sync-errors}

1. Clique em **Administrador**.

   ![](assets/salesforce-sync-errors-1.png)

1. Em Integração, clique em **Salesforce**, em seguida, o **Erros de sincronização** guia .

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Os erros listados variam do tempo atual até cinco dias antes da sincronização atual.

| Campo | Descrição |
|---|---|
| Falha em | Nível de registro _ou_ Nível da tarefa |
| Data/hora da falha | Detalhes do erro |
| Tipo de erro | Mensagem de retorno SFDC |

>[!TIP]
>
>Clicar no registro de nível de registro mostra as IDs da Marketo e do Salesforce do objeto relacionado. Em alguns casos, a mensagem no registro e os erros de nível de trabalho são diretamente do Salesforce. Pesquisá-los online pode fornecer detalhes adicionais.

## Erros de Sincronização de Filtro {#filter-sync-errors}

1. Para filtrar os dados, clique no ícone de filtro na extremidade direita da página.

   ![](assets/salesforce-sync-errors-3.png)

1. Selecione sua data e intervalo de tempo e filtre por Tipo de Erro (Nível da Tarefa ou Nível de Registro). Clique em **Aplicar** quando concluído.

   ![](assets/salesforce-sync-errors-4.png)

**Etapa opcional**: Para exportar erros de sincronização, clique em **Exportar**. Os dados serão exportados como um CSV.

![](assets/salesforce-sync-errors-5.png)
