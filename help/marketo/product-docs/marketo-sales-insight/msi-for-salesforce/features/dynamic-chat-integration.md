---
description: Integração de Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Integração dinâmica de chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 5%

---

# Integração dinâmica de chat {#dynamic-chat-integration}

Saiba mais sobre a integração do Dynamic Chat com o Sales Insight.

>[!PREREQUISITES]
>
>* Seu pacote SFDC do Sales Insight deve ser da versão [1.9 ou superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Você deve ter o [integração de Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} configurar

## Guia Configuração do Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Siga as etapas abaixo para habilitar a integração de Dynamic Chat.

1. Faça logon na sua conta do Salesforce, clique no + no final da barra de guias e clique em **Configuração do Marketo Sales Insight**.

1. Clique para abrir o &quot;Painel do Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Selecione o **Ativar dados de Dynamic Chat** caixa de seleção

   ![](assets/dynamic-chat-integration-2.png)

## Visão geral do recurso {#feature-overview}

As seguintes atividades de Dynamic Chat podem ser aproveitadas pelos usuários do Sales Insight...

Caixa de diálogo envolvida: conectada no Marketo e preenchida no Sales Insight quando um visitante clica em um chatbot e se envolve com a caixa de diálogo.

* Nome do diálogo
* URL da página
* Status (Iniciado / Ignorado / Concluído)

Compromisso agendado: conectado no Marketo e preenchido no Sales Insight quando um visitante agenda com êxito um compromisso por meio do chatbot.

* Nome do diálogo
* Agente
* URL da página
* Agendado para (inserir data e carimbo de data e hora)
* Status (Programado, Reprogramado, Cancelado)

Meta atingida: conectado no Marketo e preenchido no Sales Insight quando um visitante atinge uma meta em qualquer fluxo de diálogo.

* Nome do diálogo
* Nome da meta
* URL da página

Interagiu com o documento: conectado ao Marketo e preenchido no Sales Insight quando um visitante interage com um documento compartilhado por meio do chatbot.

* Nome do diálogo
* Documento
* Status

As atividades de chat estão disponíveis no Painel de insights.

![](assets/dynamic-chat-integration-3.png)

Uma guia Chat está disponível nos painéis Lead e Contato. Inclui colunas Tipo de atividade, Nome da caixa de diálogo e Data.

![](assets/dynamic-chat-integration-4.png)

Você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-5.png)

Da mesma forma, os painéis Conta e Oportunidade incluem as colunas Nome, Tipo de atividade, Nome da caixa de diálogo e Data.

![](assets/dynamic-chat-integration-6.png)

A guia Chat também está incluída na guia Global Marketo. Ele inclui três tipos de atividades (Caixa de diálogo envolvida, Compromisso agendado, Meta atingida), juntamente com as seguintes colunas:

* Pessoa
* Conta
* Tipo de atividade (caixa de diálogo envolvida, compromisso agendado, meta atingida)
* Nome do diálogo
* Carimbo de data e hora

Novamente, você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se a caixa de seleção &quot;Ativar dados de Dynamic Chat&quot; estiver desativada, os seguintes recursos serão desativados:
>
>* Linha com atividades de Chat no Painel de insights (grade inteligente e exibição de lista semanal)
>* Guia Chat nos painéis Lead, Contato, Conta e Oportunidade
>* Guia Chat na guia Global Marketo
>
>Não é possível desativar apenas um desses recursos.

