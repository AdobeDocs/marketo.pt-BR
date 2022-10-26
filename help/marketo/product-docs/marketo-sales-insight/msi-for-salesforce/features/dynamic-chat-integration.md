---
description: Integração dinâmica de chat - Documentos do Marketo - Documentação do produto
title: Integração dinâmica de chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 9d5c941dc4869b03787a6135550a133ce12b365b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 5%

---

# Integração dinâmica de chat {#dynamic-chat-integration}

Saiba mais sobre a integração do Dynamic Chat com o Sales Insight.

>[!PREREQUISITES]
>
>* Seu pacote SFDC do Sales Insight deve ter a versão [1.9 ou superior](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Você deve ter o [Integração do Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} configurado


## Guia Configuração do Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Siga as etapas abaixo para habilitar a integração do Dynamic Chat.

1. Faça logon na sua conta do Salesforce, clique em + no final da barra de guias e clique em **Configuração do Marketo Sales Insight**.

1. Clique para desfazer o &quot;Painel de força de visita&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Selecione o **Ativar dados dinâmicos do chat** caixa de seleção.

   ![](assets/dynamic-chat-integration-2.png)

## Visão geral dos recursos {#feature-overview}

As seguintes atividades de Bate-papo dinâmico podem ser aproveitadas pelos usuários do Sales Insight..

Caixa de Diálogo Envolvido: Conectado no Marketo e preenchido no Sales Insight quando um visitante clica em um chatbot e se envolve com a caixa de diálogo.

* Nome do diálogo
* URL da página
* Status (Iniciado / Solto / Concluído)

Compromisso Programado: Conectado no Marketo e preenchido no Sales Insight quando um visitante agenda com sucesso um compromisso por meio do chatbot.

* Nome do diálogo
* Agente
* URL da página
* Programado em (inserir carimbo de data e hora)
* Status (Programado, Reprogramado, Cancelado)

Meta alcançada: Conectado no Marketo e preenchido no Sales Insight quando um visitante atinge uma meta em qualquer fluxo de diálogo.

* Nome do diálogo
* Nome da meta
* URL da página

Interagiu com Documento: Conectado no Marketo e preenchido no Sales Insight quando um visitante interage com um documento compartilhado por meio do chatbot.

* Nome do diálogo
* Documento
* Status

As atividades de bate-papo estão disponíveis no Painel de insights.

![](assets/dynamic-chat-integration-3.png)

Uma guia Bate-papo está disponível nos painéis Líder e Contato. Inclui colunas Tipo de atividade, Nome da caixa de diálogo e Data.

![](assets/dynamic-chat-integration-4.png)

Você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-5.png)

Da mesma forma, os painéis Conta e Oportunidade incluem as colunas Nome, Tipo de Atividade, Nome da Caixa de Diálogo e Data.

![](assets/dynamic-chat-integration-6.png)

A guia Chat também está incluída na guia Global Marketo . Ele inclui três tipos de atividades (Caixa de diálogo Envolvida, Compromisso Programado, Meta Alcançada), juntamente com as seguintes colunas:

* Pessoa
* Conta
* Tipo de atividade (caixa de diálogo Envolvida, compromisso agendado, meta alcançada)
* Nome do diálogo
* Carimbo de data e hora

Novamente, você pode saber mais sobre um tipo de atividade clicando nele.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se a caixa de seleção &quot;Ativar dados do bate-papo dinâmico&quot; estiver desativada, os seguintes recursos serão desativados:
>
>* Linha com atividades de Chat no Painel de insights (grade inteligente e exibição de lista semanal)
>* Guia Bate-papo nos painéis Lead, Contato, Conta e Oportunidade
>* Guia Bate-papo na guia Global Marketo
>
>Não é possível desativar apenas um desses recursos.

