---
unique-page-id: 42762322
description: Guia de configuração do Marketo Sales Insight no Salesforce - Documentos do Marketo - Documentação do produto
title: Guia de configuração do Marketo Sales Insight no Salesforce
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Guia de Configuração do Marketo Sales Insight no Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configurações operacionais {#operational-settings}

Você precisará ter essa configuração para começar a usar o Sales Insight no SFDC.

![](assets/one.png)

* O MSI usa a API Soap e Rest
* A página Informações de vendas na sua conta do Marketo terá dois painéis correspondentes com credenciais da API Soap e Rest que você pode copiar e colar aqui
* A API Soap e Rest têm tempos limite separados que podem ser definidos de acordo com as necessidades da organização. O tempo máximo permitido é de 120 segundos
* Desativar o painel do Insights: Você pode remover as credenciais da Rest API e usar somente a API Soap. Isso desativará a guia Painel de insights em todos os painéis da força de visualização MSI

## Configuração MSI {#msi-configuration}

As configurações são aplicáveis a todos os usuários MSI e não são específicas para perfis.

**Configurações da guia Marketo**

* Modo de Depuração Melhor
* Ocultar Padrão - A opção escolhida aqui será o número de dias em que uma melhor aposta estará oculta na guia Melhores Apostas do Marketo quando você clicar no ícone &quot;Ocultar&quot;
* Campo de status do contato - A opção que você escolher aqui será o valor preenchido na coluna Cabeçalho do status da guia Melhor Economia do Marketo
* Configurações da guia - Todas as 5 guias estarão disponíveis por padrão. Você pode escolher a ordem das guias na página global do Marketo

**Configurações de página da força de visita**

* Ativar o menu suspenso Ação:

   * Capacidade de ocultar o envio de email do Marketo a partir do menu suspenso no Layout MSI de cliente potencial e contato
   * Capacidade de ocultar as opções Adicionar ao Marketo Campaign do menu suspenso no Layout MSI de lead e contato

* Eventos futuros: Capacidade de mostrar eventos convidados, todos os eventos para usuários ou ocultar totalmente essa guia
* Próximas campanhas: Capacidade de mostrar todas as campanhas de email ou ocultar completamente essa guia
* Carregar campanhas e eventos futuros: Capacidade de reduzir o número de chamadas de Rest API feitas pelos usuários, colocando eventos e campanhas atrás de uma guia sob demanda &quot;Carregar itens futuros&quot;
* Configurações da guia - Todas as 5 guias estarão disponíveis por padrão. Todas as 5 guias estarão disponíveis por padrão. Você pode escolher a ordem das guias no painel Sales Insight . A mesma ordem será aplicável a todo o layout (Lead, Contato, Conta, Oportunidade)

![](assets/two.png)

**Limites**

* Por padrão, a Atividade (Momento Interessante, Atividade da Web, Email) é definida como 1000. Por padrão, campanhas e eventos de email são definidos como 200
* Caso observe problemas de tempo limite em sua organização, é possível reduzir o limite

## Redefinir informações de vendas do Marketo {#reset-marketo-sales-insight}

A opção de fazer isso limpará todas as suas configurações no SFDC e elas não poderão ser restauradas. Você terá que reconfigurar tudo novamente.

![](assets/three.png)

>[!MORELIKETHIS]
>
>[Configuração do insight de vendas para sua equipe](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
