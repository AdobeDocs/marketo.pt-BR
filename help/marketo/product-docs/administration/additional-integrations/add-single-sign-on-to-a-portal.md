---
unique-page-id: 2360356
description: Adicionar logon único a um portal - Documentos do Marketo - Documentação do produto
title: Adicionar logon único a um portal
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---


# Adicionar logon único a um portal {#add-single-sign-on-to-a-portal}

Se você tiver um serviço de diretório que autentica usuários, é possível permitir o logon único (SSO) no Marketo. Oferecemos suporte a esse recurso usando a linguagem SAML (Security Assertion Markup Language) versão 2.0 e superior.

O Marketo funciona como um Provedor de serviços SAML (SP) e depende de um Provedor de identidade externo (IdP) para autenticar usuários.

Quando o SSO estiver ativado, o IdP poderá validar as credenciais de um usuário. Quando um usuário deseja usar o software Marketo, o IdP envia uma mensagem SAML assinada para o Marketo, atuando como o SP. Essa mensagem garante ao Marketo que o usuário está autorizado a usar o software Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Você é um usuário do Microsoft Azure? Confira o [tutorial de integração](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Como enviar a solicitação {#how-to-send-the-request}

* Envie a solicitação SSO, que é uma resposta SAML, para `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como o URL de público-alvo da controladora. Use `https://saml.marketo.com/sp`
* Se estiver usando o atributo SPNameQualifier , defina o elemento NameID para Subject como `https://saml.marketo.com/sp`
* Se estiver federando várias assinaturas do Marketo para o mesmo provedor SSO, você pode usar URLs SP exclusivas para cada subconjunto do Marketo com o formato `https://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>O Marketo é compatível somente com o iniciado pelo Provedor de identidade (também conhecido como iniciado pelo IdP), no qual o usuário inicia a página de logon do Idp pela primeira vez, é autenticado e navega até Meu Marketo.

## Observações adicionais {#additional-notes}

* **Tempo de sincronização**  - Para um novo usuário, há um atraso de cerca de 10 minutos antes de uma solicitação SSO inicial ser processada.
* **Provisionamento de usuário**  - Os usuários são provisionados manualmente pelo Marketo.
* **Autorização**  - As permissões do usuário são mantidas no Marketo.
* **Suporte a OAuth**  - No momento, o Marketo não é compatível com OAuth.
* **Propagação automática de usuário**  - Também conhecida como &quot;Provisionamento just in time&quot;, esse é o momento em que o primeiro logon SAML de um usuário é capaz de criar o usuário em qualquer aplicativo Web que ele esteja acessando (por exemplo, Marketo) e nenhuma ação manual de administrador é necessária. No momento, o Marketo não oferece suporte a isso.
* **Criptografia**  - No momento, o Marketo não suporta criptografia.

>[!NOTE]
>
>Antes de começar, tenha seu Certificado de provedor de identidade no formato X.509 e na extensão .crt, .der ou .cer.

## Atualizar as configurações do SAML {#update-saml-settings}

O SSO é desativado por padrão. Siga estas etapas para habilitar o SAML e configurá-lo.

1. Vá para **Admin** e clique em **Logon único**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Se você não vir **Logon único** em **Admin**, entre em contato com [Suporte do Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Na seção **SAML Settings**, clique em **Edit**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Altere **Início de Sessão Único SAML** para **Ativado**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Insira seu **ID do Emissor**, **ID da Entidade**, selecione o **Local da ID do Usuário** e clique em **Procurar**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Selecione o arquivo **Identity Provider Certificate**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Clique em **Salvar**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Atualizar as configurações da página de redirecionamento {#update-redirect-page-settings}

1. Na seção **Redirecionar páginas**, clique em **Editar**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Os clientes que usam a ID universal, juntamente com o SSO, devem inserir o URL de logon do Provedor de identidade no campo **Login URL**.

1. Insira um **URL de logout**. Esse é o URL para o qual você deseja que o usuário seja direcionado quando ele sair do Marketo.

   ![](assets/eight.png)

1. Insira um **URL de erro**. Esse é o URL ao qual você deseja que o usuário seja direcionado caso ocorra uma falha no logon no Marketo. Clique em **Salvar**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Ambas as páginas devem estar disponíveis publicamente.

>[!MORELIKETHIS]
>
>* [Uso de uma ID universal para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Restringir logon de usuário somente ao SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Convidar usuários do Marketo para duas instâncias com ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

