---
description: Integração do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Integração ao Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# Integração ao Dynamic Chat {#dynamic-chat-integration}

Saiba mais sobre a integração do Dynamic Chat com o Sales Insight.

>[!PREREQUISITES]
>
>* Seu pacote Sales Insight SFDC deve ser da versão [2.4.0 ou superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Você deve configurar a [integração com o Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Verifique se, nas [Configurações Operacionais](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} do Sales Insight, o campo &quot;Chave secreta da API&quot; está preenchido. Caso contrário, saiba como recuperá-lo [aqui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Guia Configuração de [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

Siga as etapas abaixo para habilitar a integração do [!DNL Dynamic Chat].

1. Faça logon na conta do [!DNL Salesforce], clique no sinal de mais no final da barra de guias e clique em **[!DNL Marketo Sales Insight Config]**.

1. Clique para abrir o &quot;[!UICONTROL Painel do Visualforce].&quot;

   ![](assets/dynamic-chat-integration-1.png)

1. Marque a caixa de seleção **[!UICONTROL Habilitar Dados do Dynamic Chat]**.

   ![](assets/dynamic-chat-integration-2.png)

## Visão geral do recurso {#feature-overview}

As [!DNL Dynamic Chat] atividades a seguir podem ser aproveitadas por [!DNL Sales Insight] usuários...

Caixa de diálogo Envolvida: conectado no Marketo e preenchido em [!DNL Sales Insight] quando um visitante clica em um chatbot e se envolve na Caixa de diálogo.

* Nome do Dialogue
* URL da página
* Status (Iniciado / Ignorado / Concluído)

Compromisso Agendado: conectado no Marketo e preenchido em [!DNL Sales Insight] quando um visitante agenda com êxito um compromisso por meio do chatbot.

* Nome do Dialogue
* Agente
* URL da página
* Agendado para (inserir data e carimbo de data e hora)
* Status (Programado, Reprogramado, Cancelado)

Meta atingida: conectado no Marketo e preenchido em [!DNL Sales Insight] quando um visitante atinge uma meta em qualquer fluxo de diálogo.

* Nome do Dialogue
* Nome da meta
* URL da página

Interagiu com o documento: fez logon no Marketo e foi preenchido em [!DNL Sales Insight] quando um visitante interage com um documento compartilhado por meio do chatbot.

* Nome do Dialogue
* Documento
* Status

As atividades de chat estão disponíveis no Painel de insights.

![](assets/dynamic-chat-integration-3.png)

Uma guia Chat está disponível nos painéis Lead e Contato. Inclui colunas [!UICONTROL Tipo de Atividade], [!UICONTROL Nome da Caixa de Diálogo] e [!UICONTROL Data].

![](assets/dynamic-chat-integration-4.png)

Você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-5.png)

Da mesma forma, os painéis Conta e Oportunidade incluem colunas [!UICONTROL Nome], [!UICONTROL Tipo de Atividade], [!UICONTROL Nome da Caixa de Diálogo] e [!UICONTROL Data].

![](assets/dynamic-chat-integration-6.png)

A guia Chat também está incluída na guia Global Marketo. Inclui três tipos de atividades ([!UICONTROL Caixa de Diálogo Envolvida], [!UICONTROL Compromisso Agendado], [!UICONTROL Meta Atingida]), juntamente com as seguintes colunas:

* [!UICONTROL Pessoa]
* [!UICONTROL Conta]
* [!UICONTROL Tipo de atividade] ([!UICONTROL Caixa de Diálogo Engajada], [!UICONTROL Compromisso Agendado], [!UICONTROL Meta Atingida])
* [!UICONTROL Nome da caixa de diálogo]
* [!UICONTROL Data]

Novamente, você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se a caixa de seleção &quot;[!UICONTROL Habilitar dados do Dynamic Chat]&quot; estiver desabilitada, os seguintes recursos serão desabilitados:
>
>* Linha com atividades de Chat no Painel de insights (grade inteligente e exibição de lista semanal)
>* Guia Chat nos painéis Lead, Contato, Conta e Oportunidade
>* Guia Chat na guia Global Marketo
>
>Não é possível desativar apenas um desses recursos.

