---
unique-page-id: 42762514
description: Visão geral dos recursos do painel de insights - Documentação do Marketo - Documentação do produto
title: Visão geral do recurso Painel de insights
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# Visão geral do recurso Painel de insights {#insights-dashboard-feature-overview}

Saiba mais sobre os recursos disponíveis no painel do Sales Insights.

>[!PREREQUISITES]
>
>Você deve ter o pacote MSI SFDC mais recente e a [configuração](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Layout do contato {#contact-layout}

**Grade Velocidade do Compromisso**

* Esta grade inteligente inclui Momentos interessantes, Email e Atividade da Web nos últimos 90 dias
* O usuário pode optar por &quot;Mostrar a atividade da conta&quot;. Isso criará camadas em todo o nível de conta Momentos interessantes, Email e Atividade da Web na exibição de contato
* O usuário pode destacar a semana específica para ver as atividades dentro dessa semana
* Exibição padrão: a semana atual está selecionada

**Detalhamento e Resumo do Engajamento**

* Detalhe os cartões de atividade de Momentos interessantes, Email e Atividade na Web
* Cartão de atividades de momentos interessantes - Inclui a opção de assinatura
* Cartão de atividade de email - Inclui a opção de visualização
* Cartão de Atividade na Web - Inclui a capacidade de clicar em um link
* A barra de Resumo semanal mostrará Momentos interessantes, Atividade de email e da Web nessa semana. Cada ícone é clicável e pode ser usado como filtros para mostrar uma atividade específica
* Exibição padrão: é uma lista de atividades da exibição atual

**Campanhas e eventos futuros de email**

Guia Campanhas de email:

* Inclui campanhas que fazem parte de programas de email ou programas padrão agendados para os próximos 90 dias
* Não específico do contato/lead (ou seja, lista de campanhas é uma lista genérica de todas as campanhas de email agendadas na instância do Marketo). A lista de campanhas em todos os painéis de cliente potencial, contato, conta e oportunidade será a mesma
* Se a recorrência da campanha for executada mais de três vezes nos próximos 90 dias, somente as próximas três execuções serão exibidas em determinado momento (semelhante ao comportamento no Marketo)
* O cartão de detalhes da atividade nesta seção terá uma opção de visualização. Se o fluxo incluir várias etapas de envio de email, todos os emails estarão disponíveis para visualização. Na etapa Enviar fluxo de email, se houver várias &quot;opções de email&quot;, a opção padrão estará disponível para visualização
* Os filtros incluem &quot;Pesquisa&quot; e &quot;Intervalo de datas&quot;

![](assets/insights-dashboard-feature-overview-2.png)

Guia Evento:

* Inclui Programas de Eventos agendados para os próximos 90 dias
* Use a opção de filtro para ver todos os eventos/eventos convidados (com base nas configurações de Administrador)
* Selecionar eventos convidados mostrará os eventos para os quais um contato específico foi convidado, juntamente com o status do membro
* Selecionar todos os eventos mostrará a lista de eventos agendados nos próximos 90 dias
* O cartão Detalhes da atividade nesta seção tem uma opção de visualização
* O filtro inclui &quot;Pesquisa&quot;, &quot;Mostrar somente eventos convidados&quot; e &quot;Intervalo de datas&quot;

![](assets/insights-dashboard-feature-overview-3.png)

## Layout do lead {#lead-layout}

**Grade Velocidade do Compromisso**

* Esta grade inteligente inclui Momentos interessantes, Email e Atividade da Web nos últimos 90 dias
* O usuário pode destacar a semana específica para ver as atividades dentro dessa semana
* Exibição padrão: a semana atual está selecionada
* O recurso &quot;Mostrar atividade da conta&quot; não está disponível em clientes potenciais, pois não faz parte de nenhuma conta no Salesforce até ser convertido em um contato

**Detalhamento e Resumo do Engajamento**

* Cartões de atividade detalhados para Momentos interessantes, Email e Atividade na Web
* Cartão de atividades de momentos interessantes - Inclui a opção de assinatura
* Cartão de atividade de email - Inclui a opção de visualização
* Cartão de Atividade na Web - Inclui a capacidade de clicar em um link
* A barra de Resumo semanal mostrará Momentos interessantes, Atividade de email e da Web nessa semana. Cada ícone é clicável e pode ser usado como filtros para mostrar uma atividade específica
* Exibição padrão: é uma lista de atividades da exibição atual

**Campanhas e Eventos de Email Futuros:**

Guia Campanhas de email:

* Inclui campanhas que fazem parte de programas de email ou programas padrão agendados para os próximos 90 dias
* Não específico do contato/lead (ou seja, lista de campanhas é uma lista genérica de todas as campanhas de email agendadas na instância do Marketo). A lista de campanhas em todos os painéis de cliente potencial, contato, conta e oportunidade será a mesma
* Se a recorrência da campanha for executada mais de três vezes nos próximos 90 dias, somente as próximas três execuções serão exibidas em determinado momento (semelhante ao comportamento no Marketo)
* O cartão de detalhes da atividade nesta seção terá uma opção de visualização. Se o fluxo incluir várias etapas de envio de email, todos os emails estarão disponíveis para visualização. Na etapa Enviar fluxo de email, se houver várias &quot;opções de email&quot;, a opção padrão estará disponível para visualização
* Os filtros incluem &quot;Pesquisa&quot; e &quot;Intervalo de datas&quot;

![](assets/insights-dashboard-feature-overview-4.png)

Guia Evento:

* Inclui Programas de Eventos agendados para os próximos 90 dias
* Use a opção de filtro para ver todos os eventos/eventos convidados (com base nas configurações de Administrador)
* Selecionar eventos convidados mostrará os eventos para os quais um contato específico foi convidado, juntamente com o status do membro
* Selecionar todos os eventos mostrará a lista de eventos agendados nos próximos 90 dias
* O cartão Detalhes da atividade nesta seção tem uma opção de visualização
* O filtro inclui &quot;Pesquisa&quot;, &quot;Mostrar somente eventos convidados&quot; e &quot;Intervalo de datas&quot;

![](assets/insights-dashboard-feature-overview-5.png)

## Layout da conta {#account-layout}

**Grade Velocidade do Compromisso**

* Esta grade inteligente inclui Momentos interessantes, Email e Atividade da Web nos últimos 90 dias para todos os contatos na conta
* O usuário pode destacar a semana específica para ver as atividades dentro dessa semana
* Exibição padrão: a semana atual está selecionada

**Detalhamento e Resumo do Compromisso**

* Cartões de atividade detalhados para Momentos interessantes, Email e Atividade na Web, incluindo nome de contato
* Cartão de atividades de momentos interessantes - Inclui a opção de assinatura
* Cartão de atividade de email - Inclui a opção de visualização
* Cartão de Atividade na Web - Inclui a capacidade de clicar em um link
* A barra de Resumo semanal mostrará Momentos interessantes, Atividade de email e da Web nessa semana. Cada ícone é clicável e pode ser usado como filtros para mostrar uma atividade específica
* Exibição padrão: é uma lista de atividades da exibição atual

**Campanhas e eventos futuros de email**

Guia Campanhas de email:

* Inclui campanhas que fazem parte de programas de email ou programas padrão agendados para os próximos 90 dias
* Não específico do contato/lead (ou seja, lista de campanhas é uma lista genérica de todas as campanhas de email agendadas na instância do Marketo). A lista de campanhas em todos os painéis de cliente potencial, contato, conta e oportunidade será a mesma
* Se a recorrência da campanha for executada mais de três vezes nos próximos 90 dias, somente as próximas três execuções serão exibidas em determinado momento (semelhante ao comportamento no Marketo)
* O cartão de detalhes da atividade nesta seção terá uma opção de visualização. Se o fluxo incluir várias etapas de envio de email, todos os emails estarão disponíveis para visualização. Na etapa Enviar fluxo de email, se houver várias &quot;opções de email&quot;, a opção padrão estará disponível para visualização
* Os filtros incluem &quot;Pesquisa&quot; e &quot;Intervalo de datas&quot;

Guia Evento:

* Inclui Programas de Eventos agendados para os próximos 90 dias
* Use a opção de filtro para ver todos os eventos/eventos convidados (com base nas configurações de Administrador)
* Selecionar eventos convidados mostrará os eventos para os quais um contato específico foi convidado, juntamente com o status do membro
* Selecionar todos os eventos mostrará a lista de eventos agendados nos próximos 90 dias
* O cartão Detalhes da atividade nesta seção tem uma opção de visualização
* O filtro inclui &quot;Pesquisa&quot;, &quot;Mostrar somente eventos convidados&quot; e &quot;Intervalo de datas&quot;

## Layout da oportunidade {#opportunity-layout}

**Grade Velocidade do Compromisso**

* Esta grade inteligente inclui Momentos interessantes, Email e Atividade da Web nos últimos 90 dias para todos os contatos na oportunidade
* O usuário pode destacar a semana específica para ver as atividades dentro dessa semana
* Exibição padrão: a semana atual está selecionada

**Detalhamento e Resumo do Compromisso**

* Cartões de atividade detalhados para Momentos interessantes, Email e Atividade na Web, incluindo nome de contato
* Cartão de atividades de momentos interessantes - Inclui a opção de assinatura
* Cartão de atividade de email - Inclui a opção de visualização
* Cartão de Atividade na Web - Inclui a capacidade de clicar em um link
* A barra de Resumo semanal mostrará Momentos interessantes, Atividade de email e da Web nessa semana. Cada ícone é clicável e pode ser usado como filtros para mostrar uma atividade específica
* Exibição padrão: é uma lista de atividades da exibição atual

**Campanhas e eventos de email futuros** guia Campanhas de email:

* Inclui campanhas que fazem parte de programas de email ou programas padrão agendados para os próximos 90 dias
* Não específico do contato/lead (ou seja, lista de campanhas é uma lista genérica de todas as campanhas de email agendadas na instância do Marketo). A lista de campanhas em todos os painéis de cliente potencial, contato, conta e oportunidade será a mesma
* Se a recorrência da campanha for executada mais de três vezes nos próximos 90 dias, somente as próximas três execuções serão exibidas em determinado momento (semelhante ao comportamento no Marketo)
* O cartão de detalhes da atividade nesta seção terá uma opção de visualização. Se o fluxo incluir várias etapas de envio de email, todos os emails estarão disponíveis para visualização. Na etapa Enviar fluxo de email, se houver várias &quot;opções de email&quot;, a opção padrão estará disponível para visualização
* Os filtros incluem &quot;Pesquisa&quot; e &quot;Intervalo de datas&quot;

Guia Evento:

* Inclui Programas de Eventos agendados para os próximos 90 dias
* Use a opção de filtro para ver todos os eventos/eventos convidados (com base nas configurações de Administrador)
* Selecionar eventos convidados mostrará os eventos para os quais um contato específico foi convidado, juntamente com o status do membro
* Selecionar todos os eventos mostrará a lista de eventos agendados nos próximos 90 dias
* O cartão Detalhes da atividade nesta seção tem uma opção de visualização
* O filtro inclui &quot;Pesquisa&quot;, &quot;Mostrar somente eventos convidados&quot; e &quot;Intervalo de datas&quot;

>[!NOTE]
>
>Se sua conta ou oportunidade tiver mais de 800 contatos, o painel não exibirá dados. No entanto, você pode acessar contatos individuais para ver seus insights e engajamento. Se sua conta tiver mais de 800 contatos, a opção &quot;Mostrar atividade no nível da conta&quot; será desativada.
