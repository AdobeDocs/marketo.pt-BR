---
unique-page-id: 37357276
description: Notas de versão - 20 de junho - Documentação do Marketo - Documentação do produto
title: Notas de versão - junho de 20
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Notas de versão: junho de 20 {#release-notes-june}

Os seguintes recursos estão incluídos na versão de junho de 2020. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões trimestrais_** Os seguintes recursos serão lançados em **5 de junho de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **[Públicos preditivos](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(estrela)](assets/yellow-star.png): os novos filtros Smart List e Smart Campaign viabilizados pelo Adobe Sensei permitem criar segmentos de público-alvo alimentados por IA para programas de marketing por email, evento e webinário. Use a IA para ajudar a segmentar públicos com base na probabilidade de um lead se registrar em um evento, participar de um evento ou cancelar a inscrição. Crie públicos-alvo semelhantes com base em programas anteriores para replicar com eficiência o sucesso anterior. Alcance metas de conversão com rastreamento preditivo de metas e obtenha recomendações sobre como refinar os segmentos de público-alvo para programas de eventos.
* **Aumento de email em lote** ![(estrela)](assets/yellow-star.png): melhoria em nosso recurso de marketing por email, que permite enviar até 3 milhões de emails em lote por hora. Reestruturamos nossa campanha em lote e o processamento de relatórios de email para aprimorar o desempenho de programas de email e campanhas de email em lote. Isso resulta em um lead time mais curto para envio, bem como em tempo de conclusão melhorado. Configure seus emails como você faria normalmente, não há complexidade adicional. Esse aprimoramento está disponível como um complemento de produto que também inclui um Pacote de lançamento de serviços de entrega, Ferramentas de entrega de email e vários Endereços IP dedicados.
* **[Integração de público-alvo com a Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: nova integração do Adobe Experience Cloud (AEC) que permite sincronizar listas estáticas de leads conhecidos do Marketo Engage com vários aplicativos da AEC para aprimorar os programas existentes, desbloquear novos casos de uso e orquestrar campanhas multicanais. Essa integração inclui Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campos Personalizados de Membros do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: capture e utilize campos personalizados sobre um membro do programa. Use esses novos campos em seus formulários Marketo Engage, visualize-os na lista de membros de um programa, utilize-os em filtros e acionadores de Smart List e inclua-os em uma nova Ação de fluxo de campanha inteligente para obter automação aprimorada e personalização mais granular. Eles também podem ser importados e exportados por meio da interface do usuário e das APIs. Aprimoramento do recurso de objetos e campos de dados personalizados.
* **Descrever membro do programa**: recupere os metadados do Membro do programa, fornecendo a capacidade de importar e exportar dados do Campo personalizado do Membro do programa usando a API REST. Aprimoramento da nossa API.
* **[Criar tarefa no Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: crie tarefas para Vendas dentro do Microsoft Dynamics usando uma nova Ação de fluxo com base no comportamento do cliente capturado no Marketo Engage. Aprimoramento da integração nativa do Microsoft Dynamics CRM.
* **Obter formulário usado pelo endpoint da API de ativo de lista**: recupere uma lista de ativos que dependem de um formulário. Aprimoramento da nossa API.
* **Definir pré-cabeçalho de email por meio da API**: ative a tradução e a localização automáticas dos campos de pré-cabeçalho do email. Aprimoramento da nossa API.
* **Armazenamento em cache de imagens e arquivos**: estamos aprimorando a estabilidade do servidor Marketo Engage ao veicular ativos de imagem e arquivo de um cache de 60 segundos.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **Descoberta de Nova Conta Geralmente Disponível**

   * A Nova descoberta de conta é um aprimoramento da nossa capacidade de Definição de perfil da conta. Ela permite que você descubra novas contas de destino para a sua estratégia ABM com base no modelo ideal de perfil do cliente alimentado por IA. Visualize, selecione e importe novas contas recomendadas, juntamente com seus indicadores de dados de ajuste e intenção baseados em IA.

<br> 

**_Lançamento durante todo o trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Integração de programas do Marketo Engage**: obtenha dados do programa diretamente do Marketo Engage para criar pontos de contato ao longo da jornada de atribuição na Bizible para creditar adequadamente programas de email e engajamento. Aprimoramento da integração do Marketo Engage.
* **Integração de atividades do Marketo Engage (BETA)**: Traga dados de atividade do Marketo Engage diretamente para a Bizible para criar pontos de contato na jornada do cliente e em todos os modelos de atribuição. Os exemplos incluem alterações na pontuação de clientes potenciais, momentos interessantes, cliques em emails ou qualquer atividade personalizada. Aprimoramento da integração do Marketo Engage.
* **Integração de atributos do cliente B2B da Bizible (BETA)**: esta é uma integração do Adobe Experience Cloud com o Adobe Analytics que permite trazer dados Bizible selecionados diretamente para o Adobe Analytics, para uma análise mais detalhada. Os exemplos incluem tráfego de site baseado em conta e análise de conteúdo por nome da empresa, atributos de conta, oportunidades de CRM e indivíduos de alto valor, conforme definido pela receita atribuída da Bizible e estágio de funil.
* **Filtros e aprimoramentos do Bizible Discover**: analise seus dados com filtros de canal, subcanal, campanha e segmento nos painéis. Aumente a visibilidade dos dados com mais atributos detalhados. Este é um aprimoramento dos nossos Discover Boards.
* **Sincronização de atividades para o Microsoft Dynamics**: atribua interações de vendas trazendo atividades do Microsoft Dynamics CRM para a jornada do ponto de contato e rastreie eventos como chamadas, compromissos ou tarefas associadas aos seus leads ou contatos. Aprimoramento da integração do Microsoft Dynamics CRM.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[Painel de insights para o Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: estamos reimaginando nosso recurso Sales Insight com nova visibilidade de eventos e campanhas de marketing futuros para oferecer aos vendedores a capacidade de tornar as recomendações mais relevantes para clientes e clientes potenciais com base em suas necessidades e interesses. Os vendedores também podem visualizar o Contato e a Atividade da conta na linha do tempo e acessar facilmente os detalhes adicionais da atividade. Encontre mais detalhes sobre como atualizar seu pacote [aqui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Anúncios {#announcements}

* **Atualização de ITP 2.1+ RTP**: devido a alterações na política de cookies do Safari, a capacidade dos cookies RTP de rastrear usuários em sessões no mesmo domínio será limitada pela ITP a 1 ou 7 dias, com base no navegador e na versão usada pelo visitante. Para levar em conta isso, estamos implementando um novo serviço da Web para permitir que os cookies RTP sejam definidos com um cabeçalho Set-Cookie por meio da resposta HTTP. Mais informações podem ser encontradas [aqui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Alterações na infraestrutura da campanha em lote**: estamos atualizando nossos serviços de campanha em lote durante o restante deste ano. Essa será uma atualização contínua que não afetará nenhuma campanha em lote que esteja em andamento e não resultará em uma mudança de comportamento. Nenhuma ação é necessária. Encontre mais detalhes aqui [Publicação da nação](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Desaprovações {#deprecations}

* **[Líder associado do Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: A partir da versão 159 do Munchkin JS, um aviso de desativação será registrado no console do navegador quando o método Associar lead for chamado, indicando que o recurso será removido em uma versão futura.  A programação de descontinuação completa será anunciada posteriormente.

**_Webinário de lançamento do produto_** [Assistir a gravação](https://engage.marketo.com/June-Release-2020-On-Demand.html) do nosso webinário sobre inovações na versão do produto de 20 de junho.
