---
unique-page-id: 42762322
description: Guia Configuração do Marketing Insight do setor de Vendas no Salesforce - Documentos do Marketing - Documentação do produto
title: Guia Configuração do Marketing Insight do setor de Vendas no Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Guia Configuração do Marketing Insight do setor de Vendas no Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configurações operacionais {#operational-settings}

Será necessário ter essa configuração para start usando o Sales Insight no SFDC.

![](assets/one.png)

* O MSI usa a API Soap e Rest
* A página de Informações de vendas na sua conta de Marketing terá dois painéis correspondentes com credenciais de API Soap e Rest que você pode copiar e colar aqui
* A API Soap e Rest tem tempos limite separados que você pode definir com base nas necessidades de sua organização. O tempo máximo permitido é de 120 segundos
* Desabilitando o Painel Insights: Você pode remover as credenciais da Rest API e usar somente a Soap API. Isso desativará a guia Painel Insights em todos os painéis MSI

## Configuração MSI {#msi-configuration}

As configurações são aplicáveis a todos os usuários de MSI e não são específicas aos perfis.

**Configurações da guia Marketo**

* Modo de Depuração de Melhores Melhoras
* Ocultar padrão - a opção que você escolher aqui será o número de dias em que uma melhor aposta ficará oculta na guia Melhores apostas no Marketo quando você clicar no ícone &quot;Ocultar&quot;
* Campo de status do contato - a opção que você escolher aqui será o valor preenchido na coluna Cabeçalho do status da guia Melhores apostas em Marketo
* Configurações de guia - Todas as cinco guias estarão disponíveis por padrão. Você pode escolher a ordem das guias na página global Marketo

**Configurações da página de força de visita**

* Menu suspenso Ativar ação:

   * Capacidade de ocultar Enviar e-mail para marketing do menu suspenso no Layout MSI de cliente potencial e contato
   * Capacidade de ocultar as opções de Adicionar à Campanha de marketing do menu suspenso no Layout MSI de cliente potencial e contato

* Eventos futuros: Capacidade de mostrar eventos convidados, todos eventos para usuários ou ocultar completamente esta guia
* Campanhas futuras: Capacidade de mostrar todas as campanhas de e-mail ou ocultar completamente esta guia
* Configurações de guia - Todas as cinco guias estarão disponíveis por padrão. Todas as cinco guias estarão disponíveis por padrão. Você pode escolher a ordem das guias no painel Sales Insight. A mesma ordem será aplicável a todos os layouts (Lead, Contact, Conta, Oportunidade)

![](assets/two.png)

**Limites**

* A atividade (Momento Interessante, Atividade da Web, E-mail) é definida como 1000 por padrão. Por padrão, campanhas e Eventos de e-mail são definidos como 200
* Caso observe problemas de tempo limite na sua organização, você pode reduzir o limite

## Redefinir insight de vendas do Marketing to {#reset-marketo-sales-insight}

A opção de fazer isso limpará todas as suas configurações no SFDC e elas não poderão ser restauradas. Você terá que reconfigurar tudo novamente.

![](assets/three.png)

