---
unique-page-id: 13795395
description: Notas de versão - inverno de 18 - Documentos da Marketo - Documentação do produto
title: Notas de versão - inverno de 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 9%

---

# Notas de versão: Inverno de 18 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 18. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

Clique nos links de título para exibir os artigos detalhados de cada recurso. **Observação**: Alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver várias subposições, as vinculações serão colocadas lá.

## Aprimoramentos de desempenho e throughput da campanha {#campaign-performance-and-throughput-enhancements}

A Marketo está aproveitando nossa grande arquitetura de dados para aumentar a taxa de transferência da campanha do acionador e melhorar o processamento da atividade da Web, para que você possa reagir mais rapidamente às ações do seu público-alvo.

## Melhorias na integração do Marketo ao CRM do Salesforce {#enhancements-to-marketo-s-salesforce-crm-integration}

Temos duas melhorias na nossa Integração do Salesforce CRM:

* [Notificações do administrador do Marketo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) para determinadas falhas de sincronização do CRM (credenciais expiradas, limites de API atingidos, etc.)

* [Capacidade de desativar notificações por email](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) para Proprietários Potenciais na atribuição de lead

Estas melhorias serão lançadas em 2018.

## [Marketo Performance Insights](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>O Performance Insights é um produto complementar. Entre em contato com seu Gerente de conta ou Executivo de conta da Marketo para obter uma cotação.

Explore como suas campanhas e canais estão afetando os resultados comerciais com análises de atribuição, visualizações interativas e uma tabela de dados detalhada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Aprimoramentos de marketing baseado em conta {#account-based-marketing-enhancements}

**[Hierarquias de ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para clientes ABM com Salesforce ou Microsoft Dynamics, o ABM herdará automaticamente (e exibirá) os relacionamentos pai-filho estabelecidos no CRM. Você poderá usar esses relacionamentos tanto no relatório de roll-up quanto na execução da campanha.

## Marketing por e-mail {#email-marketing}

**[Roteiro dinâmico de e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Agora há suporte à criação rápida de roteiros em e-mails usando conteúdo dinâmico. Combine velocidade e conteúdo dinâmico baseado em segmentação para criar emails altamente personalizados.

**Fuso horário do destinatário**

* **[Cadência mensal de cultura](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Adicionamos a capacidade de programar programas de educação em uma cadência mensal.

* **[Parar entrega](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Agora você pode interromper todos os envios restantes no meio da execução.

## Integrações de rede de anúncios {#ad-network-integrations}

**[Integração à correspondência de clientes do Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Com essa integração, você pode enviar um público-alvo do Marketo para o Google para ser direcionado usando o Google AdWords, bem como direcionar novamente os públicos-alvo através do YouTube, Search e Gmail.

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

**[Ativar/Desativar API de campanhas](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

Essa nova API permite que você ative e desative remotamente campanhas do acionador, para que possa criar modelos de programa totalmente automatizados. Crie um template de programa uma vez, depois automatize a clonagem, as atualizações de materiais de marketing e agora a ativação/agendamento de campanhas inteligentes.

## ToutApp {#toutapp}

**Atualização para cancelamento de inscrição**

A partir de 1 de março de 2018, todos os emails enviados de [ToutApp.com](https://ToutApp.com) (e usando o botão &quot;Email com saída&quot; no Salesforce) terá um link de cancelamento de assinatura anexado à parte inferior.

**Atualização para feeds ao vivo**

Atualizamos a aparência das guias Envolvimento e Tarefa para facilitar e agilizar a resposta dos membros de Vendas às atividades dos clientes diretamente do Feed ativo.

**Atualização para exibição detalhada de pessoas**

A PDV (Exibição de detalhes de pessoas) aprimorada oferece uma visão abrangente de seus contatos, reunindo seus detalhes de contato do Tout e do Salesforce CRM.
