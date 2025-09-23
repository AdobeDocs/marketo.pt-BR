---
unique-page-id: 14352464
description: Painéis de relatórios no Salesforce - Documentação do Marketo - Documentação do produto
title: Painéis de relatórios no Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 4%

---

# Painéis de relatórios no Salesforce {#reporting-dashboards-in-salesforce}

Saiba como configurar painéis abaixo.

## Relatório de aberturas e cliques {#open-and-click-report}

1. Selecione o tipo de registro **[!UICONTROL Tarefas e Eventos]**.
1. Defina os parâmetros do relatório com base no intervalo de tempo e na estrutura hierárquica desejados.
1. Adicione um filtro para remover emails internos registrados em [!DNL Salesforce] (por exemplo, Empresa/Conta diferente da Marketo).
1. Selecione o formato de relatório **[!UICONTROL Resumo]**.
1. Adicione os campos Assunto, Atribuído e Vendas do Marketo Clicadas/Vendas do Marketo visualizadas ao relatório.
1. Clique duas vezes em **[!UICONTROL Adicionar Fórmula]** no painel Campos.
1. Adicione um nome à fórmula, selecione **[!UICONTROL Percent]** no formato e selecione **[!UICONTROL Agrupamento 1]**.
1. Selecione **[!UICONTROL Vendas do Marketo clicadas/Vendas do Marketo visualizadas]** e depois **[!UICONTROL Soma]** nos Campos de resumo.
1. Adicione um sinal de divisão à fórmula e selecione **[!UICONTROL Contagem de Registros]** nos campos Resumo - _Salvar como_.

## Relatório de Desempenho do Modelo {#template-performance-report}

1. Personalize o relatório Abrir e Clicar para incluir os seguintes campos - _Salvar como_.

## Relatório de volume do modelo {#template-volume-report}

1. Modifique o Relatório de Desempenho do Modelo e inclua o filtro &quot;Modelo de Vendas do Marketo não é igual a em branco&quot;.
1. Remover o campo Cliques do Marketo Sales - _Salvar como_.

## Relatório de contas de tendência {#trending-accounts-report}

1. Selecione o tipo de registro Atividades com contas.
1. Configure os parâmetros e campos do relatório conforme indicado abaixo - _Salvar como_.
