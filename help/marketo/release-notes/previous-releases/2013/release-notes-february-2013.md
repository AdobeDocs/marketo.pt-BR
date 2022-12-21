---
unique-page-id: 2951103
description: Notas de versão - fevereiro de 2013 - Documentação da Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2013
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Notas de versão: Fevereiro de 2013 {#release-notes-february}

A versão de fevereiro inclui um recurso altamente solicitado, suporte para o Apple Safari e outras pequenas melhorias.

## Suporte oficial para o Apple Safari {#official-support-for-apple-safari}

As versões mais recentes do Apple Safari para Mac e Windows são totalmente compatíveis para uso com o Gerenciamento de clientes potenciais da Marketo. Observação: O Safari no iOS não é totalmente compatível.

## Aprimoramentos de Webhooks {#webhooks-enhancements}

Os Webhooks são aprimorados para tokens de escape no URL/payload e também podem atualizar campos de lead do Marketo analisando respostas XML/JSON de sistemas de terceiros (não disponível no Spark SMB Edition).

## Endpoint da API SOAP atualizado {#updated-soap-api-endpoint}

O endpoint preferencial da API SOAP foi atualizado, que é mostrado em Admin -> SOAP API. Atualize suas chamadas para usar este novo terminal. As chamadas de API para o endpoint antigo estão obsoletas, mas continuarão a funcionar. (API SOAP não disponível no Spark SMB Edition)

## Suporte móvel para guias Facebook {#mobile-support-for-facebook-tabs}

As guias do facebook publicadas do Marketo detectarão dispositivos móveis e os encaminharão para uma página de aterrissagem. Isso garantirá que o usuário obtenha o conteúdo correto em dispositivos móveis nos quais as guias do Facebook não são compatíveis (disponíveis em Spark, Standard, Select SMB Editions e Marketo Social Marketing).

## Em breve: Suporte para vários modelos {#coming-soon-support-for-multiple-models}

Estamos preparando o terreno para suportar vários modelos de ciclo de receita, votamos a ideia nº 1 para RCA na Comunidade, em uma versão futura. Nesta versão, você observará algumas alterações, incluindo [Filtros de Smart List e Adicionar Opções em Etapas de Fluxo](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) apoiar a seleção de um modelo e de um estágio. Também estamos movendo os campos Estágio da receita do cliente potencial e Modelo do ciclo da receita do cliente potencial para fora da guia Grade de lead da lista inteligente.
