---
unique-page-id: 37356893
description: Visão geral dos recursos MSI - Documentação do Marketo - Documentação do produto
title: Visão geral do recurso MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: bda95da160c5a27a0a460d26c102e6166c1ddea0
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 11%

---

# Visão geral do recurso MSI {#msi-feature-overview}

O MSI tem os seguintes recursos disponíveis no Salesforce Lightning e Classic.

>[!NOTE]
>
>Para ver todos os dados disponíveis, verifique se o zoom do seu navegador está definido como não mais do que 125% ao usar o Windows e 150% no SO Mac.

## Painel Visualforce {#visualforce-panel}

O painel MSI Visualforce inclui as seguintes funcionalidades:

* Guias

   * [Painel de insights](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Momentos interessantes
   * Atividade na Web
   * Email
   * Pontuação

* Ações

   * Adicionar à campanha do Marketo
   * Enviar e-mail do Marketo
   * Adicionar/Remover da Lista de Controle

* Estrelas e chamas

## Layout do lead {#lead-layout}

Páginas do Visualforce:

* Cliente em potencial - Inclui a opção de clicar no hiper &quot;Ir para a lista completa&quot;, você será direcionado para uma nova guia no Salesforce, onde o painel MSI estará visível em um layout de página completo
* Lista Completa de Clientes Potenciais - Não inclui a opção &quot;Ir para Lista Completa&quot;
* Lead Mobile - visível no aplicativo móvel do Salesforce
* Ponte de contato de cliente potencial - Exibe o painel MSI do contato adicionado no campo ID de contato MSI

Campos:

* Último momento interessante
* Data do último momento interessante
* Desc. do último momento interessante
* Fonte do último momento interessante
* Tipo do último momento interessante
* Última atividade do Marketo no Sales
* Último envolvimento do Marketo no Sales
* Pontuação relativa
* Valor de pontuação relativa
* Urgência
* Valor de urgência
* Exibir no Marketo - clique neste campo para abrir uma exibição não editável do cliente potencial no Marketo. Inclui: Informações do lead, Informações da empresa, Informações do lead SFDC, Campos personalizados SFDC, Log de atividades
* Id de contato MSI - Adicione um contato do Salesforce a esse campo e inclua o painel &quot;Lead Contact Bridge&quot; no layout do lead para ver o painel MSI do contato

## Layout do contato {#contact-layout}

Páginas do Visualforce:

* Contato - Inclui a opção de clicar na hiper &quot;Ir para a lista completa&quot;, você será enviado para uma nova guia no Salesforce, onde o painel MSI estará visível em um layout de página completo
* Lista Completa de Contatos - Não inclui a opção &quot;Ir para Lista Completa&quot;
* Contato móvel - Visível no aplicativo móvel Salesforce
* Adicionar à página de contato do Marketo Campaign - o recurso Adicionar ao Marketo Campaign está disponível neste painel

Campos:

* Último momento interessante
* Data do último momento interessante
* Desc. do último momento interessante
* Fonte do último momento interessante
* Tipo do último momento interessante
* Última atividade do Marketo por Vendas
* Pontuação relativa
* Valor de pontuação relativa
* Urgência
* Valor de urgência
* Exibir no Marketo - clique neste campo para abrir uma exibição não editável do cliente potencial no Marketo. Inclui: Informações do lead, Informações da empresa, Informações do lead SFDC, Campos personalizados SFDC, Log de atividades
* Pontuação de lead do Mkto
* Sales Insight - abre a página de lista completa de contatos

## Layout da conta {#account-layout}

Páginas do Visualforce:

* Conta - Inclui a opção de clicar no hiper &quot;Ir para a lista completa&quot;, você será enviado para uma nova guia no Salesforce, onde o painel MSI estará visível em um layout de página completo
* Lista Completa da Conta - Não inclui a opção &quot;Ir para Lista Completa&quot;
* Conta móvel - Visível no aplicativo móvel Salesforce

Campos:

* Sales Insight - abre a página de lista completa de contatos

Ações:

* Adicionar à campanha do Marketo
* Enviar e-mail do Marketo
* Adicionar/Remover da Lista de Controle

Os seguintes recursos são **não disponível** na página Layout da conta:

* Estrelas e chamas

## Layout da oportunidade {#opportunity-layout}

Páginas do Visualforce:

* Oportunidade - Inclui a opção de clicar na hiper &quot;Ir para a lista completa&quot;, você será direcionado para uma nova guia no Salesforce, onde o painel MSI estará visível em um layout de página inteira
* Lista completa da oportunidade - Não inclui a opção &quot;Ir para lista completa&quot;
* Oportunidade móvel - visível no aplicativo móvel do Salesforce

Campos:

* Sales Insight - abre a página de lista completa de contatos
* Análise de oportunidade da Marketo - abre o Analisador de influência de oportunidades na Marketo

Ações:

* Adicionar à campanha do Marketo
* Enviar e-mail do Marketo
* Adicionar/Remover da Lista de Controle

Os seguintes recursos são **não disponível** na página Layout da oportunidade:

* Estrelas e chamas

## Exibição da Lista de Clientes Potenciais e de Contatos (Ações em Massa) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning: adicione aos botões de ação em massa Adicionar à lista de favoritos, Adicionar ao Marketo Campaign e Enviar email do Marketo na exibição da lista de clientes potenciais e de contatos.

Salesforce Classic: adicionar à Lista de favoritos, adicionar ao Marketo Campaign e enviar botões de ação em massa do Marketo Email na exibição da Lista de clientes potenciais e de contatos.

## Guia Marketo {#marketo-tab}

* Melhores opções

   * Inclui a capacidade de criar e editar visualizações. Capacidade de Ocultar Melhores Opções dependendo da configuração da opção &quot;Ocultar Padrão&quot; na página de Configuração do Marketo
   * Colunas - Nome, Conta, Último Momento Interessante, Cabeçalho De Status, Envolvimento (Estrelas E Chamas), Ocultar

* Minha lista de observação

   * Inclui a capacidade de criar e editar visualizações
   * Colunas - Nome, Conta, Último momento interessante, Cabeçalho de status, Envolvimento (Estrelas e Chamas), Remover

* Atividade na Web

   * Inclui a capacidade de criar e editar visualizações, a funcionalidade de filtro de intervalo de tempo
   * Coluna - Exibição de página, Nome, Conta, Última visita

* Atividade anônima na Web

   * Inclui a capacidade de criar e editar visualizações, a funcionalidade de filtro de intervalo de tempo
   * Colunas - Exibição de página, Empresa, Última visita, Pesquisa (abre a página LinkedIn da empresa)

* Meu e-mail

   * Inclui a capacidade de criar e editar visualizações
   * Colunas - Nome, Conta, Assunto, Data, Abertura, Clique

* Feed de lead - Inclui a capacidade de se inscrever em momentos interessantes, o feed RSS na página Configuração deve estar habilitado para usar este recurso

   * Cliente Potencial/Contato que teve este momento interessante
   * Tipo de momento interessante (Web, email ou marco) e descrição
   * Nome da conta
   * Hora em que este momento interessante ocorreu
   * Inscreva-se na opção para receber notificação por email sobre esse tipo de evento
   * Ícone de alta prioridade para mostrar esta pessoa como Melhor Opção

## Guia Configuração do Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

* Configurações operacionais: inclui credenciais da API Soap &amp; Rest necessárias para configurar o MSI no SFDC
* Configuração MSI: inclui a configuração da guia Marketo e do painel MSI visualforce
* Redefinir o Marketo Sales Insight: inclui a capacidade de eliminar todas as configurações

>[!MORELIKETHIS]
>
>[Guia Configuração do Marketo Sales Insight no Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Relatórios de desempenho do Sales Insight {#sales-insight-performance-reports}

Exibir o desempenho de emails enviados por meio do Salesforce, Microsoft Dynamics ou de um plug-in do Gmail ou Outlook

## MSI para dispositivos móveis {#msi-for-mobile}

Os recursos MSI são compatíveis com o aplicativo móvel Salesforce

## Suporte de idioma {#language-support}

O Marketo Sales Insight é armazenado por idioma. Portanto, se você quiser que ele funcione em mais de um idioma, insira as credenciais separadamente para cada idioma.

>[!NOTE]
>
>* Um contato/lead precisa estar na partição Padrão para ser adicionado à Lista de favoritos.
>
>* O pacote MSI Salesforce não é compatível com a exibição personalizada com campos dependentes.
