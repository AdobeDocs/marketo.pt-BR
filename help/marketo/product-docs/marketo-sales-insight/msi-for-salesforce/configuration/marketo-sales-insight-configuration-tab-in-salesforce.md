---
unique-page-id: 42762322
description: Guia Configuração do Marketo Sales Insight no Salesforce - Documentos da Marketo - Documentação do produto
title: Guia Configuração do Marketo Sales Insight no Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Guia Configuração do Marketo Sales Insight no Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configurações operacionais {#operational-settings}

Você precisará ter essa configuração para começar a usar o Sales Insight no SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* O MSI usa a API Soap e Rest
* A página Informações de vendas na sua conta do Marketo terá dois painéis correspondentes com credenciais da API Soap e Rest que você pode copiar e colar aqui
* A API Soap e Rest têm tempos limite separados que podem ser definidos de acordo com as necessidades da organização. O tempo máximo permitido é de 120 segundos
* Desativar o painel do Insights: Você pode remover as credenciais da Rest API e usar somente a API Soap. Isso desativará a guia Painel de insights em todos os painéis da força de visualização MSI

## Configuração MSI {#msi-configuration}

As configurações são aplicáveis a todos os usuários MSI e não são específicas para perfis.

**Configurações de página da força de visita**

* Ativar o menu suspenso Ação:
   * Capacidade de ocultar o envio de email do Marketo a partir do menu suspenso no Layout MSI de Cliente Potencial e Contato
   * Capacidade de ocultar as opções Adicionar ao Marketo Campaign do menu suspenso em Lead e Entrar em contato com o layout MSI
* Eventos futuros: Capacidade de mostrar eventos convidados, todos os eventos para usuários ou ocultar completamente essa guia
* Próximas campanhas: Capacidade de mostrar todas as campanhas de email ou ocultar completamente essa guia
* Carregar campanhas e eventos futuros: Capacidade de reduzir o número de chamadas de Rest API feitas pelos usuários, colocando eventos e campanhas atrás de uma guia sob demanda &quot;Carregar itens futuros&quot;
* Configurações da guia: Todas as cinco guias estarão disponíveis por padrão. Você pode escolher a ordem das guias no painel Sales Insight . A mesma ordem será aplicável a todos os layouts (lead, contato, conta, oportunidade)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Guia Global do Marketo**

* Feed RSS Habilitado: Quando ativados, os usuários do MSI podem visualizar seu Feed de lead em um feed RSS (além do Feed de lead no Salesforce). O feed RSS só pode funcionar se o recurso &quot;Expiração do token&quot; estiver desativado. Essa configuração é controlada na página do Administrador do Marketo Sales Insight.
* Modo de depuração das melhores opções
* Ocultar Padrão: A opção escolhida aqui será o número de dias em que uma melhor aposta estará oculta na guia Melhores Ofertas do Marketo ao clicar no ícone &quot;Ocultar&quot;
* Campo de status do contato: A opção escolhida aqui será o valor preenchido na coluna Cabeçalho do Status na guia Melhores Melhores Opções do Marketo
* Configurações do feed ao vivo: A opção de optar por mostrar somente o Feed em tempo real (nos painéis de Lead, Contato, Conta e Oportunidade e na página Marketo Global), somente o Feed de Lead (na Página Global da Marketo) ou o Feed em tempo real e de lead
* Configurações da guia: Todas as cinco guias estarão disponíveis por padrão. Você pode escolher a ordem das guias na página global do Marketo

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Limites**

* Por padrão, a Atividade (Momento Interessante, Atividade da Web, Email) é definida como 1000. Por padrão, campanhas e eventos de email são definidos como 200
* Caso observe problemas de tempo limite em sua organização, é possível reduzir o limite

**Configurações de ação**

* Enviar email do Marketo: Ativar isso dará a todos os usuários do Sales Insight acesso para enviar emails do lead, contato, conta, painéis de oportunidades e da guia Melhores vantagens (ações em massa e envolvimento em linha)
* Adicionar ao Marketo Campaign: Ativar isso dará a todos os usuários do Sales Insight acesso para adicionar campanhas a partir do lead, contato, conta, painéis de oportunidades e da guia Melhores vantagens (ações em massa e envolvimento em linha)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Redefinir Insight de Vendas da Marketo {#reset-marketo-sales-insight}

A opção de fazer isso limpará todas as suas configurações no SFDC e elas não poderão ser restauradas. Você terá que reconfigurar tudo novamente.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!IMPORTANT]
>
>Não marque a caixa de seleção &quot;Ativar ações MSI&quot;, a menos que esteja usando os recursos de Ações de insights de vendas.

>[!MORELIKETHIS]
>
>[Adicionar acesso ao insight de vendas a perfis](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}
