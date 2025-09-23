---
unique-page-id: 13795395
description: Notas de versão - Winter '18 - Marketo Docs - Documentação do produto
title: Notas de versão - inverno de 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '582'
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
