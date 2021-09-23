---
unique-page-id: 37357276
description: Notas de versão - 20 de junho - Documentos da Marketo - Documentação do produto
title: Notas de versão - junho de 2020
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Notas de versão: Junho de 20 {#release-notes-june}

Os seguintes recursos estão incluídos na versão de 20 de junho. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestraisOs seguintes recursos serão lançados em 5_** de junho de 2020 ****.

## Marketo Engage principal {#core-marketo-engage}

* **[Públicos preditivos](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![ (estrela)](assets/yellow-star.png): Os novos filtros Smart List e Smart Campaign fornecidos pela Adobe Sensei permitem criar segmentos de público-alvo alimentados por IA para programas de email, evento e marketing de webinar. Use a IA para ajudar a segmentar públicos com base na probabilidade de lead de se registrar em um evento, participar de um evento ou cancelar a assinatura. Crie públicos semelhantes com base em programas anteriores para replicar com eficiência o sucesso anterior. Alcance metas de conversão com rastreamento preditivo de metas e obtenha recomendações sobre como refinar seus segmentos de público-alvo para programas de eventos.
* **Aumento do e-mail em lote** ![ (estrela)](assets/yellow-star.png): Aprimoramento do nosso recurso de marketing por email, que permite enviar até 3 milhões de emails em lote por hora. Reprojetamos nossa campanha em lote e o processamento de relatórios por email para aprimorar o desempenho de programas de email e campanhas de email em lote. Isso resulta em menos tempo de lead para o envio, bem como em um tempo de conclusão aprimorado. Configure seus envios de email normalmente, não há mais complexidade. Esse aprimoramento está disponível como um complemento de produto que também inclui um pacote de lançamento de serviços de entrega, ferramentas de entrega de email e vários endereços IP dedicados.
* **[Integração de público-alvo com o Adobe Experience Cloud (AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Nova integração do Adobe Experience Cloud (AEC) que permite sincronizar listas estáticas de leads conhecidos do Marketo Engage com vários aplicativos AEC para aprimorar programas existentes, desbloquear novos casos de uso e orquestrar campanhas de vários canais. Essa integração inclui Adobe Analytics, Adobe Target, Adobe Experience Manager, Adobe Audience Manager e Adobe Advertising Cloud.
* **[Campos personalizados do membro do programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**: Capture e utilize campos personalizados sobre um membro do programa. Use esses novos campos em seus formulários do Marketo Engage, visualize-os em uma lista de membros do programa, aproveite-os em filtros e acionadores da Smart List e inclua-os em uma nova Ação de fluxo de campanha inteligente para automação aprimorada e personalização mais granular. Eles também podem ser importados e exportados por meio da interface do usuário e das APIs do . Aprimoramento do recurso de objetos de dados e campos personalizados.
* **Descrever Membro** do Programa: Recupere os metadados do Membro do Programa, permitindo importar e exportar os dados do Campo Personalizado do Membro do Programa usando a REST API. Aprimoramento da nossa API.
* **[Criar tarefa no Microsoft Dynamics](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**: Crie tarefas para Vendas no Microsoft Dynamics usando uma nova Ação de Fluxo com base no comportamento do cliente capturado no Marketo Engage. Aprimoramento da integração nativa do Microsoft Dynamics CRM.
* **Obter formulário usado pelo ponto de extremidade** da API de ativos de lista: Recupere uma lista de ativos que dependem de um formulário. Aprimoramento da nossa API.
* **Definir Precabeçalho de email por API**: Habilite a tradução automática e a localização dos campos de pré-cabeçalho de email. Aprimoramento da nossa API.
* **Armazenamento em cache** de imagens e arquivos: Estamos aprimorando a estabilidade do servidor do Marketo Engage, disponibilizando ativos de imagem e arquivo de um cache de 60 segundos.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **Descoberta de Nova Conta Geralmente Disponível**

   * A New Account Discovery é um aprimoramento da nossa capacidade de criação de perfis de contas que permite descobrir novas contas-alvo para sua estratégia de ABM com base no modelo ideal de perfil de cliente desenvolvido por IA. Exiba, selecione e importe novas contas recomendadas, juntamente com seus indicadores de dados de ajuste e intenção baseados em IA.

<br> 

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Integração** de programas Marketo Engage: Puxe os dados do programa diretamente do Marketo Engage para criar pontos de contato ao longo da jornada de atribuição na Bizible para creditar apropriadamente os programas de email e de envolvimento. Aprimoramento da integração com o Marketo Engage.
* **Integração de atividades do Marketo Engage (BETA)**: Traga os dados de atividade do Marketo Engage diretamente para a Bizible para criar pontos de contato na jornada do cliente e em todos os modelos de atribuição. Os exemplos incluem alterações de pontuação de lead, momentos interessantes, clique de email ou qualquer atividade personalizada. Aprimoramento da integração com o Marketo Engage.
* **Integração Bizible B2B de atributos do cliente (BETA)**: Esta é uma integração do Adobe Experience Cloud com o Adobe Analytics que permite trazer dados Bizible selecionados diretamente para o Adobe Analytics para uma análise mais profunda. Os exemplos incluem tráfego de site baseado em conta e análise de conteúdo por nome de empresa, atributos de conta, oportunidades de CRM e indivíduos de alto valor, conforme definido pela receita atribuída da Bizible e estágio de funil.
* **Filtros e aprimoramentos** Bizible Discover: Analise seus dados com filtros de canal, subcanal, campanha e segmento nos painéis. Fortaleça a visibilidade dos dados com mais atributos detalhados. Este é um aprimoramento dos nossos quadros do Discover.
* **Sincronização de atividades para o Microsoft Dynamics**: Atribua interações de vendas ao trazer as atividades do Microsoft Dynamics CRM para a jornada do ponto de contato e rastreie eventos como chamadas, compromissos ou tarefas associadas aos seus leads ou contatos. Aprimoramento da integração com o Microsoft Dynamics CRM.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[Painel de insights para o Salesforce CRM](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**: Estamos reimaginando nosso recurso de Sales Insight com uma nova visibilidade dos eventos e campanhas de marketing futuros para dar aos vendedores a capacidade de tornar as recomendações mais relevantes para os clientes e clientes potenciais com base em suas necessidades e interesses. Os vendedores também podem visualizar o Contato e a Atividade da conta na linha do tempo e acessar facilmente os detalhes adicionais da atividade. Encontre mais detalhes sobre como atualizar seu pacote [aqui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## Anúncios {#announcements}

* **Atualização** de RTP ITP 2.1+: Devido a alterações na política de cookies do Safari, a capacidade dos cookies RTP de rastrear usuários em sessões no mesmo domínio será limitada pelo ITP a 1 ou 7 dias com base na versão do navegador e do navegador usada pelo visitante. Para levar isso em conta, estamos implementando um novo serviço da Web para permitir que os cookies RTP sejam definidos com um cabeçalho Set-Cookie por meio da resposta HTTP. Mais informações podem ser encontradas [aqui](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **Alterações** na infraestrutura da campanha em lote: Estamos atualizando nossos serviços de campanha em lote durante o resto do ano. Esta será uma atualização contínua que não afetará nenhuma campanha em lote que esteja em andamento e não resultará em uma mudança de comportamento. Nenhuma ação é necessária. Encontre mais detalhes neste [Nation post](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## Descontinuações {#deprecations}

* **[Líder](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** da Associação Munchkin: A partir da versão 159 do Munchkin JS, um aviso de desativação será registrado no console do navegador quando o método Associar lead for chamado, indicando que o recurso será removido em uma versão futura.  O cronograma completo de descontinuação será anunciado em uma data posterior.

**_Webinar da versão do produtoAssista ao_** [ ](https://engage.marketo.com/June-Release-2020-On-Demand.html) registro do nosso webinário de inovações da versão do produto de 20 de junho.
