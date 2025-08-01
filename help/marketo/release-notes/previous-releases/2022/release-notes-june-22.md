---
description: Notas de versão - junho de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão – Junho de 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Notas de versão: junho de 2022 {#release-notes-june-22}

Abaixo você encontrará todos os recursos incluídos na versão de junho de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo Engage para obter mais informações.

Os recursos a seguir serão lançados em **24 de junho de 2022**, com uma implantação em fases dos recursos restantes nas semanas seguintes (a menos que especificado de outra forma).

## Ambiente de dados de marketing {#marketing-data-environment}

* **Expor campos CreatedAt/UpdatedAt para Objetos Personalizados**: oferece a capacidade de inspecionar esses campos na tela de Detalhes da pessoa para obter insight adicionais.

## Orquestração entre canais {#cross-channel-orchestration}

* **Usabilidade de Stream Designer aprimorada para[!DNL Dynamic Chat]**: adicione cartões diretamente da tela Stream Designer sem a necessidade de arrastar e soltar. A interface do [!DNL Dynamic Chat] também foi aprimorada para oferecer melhor visibilidade do conteúdo em cartões individuais.

* **Regras Avançadas de Roteamento de Compromissos para[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] oferece mais opções de roteamento de compromissos direcionados. Especifique quais compromissos de agente devem ser encaminhados com base nos atributos do Marketo Engage, garantindo que os clientes potenciais sejam encaminhados aos agentes apropriados.

* **Relatórios de Caixa de Diálogo Avançada para[!DNL Dynamic Chat]**: visualize o desempenho de suas campanhas do [!DNL Dynamic Chat] com mais detalhes usando visualizações de dados totalmente novas para métricas de envolvimento e conversão.

* **Dessincronizar Atributos do Marketo Engage Não Utilizados para[!DNL Dynamic Chat]**: Dessincronize os atributos do Marketo Engage da sua assinatura do [!DNL Dynamic Chat] que não são utilizados, ajudando a facilitar a limpeza dos dados e permitindo que os atributos alternativos sejam sincronizados conforme necessário.

## Experiência da próxima geração

**Novos Modos de Exibição de Alternância**: os modos de exibição abaixo agora estão disponíveis na Experiência da Próxima Geração:

* [Exibir detalhes do email](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Exibição da Lista de Emails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automação de experiência {#experience-automation}

* **Exclusões de Regra de Validação do Campo de Formulário Global**: exclua formulários específicos das Regras de Validação do Formulário Global para que as centrais de assinaturas e outros fluxos de trabalho críticos comerciais possam aceitar todos os valores.

* **Etapas de fluxo de autoatendimento**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros da Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em Campanhas de acionador, em lote e de executável, em contraste com Webhooks, que só podem ser usados em Campanhas de acionador.

* **Rastreamento de link agnóstico de protocolo do Munchkin**: estenda o suporte ao rastreamento de links `tel` e `mailto` com o Munchkin para rastrear um conjunto expandido de comportamentos da Web.

* **Métodos HTTP adicionais para webhooks**: especifique PUT, PATCH e DELETE como tipos de solicitação para interagir com serviços Web.

## [!DNL Sales Insight] {#sales-insight}

![(estrela)](assets/yellow-star.png)

* Conjunto de Permissões **[!DNL Sales Insight]em[!DNL Salesforce]**: Os administradores podem fornecer acesso de [!DNL Sales Insight] a um conjunto limitado de pessoas no nível de usuário, em vez do nível de perfil, por meio do conjunto de permissões do Aplicativo Marketo, que faz parte do pacote [!DNL Sales Insight] [!DNL Salesforce].

* **Atualização do Meu Bloco do Marketo - [!DNL Sales Insight] Ações**: os Administradores do Marketo (e os usuários que eles designarem) agora podem navegar rapidamente para a instância de Ações do [!DNL Sales Insight] por meio de um novo bloco de Ações do [!DNL Sales Insight], localizado na página Meu Marketo.

## [!DNL Sales Connect] {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **[!DNL Salesforce]Atualização da API**: com a versão do verão de 2022 do [!DNL Salesforce], as versões herdadas da API de 21 a 30 não serão mais suportadas pelo [!DNL Salesforce]. Com esta versão do Marketo Engage, todas as [!DNL Sales Connect] solicitações que usam versões de API herdadas foram atualizadas para permanecer em uma versão com suporte. Para obter detalhes completos sobre os planos de aposentadoria da API [!DNL Salesforce], clique [aqui](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Aprimoramentos na API {#api-enhancements}

* **Novos recursos de filtragem para API de Extração de Membro de Programa em Massa**: filtre por status de associação de programa, updatedAt, cadência ou conteúdo esgotado para refinar o conjunto de dados extraído.

* **Aprimoramento da API de Extração de Membro de Programa em Massa**: especifique até 10 programas durante a criação do trabalho para melhorar a taxa de transferência.

## Anúncios {#announcements}

* **Substituição do Forms - Forms 1.0, ponto de extremidade de captura/salvamento de clientes potenciais e versões sem script de formulários**: o suporte para ativos do Forms 1.0 será completamente removido do Marketo Engage até outubro de 2022. Todos os ativos existentes do Forms 1.0 deixarão de funcionar. Os formulários do Marketo Engage exigirão que o JavaScript seja carregado nas páginas de aterrissagem e sites.

**_Webinar de lançamento de produto_**

[Webinar da versão de junho e agosto de 2022 do Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
