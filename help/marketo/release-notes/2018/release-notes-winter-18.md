---
unique-page-id: 13795395
description: Notas de versão - inverno de 18 - Documentos do Marketo - Documentação do produto
title: Notas de versão - inverno de 18
translation-type: tm+mt
source-git-commit: d68eba976d0b71339fc5b70b3c035641d9e81d44
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---


# Notas de versão: Inverno &#39;18 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 18. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

Clique nos links de título para exibir os artigos detalhados de cada recurso. **Observação**: Alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver várias subposições, as vinculações serão colocadas lá.

## Aprimoramentos de desempenho e throughput da campanha {#campaign-performance-and-throughput-enhancements}

O Marketo está aproveitando nossa grande arquitetura de dados para aumentar a taxa de transferência da campanha do acionador e melhorar o processamento da atividade da Web, para que você possa reagir mais rápido às ações de seu público-alvo.

## Aprimoramentos na integração do Salesforce CRM do Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Temos duas melhorias na nossa Integração do Salesforce CRM:

* [Notificações do Administrador do Marketo ](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) para determinadas falhas de sincronização do CRM (credenciais expiradas, limites de API alcançados, etc.)

* [Capacidade de desativar ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) notificações por email para Proprietários Potenciais na atribuição de lead

Estas melhorias serão lançadas em 2018.

## [Insights de desempenho do Marketo](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>O Performance Insights é um produto complementar. Entre em contato com o Gerente de sucesso do cliente do Marketo ou o Executivo de conta para obter uma cotação.

Explore como suas campanhas e canais estão afetando os resultados comerciais com análises de atribuição, visualizações interativas e uma tabela de dados detalhada.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Aprimoramentos de marketing baseado em conta {#account-based-marketing-enhancements}

**[Hierarquias de ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Para clientes ABM com Salesforce ou Microsoft Dynamics, o ABM herdará automaticamente (e exibirá) os relacionamentos pai-filho estabelecidos no CRM. Você poderá usar esses relacionamentos tanto no relatório de roll-up quanto na execução da campanha.

## Marketing de email {#email-marketing}

**[Script de email dinâmico](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Agora, os scripts do Velocity são suportados em emails que usam conteúdo dinâmico. Combine velocidade e conteúdo dinâmico baseado em segmentação para criar emails altamente personalizados.

**Fuso Horário do Recipient**

* **[Cadência](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)** mensal de cultura: Adicionamos a capacidade de programar programas de educação em uma cadência mensal.

* **[Parar entrega](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Agora você pode interromper todos os envios restantes no meio da execução.

## Integrações de rede de anúncios {#ad-network-integrations}

**[Integração de correspondência do cliente do Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Com essa integração, você pode enviar um público-alvo do Marketo para o Google para ser direcionado usando o Google AdWords, bem como redirecionar públicos-alvo no YouTube, Pesquisar e Gmail.

**[Aprimoramento da API de públicos-alvo correspondentes do LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Nossa nova API do LinkedIn agora permite redirecionar pessoas no banco de dados do Marketo em várias contas do LinkedIn Campaign Manager.

## Personalização da Web {#web-personalization}

**Fonte de dados japonesa para personalização da Web**

O Marketo está adicionando uma fonte de dados japonesa adicional para a Personalização da Web para melhorar a identificação do visitante da Web (pesquisa de IP reverso) e a personalização para visitantes que chegam do Japão. Os nomes da organização serão exibidos em japonês.

**[Criar um segmento da Web usando listas estáticas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

A Personalização da Web agora pode personalizar o conteúdo para um visitante conhecido da Web que faz parte de uma lista estática definida em Atividades de marketing (MLM). Com esse aprimoramento, agora é possível comercializar listas estáticas em todos os canais e direcionar pessoas nessas listas com conteúdo personalizado em seu site.

## ContentAI {#contentai}

**Aprimoramento do algoritmo preditivo**

Conteúdo recomendado por meio dos algoritmos ContentAI otimizados do Marketo geram até o dobro de cliques como conteúdo aleatório.

## Integração {#integration}

**[Ativar/desativar a API do Campaign](https://developers.marketo.com/rest-api/assets/campaigns/)**

Essa nova API permite que você ative e desative remotamente campanhas do acionador, para que possa criar modelos de programa totalmente automatizados. Crie um template de programa uma vez, depois automatize a clonagem, as atualizações de materiais de marketing e agora a ativação/agendamento de campanhas inteligentes.

## ToutApp {#toutapp}

**Cancelar assinatura da atualização**

A partir de 1 de março de 2018, todos os emails enviados de [ToutApp.com](https://ToutApp.com) (e usando o botão &quot;Email with Tout&quot; no Salesforce) terão um link de cancelamento de inscrição anexado à parte inferior.

**Atualização do Feed ao Vivo**

Atualizamos a aparência das guias Envolvimento e Tarefa para facilitar e agilizar a resposta dos membros de Vendas às atividades dos clientes diretamente do Feed ativo.

**Atualização da Exibição de Detalhes de Pessoas**

A PDV (Exibição de detalhes de pessoas) aprimorada oferece uma visão abrangente de seus contatos, reunindo seus detalhes de contato do Tout e do Salesforce CRM.
