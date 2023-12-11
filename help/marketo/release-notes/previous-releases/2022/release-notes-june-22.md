---
description: Notas de versão - junho de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - junho de 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Notas de versão: junho de 2022 {#release-notes-june-22}

Abaixo você encontrará todos os recursos incluídos na versão de junho de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

Os recursos a seguir começarão a ser lançados em **24 de junho de 2022**, com uma implantação em fases dos recursos restantes nas semanas subsequentes (a menos que especificado de outra forma).

## Ambiente de dados de marketing {#marketing-data-environment}

* **Expor campos CreatedAt/UpdatedAt para objetos personalizados**: oferece a capacidade de inspecionar esses campos na tela Detalhes da pessoa para obter informações adicionais.

## Orquestração entre canais {#cross-channel-orchestration}

* **Usabilidade aprimorada do Stream Designer para Dynamic Chat**: adicione cartões diretamente da tela do Stream Designer sem a necessidade de arrastar e soltar. A interface Dynamic Chat também foi aprimorada para oferecer melhor visibilidade do conteúdo em cartões individuais.

* **Regras Avançadas de Roteamento de Compromissos para o Dynamic Chat**: o Dynamic Chat oferece mais opções para o roteamento de compromissos direcionados. Especifique quais compromissos de agente devem ser encaminhados com base nos atributos de Marketo Engage, garantindo que os clientes potenciais sejam encaminhados aos agentes apropriados.

* **Relatórios avançados de diálogo para o Dynamic Chat**: visualize o desempenho de suas campanhas do Dynamic Chat com mais detalhes usando visualizações de dados totalmente novas para métricas de engajamento e conversão.

* **Dessincronizar atributos de Marketo Engage não utilizados para o Dynamic Chat**: não sincronize atributos de Marketo Engage da sua assinatura de Dynamic Chat que não são usados, ajudando você a facilitar a limpeza dos dados e permitindo que atributos alternativos sejam sincronizados conforme necessário.

## Experiência da próxima geração

**Novas Visualizações de Alternância**: as exibições abaixo agora estão disponíveis na Experiência de próxima geração:

* [Exibição de detalhes do email](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Exibição da lista de e-mails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automação de experiência {#experience-automation}

* **Exclusões da regra de validação do campo de formulário global**: exclua formulários específicos das Regras de validação de formulário global para que as centrais de assinaturas e outros fluxos de trabalho críticos para os negócios possam aceitar todos os valores.

* **Etapas de fluxo de autoatendimento**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros do Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em Campanhas de acionador, em lote e de executáveis, em contraste com Webhooks, que só podem ser usados em Campanhas de acionador.

* **Rastreamento de link agnóstico do protocolo Munchkin**: estenda o suporte para rastreamento do `tel` e `mailto` links com Munchkin para rastrear um conjunto expandido de comportamentos da web.

* **Métodos HTTP adicionais para webhooks**: especifique PUT, PATCH e DELETE como tipos de solicitação para interagir com os serviços da Web.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **Permissão de Insight de vendas definida no Salesforce**: os administradores podem fornecer acesso ao Sales Insight a um conjunto limitado de pessoas no nível do usuário, em vez do nível do perfil, por meio do conjunto de permissões do aplicativo Marketo, que faz parte do pacote Sales Insight Salesforce.

* **Atualização do meu bloco do Marketo - Ações do Sales Insight**: os administradores do Marketo (e os usuários que eles designarem) agora podem navegar rapidamente para a instância de Ações do Sales Insight por meio de um novo bloco Ações do Sales Insight localizado na página Meu Marketo.

## Conexão de vendas {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Atualização da API do Salesforce**: com a versão do Salesforce no verão de 22, as versões herdadas da API 21-30 não serão mais compatíveis com o Salesforce. Com esta versão do Marketo Engage, todas as solicitações do Sales Connect usando versões de API herdadas foram atualizadas para permanecer em uma versão compatível. Para obter detalhes completos sobre os planos de retirada da API do Salesforce, clique em [aqui](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## Aprimoramentos na API {#api-enhancements}

* **Novos recursos de filtragem para a API de extração de membros de programa em massa**: filtre por status de associação de programa, conteúdo atualizado em, cadência ou esgotado para refinar o conjunto de dados extraído.

* **Aprimoramento da API de extração de membro do programa em massa**: especifique até 10 programas durante a criação do trabalho para melhorar a taxa de transferência.

## Anúncios {#announcements}

* **Substituição do Forms - Forms 1.0, endpoint de captura/salvamento de clientes potenciais e versões sem script de formulários**: o suporte aos ativos do Forms 1.0 será completamente removido do Marketo Engage até outubro de 2022. Todos os ativos existentes do Forms 1.0 deixarão de funcionar. Os formulários Marketo Engage exigirão que o JavaScript seja carregado nas páginas de aterrissagem e sites.

**_Webinário de lançamento do produto_**

[Webinário da versão de Marketo Engage de junho e agosto de 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
