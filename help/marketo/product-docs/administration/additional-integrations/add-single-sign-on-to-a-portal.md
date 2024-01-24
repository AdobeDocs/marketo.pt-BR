---
unique-page-id: 2360356
description: Adicionar logon único a um portal - Documentação do Marketo - Documentação do produto
title: Adicionar Logon Único a um Portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# Adicionar Logon Único a um Portal {#add-single-sign-on-to-a-portal}

Se você tiver um serviço de diretório que autentica usuários, poderá permitir logon único (SSO) na Marketo. Oferecemos suporte para esse recurso usando [!DNL Security Assertion Markup Language] (SAML) versão 2.0 e superior.

O Marketo funciona como um Provedor de serviço (SP) SAML e depende de um Provedor de identidade externo (IdP) para autenticar os usuários.

Quando o SSO está ativado, o IdP pode validar as credenciais de um usuário. Quando um usuário deseja usar o software Marketo, o IdP envia uma mensagem SAML assinada para a Marketo, atuando como o SP. Essa mensagem garante à Marketo que o usuário está autorizado a usar o software da Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>Isso não se aplica a assinaturas integradas à Identidade do Adobe. Para assinaturas integradas à Identidade do Adobe, o Logon único é configurado no nível da Organização Adobe no Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Você é um [!DNL Microsoft Azure] usuário? Confira o [tutorial de integração](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target="_blank"}.

## Como enviar a solicitação {#how-to-send-the-request}

* Enviar a solicitação de SSO, que é uma resposta SAML, para `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como o URL do público-alvo do SP. Uso `http://saml.marketo.com/sp`
* Se você estiver usando o atributo SPNameQualifier, defina o elemento NameID para Subject como `http://saml.marketo.com/sp`
* Se você estiver federando várias assinaturas do Marketo para o mesmo provedor SSO, poderá usar URLs exclusivos de SP para cada subconjunto do Marketo com o formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>O Marketo só é compatível com o provedor de identidade iniciado (também conhecido como iniciado por IdP), no qual o usuário inicia primeiro a página de logon do Idp, se autentica e depois navega até o My Marketo.

## Observações adicionais {#additional-notes}

* **Tempo de sincronização** - Para um novo usuário, há um atraso de aproximadamente 10 minutos antes do processamento de uma solicitação de SSO inicial.
* **Provisionamento de usuário** - Os usuários são provisionados manualmente pela Marketo.
* **Autorização** - As permissões do usuário são mantidas no Marketo.
* **Suporte para OAuth** - No momento, o Marketo não é compatível com o OAuth.
* **Propagação Automática de Usuários** - Também conhecido como &quot;Provisionamento Just in Time&quot;, isso ocorre quando o primeiro logon SAML de um usuário é capaz de criar o usuário em qualquer aplicativo web que ele esteja acessando (por exemplo, Marketo) e nenhuma ação de administrador manual é necessária. No momento, o Marketo não oferece suporte a isso.
* **Criptografia** - No momento, o Marketo não oferece suporte à criptografia.

>[!NOTE]
>
>Antes de começar, tenha seu Certificado de Provedor de Identidade no formato X.509 e na extensão .crt, .der ou .cer.

## Atualizar Configurações SAML {#update-saml-settings}

O SSO está desativado por padrão. Siga estas etapas para ativar o SAML e configurá-lo.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Clique em **[!UICONTROL Logon único]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Se você não vir **[!UICONTROL Logon único]** em **[!UICONTROL Admin]**, entre em contato [Suporte ao Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. No **[!UICONTROL Configurações de SAML]** clique em **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Alterar **[!UICONTROL Logon único SAML]** para **[!UICONTROL Ativado]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Insira seu **[!UICONTROL ID do Emissor]**, **[!UICONTROL ID da entidade]**, selecione o **[!UICONTROL Local da ID de usuário]** e, em seguida, clique em **[!UICONTROL Procurar]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Selecione o **[!UICONTROL Certificado do provedor de identidade]** arquivo.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Atualizar configurações da página de redirecionamento {#update-redirect-page-settings}

1. No **[!UICONTROL Redirecionar páginas]** clique em **[!UICONTROL Editar]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Os clientes que usam a Universal ID junto com o SSO devem inserir o URL de logon do Provedor de identidade na **[!UICONTROL URL de logon]** campo.

1. Insira um **[!UICONTROL URL de saída]**. Este é o URL ao qual você deseja que o usuário seja direcionado quando fizer logout do Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Insira um **[!UICONTROL URL do erro]**. Esse é o URL para o qual você deseja que o usuário seja direcionado em caso de falha ao fazer logon no Marketo. Clique em **[!UICONTROL Salvar]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Ambas as páginas devem estar disponíveis publicamente.

>[!MORELIKETHIS]
>
>* [Uso de uma Universal ID para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [Restringir o logon do usuário somente ao SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Convidar usuários do Marketo para duas instâncias com Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
