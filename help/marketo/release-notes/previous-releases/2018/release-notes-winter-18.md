---
unique-page-id: 13795395
description: Notas de versão - Winter '18 - Marketo Docs - Documentação do produto
title: Notas de versão - inverno de 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
TQID: https://experienceleague.adobe.com/IBxE-nJhOC4vaFcydzdsr9aAhMmiHuQro57k1SCiwTA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 598
ht-degree: 7%

---

# Notas de versão: inverno de 2018 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão Winter &#39;18. Verifique a edição do Marketo quanto à disponibilidade de recursos.

Clique nos links de título para exibir artigos detalhados para cada recurso. **Observação**: alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver vários subtítulos, os links serão colocados lá.

## Aprimoramentos no desempenho e na taxa de transferência da campanha {#campaign-performance-and-throughput-enhancements}

O Marketo está aproveitando nossa arquitetura de big data para aumentar a taxa de transferência de campanha do acionador e melhorar o processamento de atividades na Web, para que você possa reagir às ações do seu público-alvo mais rapidamente.

## Melhorias na integração do CRM [!DNL Salesforce] da Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Temos duas melhorias na Integração de CRM do [!DNL Salesforce]:

* [Notificações de administrador do Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) sobre determinadas falhas de sincronização do CRM (credenciais expiradas, limites de API atingidos, etc.)

* [Capacidade de desativar notificações por email](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) para Proprietários Principais na atribuição de clientes potenciais

Estas melhorias serão introduzidas em 2018.

## [Marketo Performance Insights](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>O [!UICONTROL Performance Insights] é um produto complementar. Entre em contato com o Gerente de sucesso do cliente da Marketo ou o Executivo de conta para obter uma cotação.

Explore como suas campanhas e canais estão afetando os resultados dos negócios com análises de atribuição, visualizações interativas e uma tabela de dados detalhada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Aprimoramentos de marketing com base em conta {#account-based-marketing-enhancements}

**[Hierarquias ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para clientes ABM com [!DNL Salesforce] ou [!DNL Microsoft Dynamics], o ABM agora herdará (e exibirá) automaticamente as relações pai-filho estabelecidas no CRM. Você poderá usar esses relacionamentos no relatório de roll-up e na execução da campanha.

## Marketing por email {#email-marketing}

**[Roteiro dinâmico de e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Os scripts do Velocity agora são aceitos em emails que usam conteúdo dinâmico. Combine conteúdo dinâmico baseado em velocidade e segmentação para criar emails altamente personalizados.

**Fuso horário do destinatário**

* **[Cadência de Criação Mensal](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: adicionamos a capacidade de agendar programas de criação em uma cadência mensal.

* **[Parar entrega](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: agora você pode parar qualquer envio restante no meio da execução.

## Integrações da rede de publicidade {#ad-network-integrations}

**[Integração à correspondência de clientes do Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Com essa integração, você pode enviar um público-alvo do Marketo para o Google para ser direcionado usando o [!DNL Google AdWords], bem como redirecionar públicos-alvo no [!DNL YouTube], Search e [!DNL Gmail].

**[[!DNL LinkedIn] Aprimoramento da API de Públicos-alvo correspondentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Nossa nova API [!DNL LinkedIn] agora permite que você redirecione pessoas em seu banco de dados do Marketo para várias contas do Campaign Manager [!DNL LinkedIn].

## Personalização na web {#web-personalization}

**Source de Dados Japonês para Web Personalization**

A Marketo está adicionando uma fonte de dados japonesa adicional para o Web Personalization a fim de melhorar a identificação de visitantes da Web (pesquisa de IP reverso) e a personalização para visitantes vindos do Japão. Os nomes da organização serão exibidos em japonês.

**[Crie um segmento da Web com listas estáticas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

O Web Personalization agora pode personalizar o conteúdo para um visitante conhecido da Web que faz parte de uma lista estática definida nas Atividades de marketing (MLM). Com esse aprimoramento, agora é possível vender para listas estáticas em canais e direcionar pessoas nessas listas com conteúdo personalizado no seu site.

## IA de conteúdo {#contentai}

**Aprimoramento do Algoritmo Preditivo**

O conteúdo recomendado por meio dos algoritmos otimizados de IA de conteúdo do Marketo gera até duas vezes mais cliques do que o conteúdo aleatório.

## Integração {#integration}

**[Ativar/desativar API do Campaign](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Essa nova API permite ativar e desativar remotamente campanhas de acionador para que você possa criar modelos de programa totalmente automatizados. Crie um modelo de programa uma vez, depois automatize a clonagem, as atualizações de material de apoio de marketing e agora a ativação/programação de campanhas inteligentes.

## [!DNL ToutApp] {#toutapp}

**Atualização para cancelamento de inscrição**

A partir de 1º de março de 2018, todos os emails enviados do [ToutApp.com](https://ToutApp.com) (e usando o botão &quot;Email com [!DNL Tout]&quot; no [!DNL Salesforce]) terão um link de cancelamento de inscrição anexado à parte inferior.

**Atualização para feeds ao vivo**

Atualizamos a aparência das guias Envolvimento e Tarefa para facilitar e agilizar a resposta dos membros de Vendas às atividades de seus clientes diretamente do Feed ativo.

**Atualização para exibição detalhada de pessoas**

O PDV (Exibição de Detalhes das Pessoas) aprimorado oferece uma exibição abrangente dos seus contatos, reunindo os detalhes de contato do [!DNL Tout] e do [!DNL Salesforce] CRM.
