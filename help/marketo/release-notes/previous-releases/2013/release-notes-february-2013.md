---
unique-page-id: 2951103
description: Notas de versão - fevereiro de 2013 - Documentação do Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Notas de versão: fevereiro de 2013 {#release-notes-february}

A versão de fevereiro inclui um recurso altamente solicitado, suporte para [!DNL Apple Safari] e outras pequenas melhorias.

## Suporte Oficial para [!DNL Apple Safari] {#official-support-for-apple-safari}

As versões mais recentes do [!DNL Apple Safari] para Mac e [!DNL Windows] são totalmente compatíveis com o uso com o Gerenciamento de Cliente Potencial da Marketo. Observação: [!DNL Safari] no iOS não é totalmente compatível.

## Aprimoramentos do Webhooks {#webhooks-enhancements}

Os Webhooks são aprimorados para evitar tokens na URL/carga útil e também podem atualizar campos de clientes potenciais do Marketo analisando respostas XML/JSON de sistemas de terceiros (não disponível no [!DNL Spark SMB Edition]).

## Ponto de extremidade de API do SOAP atualizado {#updated-soap-api-endpoint}

O ponto de extremidade de API preferencial do SOAP foi atualizado, mostrado em [!UICONTROL Admin] -> API do SOAP. Atualize suas chamadas para usar este novo ponto de extremidade. As chamadas de API para o endpoint antigo foram descontinuadas, mas continuarão funcionando. (API do SOAP não disponível no [!DNL Spark SMB Edition])

## Suporte móvel para [!DNL Facebook] guias {#mobile-support-for-facebook-tabs}

[!DNL Facebook] guias publicadas do Marketo detectarão dispositivos móveis e os rotearão para uma página de aterrissagem. Isso garantirá que o usuário obtenha o conteúdo correto em dispositivos móveis nos quais não há suporte para guias [!DNL Facebook] (disponíveis em [!DNL Spark], [!DNL Standard], [!DNL Select SMB Editions] e [!DNL Marketo Social Marketing]).

## Em breve: suporte para vários modelos {#coming-soon-support-for-multiple-models}

Estamos estabelecendo as bases para oferecer suporte a vários modelos de ciclo de receita, votou a ideia #1 para a RCA na Comunidade, em uma versão futura. Nesta versão, você observará algumas alterações, incluindo [Filtros de Smart List e Adicionar Opções em Etapas de Fluxo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md), para oferecer suporte à seleção de um modelo e estágio. Também estamos removendo os campos Estágio da Receita Principal e Modelo de Ciclo de Receita Principal da guia de grade de Cliente Potencial da Smart List.
