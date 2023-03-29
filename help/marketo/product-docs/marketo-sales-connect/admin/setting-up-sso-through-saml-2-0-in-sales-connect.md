---
unique-page-id: 14352405
description: Configuração do SSO por meio do SAML 2.0 no Sales Connect - Documentos da Marketo - Documentação do produto
title: Configurando SSO por meio do SAML 2.0 no Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Configurando SSO por meio do SAML 2.0 no Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Oferecemos suporte ao SSO por meio da especificação SAML 2.0. No entanto, não temos integrações diretas com nenhum provedor no momento. Precisaremos coletar algumas informações do seu provedor de SSO para obter essa configuração.

>[!NOTE]
>
>Isso só se aplica a **Marketo Sales Connect** usuários. Se você não tiver o Sales Connect, mas quiser saber mais, entre em contato com a equipe de conta do Adobe (seu gerente de conta).

## Requisitos {#requirements}

* Conta SSO
* Assinatura de conexão do Marketo Sales
* Metadata.xml da conta SSO (URL de edição, endpoint para validação e uma chave pública)

## Configuração {#setup}

O metadata.xml da instância SSO da sua equipe deve conter o URL do emissor, o terminal para a validação e uma chave pública.

Também precisaremos que o Local SSO da conta SSO de sua empresa seja um domínio exclusivo. Por exemplo, precisamos de um subdomínio exclusivo como `toutapp.pingidentity.com` ou similar. Sem esse tipo de identificador exclusivo, não poderemos configurar o SAML no painel.

Um logon e Okta nem sempre fornecem identificadores exclusivos ao atribuir um URL. Se você estiver usando o Okta ou One Login, significa que não poderemos configurar um logon no botão do painel. Ainda seremos capazes de configurá-lo a partir do botão de Início de Sessão Único no [aplicação web](https://toutapp.com/login).

Assim que tivermos essas informações, trabalharemos com nossa equipe de engenharia para configurar isso para sua assinatura.
