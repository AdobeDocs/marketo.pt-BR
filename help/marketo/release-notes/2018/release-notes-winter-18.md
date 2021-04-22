---
unique-page-id: 13795395
description: Notas de versão - inverno de 18 - Documentos da Marketo - Documentação do produto
title: Notas de versão - inverno de 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 8%

---

# Notas de versão: Inverno &#39;18 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 18. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

Clique nos links de título para exibir os artigos detalhados de cada recurso. **Observação**: Alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver várias subposições, as vinculações serão colocadas lá.

## Aprimoramentos de desempenho e throughput da campanha {#campaign-performance-and-throughput-enhancements}

A Marketo está aproveitando nossa grande arquitetura de dados para aumentar a taxa de transferência da campanha do acionador e melhorar o processamento da atividade da Web, para que você possa reagir mais rapidamente às ações do seu público-alvo.

## Aprimoramentos na integração do Salesforce CRM do Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Temos duas melhorias na nossa Integração do Salesforce CRM:

* [Notificações ](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) de administrador do Marketo para determinadas falhas de sincronização do CRM (credenciais expiradas, limites de API alcançados, etc.)

* [Capacidade de desativar ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) notificações por email para Proprietários Potenciais na atribuição de lead

Estas melhorias serão lançadas em 2018.

## [Marketo Performance Insights](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>O Performance Insights é um produto complementar. Entre em contato com o Gerente de sucesso do cliente da Marketo ou o Executivo de conta para obter uma cotação.

Explore como suas campanhas e canais estão afetando os resultados comerciais com análises de atribuição, visualizações interativas e uma tabela de dados detalhada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Aprimoramentos de marketing baseado em conta {#account-based-marketing-enhancements}

**[Hierarquias de ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para clientes ABM com Salesforce ou Microsoft Dynamics, o ABM herdará automaticamente (e exibirá) os relacionamentos pai-filho estabelecidos no CRM. Você poderá usar esses relacionamentos tanto no relatório de roll-up quanto na execução da campanha.

## Marketing por e-mail {#email-marketing}

**[Roteiro dinâmico de e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Agora há suporte à criação rápida de roteiros em e-mails usando conteúdo dinâmico. Combine velocidade e conteúdo dinâmico baseado em segmentação para criar emails altamente personalizados.

**Fuso horário do destinatário**

* **[Cadência](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)** mensal de cultura: Adicionamos a capacidade de programar programas de educação em uma cadência mensal.

* **[Parar entrega](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Agora você pode interromper todos os envios restantes no meio da execução.

## Integrações de rede de anúncios {#ad-network-integrations}

**[Integração à correspondência de clientes do Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Com essa integração, você pode enviar um público-alvo da Marketo para o Google para ser direcionado usando o Google AdWords, bem como direcionar novamente os públicos-alvo através do YouTube, Search e Gmail.

**[Aprimoramento da API de públicos-alvo correspondentes do linkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Nossa nova API do LinkedIn agora permite que você direcione novamente pessoas no seu banco de dados do Marketo em várias contas do LinkedIn Campaign Manager.

## Personalização na Web {#web-personalization}

**Fonte de dados japonesa para personalização da Web**

A Marketo está adicionando uma fonte de dados japonesa adicional para a Personalização da Web para melhorar a identificação do visitante da Web (pesquisa de IP reverso) e a personalização para visitantes que chegam do Japão. Os nomes da organização serão exibidos em japonês.

**[Crie um segmento da Web com listas estáticas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

A Personalização da Web agora pode personalizar o conteúdo para um visitante conhecido da Web que faz parte de uma lista estática definida em Atividades de marketing (MLM). Com esse aprimoramento, agora é possível comercializar listas estáticas em todos os canais e direcionar pessoas nessas listas com conteúdo personalizado em seu site.

## ContentAI {#contentai}

**Aprimoramento do algoritmo de previsões**

O conteúdo recomendado por meio dos algoritmos otimizados ContentAI da Marketo geram até duas vezes mais cliques que o conteúdo aleatório.

## Integração {#integration}

**[Ativar/Desativar API de campanhas](https://developers.marketo.com/rest-api/assets/campaigns/)**

Essa nova API permite que você ative e desative remotamente campanhas do acionador, para que possa criar modelos de programa totalmente automatizados. Crie um template de programa uma vez, depois automatize a clonagem, as atualizações de materiais de marketing e agora a ativação/agendamento de campanhas inteligentes.

## ToutApp {#toutapp}

**Atualização para cancelamento de inscrição**

A partir de 1 de março de 2018, todos os emails enviados de [ToutApp.com](https://ToutApp.com) (e usando o botão &quot;Email with Tout&quot; no Salesforce) terão um link de cancelamento de inscrição anexado à parte inferior.

**Atualização para feeds ao vivo**

Atualizamos a aparência das guias Envolvimento e Tarefa para facilitar e agilizar a resposta dos membros de Vendas às atividades dos clientes diretamente do Feed ativo.

**Atualização para exibição detalhada de pessoas**

A PDV (Exibição de detalhes de pessoas) aprimorada oferece uma visão abrangente de seus contatos, reunindo seus detalhes de contato do Tout e do Salesforce CRM.
