---
unique-page-id: 14352405
description: Configurando SSO por meio do SAML 2.0 no Sales Connect - Documentos do Marketing - Documentação do produto
title: Configurando SSO por meio do SAML 2.0 no Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Configurando SSO por meio do SAML 2.0 no Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Oferecemos suporte ao SSO através da especificação SAML 2.0. No entanto, não temos integrações diretas com nenhum provedor no momento. Precisaremos coletar algumas informações do seu provedor SSO para obter essa configuração.

>[!NOTE]
>
>**Lembrete**
>
>Isso só se aplica aos clientes do **Marketing** Sales Connect. Se você não tiver o Sales Connect, mas quiser saber mais, entre em contato com seu Gerente de sucesso do cliente.

## Requisitos {#requirements}

* Conta SSO
* Subscrição de conexão de Vendas do Marketing
* Metadata.xml da conta SSO (URL de edição, ponto de extremidade para validação e chave pública)

## Configuração {#setup}

O arquivo metadata.xml da instância SSO da sua equipe deve conter o URL do emissor, o terminal para validação e uma chave pública.

Também será necessário que a Localização SSO da sua conta SSO do empresa seja um domínio exclusivo. Por exemplo, nós `require a unique subdomain` gostamos de &quot;toutapp.pingidentity.com&quot; ou similar. Sem esse tipo de identificador exclusivo, não será possível configurar o SAML a partir do painel.

Um logon e o Okta nem sempre fornecem identificadores únicos ao atribuir um URL. Se você estiver usando Okta ou One Login, isso significa que não poderemos configurar um logon a partir do botão painel. Ainda assim, poderemos configurá-lo a partir do botão Logon único no aplicativo [da](http://toutapp.com/login)Web.

Assim que tivermos essas informações, trabalharemos com nossa equipe de engenharia para configurar isso para sua subscrição.
