---
unique-page-id: 2951103
description: Notas de versão - fevereiro de 2013 - Documentação do Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Notas de versão: fevereiro de 2013 {#release-notes-february}

A versão de fevereiro inclui um recurso altamente solicitado, suporte para o Apple Safari e outras pequenas melhorias.

## Suporte oficial para o Apple Safari {#official-support-for-apple-safari}

As versões mais recentes do Apple Safari para Mac e Windows são totalmente compatíveis com o uso do Marketo Lead Management. Observação: o Safari no iOS não é totalmente compatível.

## Aprimoramentos do Webhooks {#webhooks-enhancements}

Os Webhooks são aprimorados para evitar tokens no URL/carga útil e também podem atualizar os campos de clientes potenciais do Marketo analisando respostas XML/JSON de sistemas de terceiros (não disponível na Spark SMB Edition).

## Ponto de extremidade de API SOAP atualizado {#updated-soap-api-endpoint}

O endpoint da API de SOAP preferencial foi atualizado, o que é mostrado em Administração -> API de SOAP. Atualize suas chamadas para usar este novo ponto de extremidade. As chamadas de API para o endpoint antigo foram descontinuadas, mas continuarão funcionando. (API SOAP não disponível no Spark SMB Edition)

## Suporte móvel para guias do Facebook {#mobile-support-for-facebook-tabs}

As guias do facebook publicadas no Marketo detectarão dispositivos móveis e os rotearão para uma página de aterrissagem. Isso garantirá que o usuário obtenha o conteúdo correto em dispositivos móveis nos quais as guias do Facebook não são compatíveis (disponíveis no Spark, Standard, Select SMB Editions e Marketo Social Marketing).

## Em breve: suporte para vários modelos {#coming-soon-support-for-multiple-models}

Estamos estabelecendo as bases para oferecer suporte a vários modelos de ciclo de receita, votou a ideia #1 para a RCA na Comunidade, em uma versão futura. Nesta versão, você observará algumas alterações, incluindo [Filtros de Smart List e Adicionar Opções em Etapas de Fluxo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md), para oferecer suporte à seleção de um modelo e estágio. Também estamos removendo os campos Estágio da Receita Principal e Modelo de Ciclo de Receita Principal da guia de grade de Cliente Potencial da Smart List.
