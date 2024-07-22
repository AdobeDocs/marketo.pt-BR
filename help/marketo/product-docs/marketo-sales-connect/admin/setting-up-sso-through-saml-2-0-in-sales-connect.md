---
unique-page-id: 14352405
description: Configuração de SSO por meio do SAML 2.0 no Sales Connect - Documentação do Marketo - Documentação do produto
title: Configuração de SSO por meio do SAML 2.0 no Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Configuração de SSO por meio do SAML 2.0 no Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Oferecemos suporte a SSO por meio da especificação SAML 2.0. No entanto, não temos integrações diretas com nenhum provedor no momento. Precisaremos coletar algumas informações do seu provedor de SSO para obter essa configuração.

>[!NOTE]
>
>Isso só é aplicável a usuários do **Marketo Sales Connect**. Se você não tiver o Sales Connect, mas quiser saber mais, entre em contato com a equipe de conta do Adobe (seu gerente de conta).

## Requisitos {#requirements}

* Conta SSO
* Assinatura do Marketo Sales Connect
* Metadata.xml da conta SSO (URL da ocorrência, o endpoint para validação e uma chave pública)

## Configuração {#setup}

O metadata.xml da instância do SSO da sua equipe deve conter o URL do emissor, o endpoint para validação e uma chave pública.

Também precisaremos que a Localização do SSO da sua conta de SSO seja um domínio exclusivo. Por exemplo, precisamos de um subdomínio exclusivo como `toutapp.pingidentity.com` ou similar. Sem esse tipo de identificador exclusivo, não poderemos configurar o SAML no painel.

Um logon e o Okta nem sempre fornecem identificadores exclusivos ao atribuir um URL. Se você estiver usando o Okta ou One Login, significa que não será possível configurar um login através do botão do painel. Ainda poderemos configurá-lo a partir do botão Logon Único no [aplicativo Web](https://toutapp.com/login).

Quando tivermos essas informações, trabalharemos com nossa equipe de engenharia para configurar isso para sua assinatura.
