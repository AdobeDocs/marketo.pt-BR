---
unique-page-id: 2360356
description: Adicionar logon único a um portal - Documentos do Marketo - Documentação do produto
title: Adicionar logon único a um portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Adicionar logon único a um portal {#add-single-sign-on-to-a-portal}

Se você tiver um serviço de diretório que autentica usuários, é possível permitir o logon único (SSO) no Marketo. Oferecemos suporte a esse recurso usando a linguagem SAML (Security Assertion Markup Language) versão 2.0 e superior.

O Marketo funciona como um Provedor de serviços SAML (SP) e depende de um Provedor de identidade externo (IdP) para autenticar usuários.

Quando o SSO estiver ativado, o IdP poderá validar as credenciais de um usuário. Quando um usuário deseja usar o software Marketo, o IdP envia uma mensagem SAML assinada para a Marketo, atuando como o SP. Essa mensagem garante à Marketo que o usuário está autorizado a usar o software Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Você é um usuário do Microsoft Azure? Confira os [tutorial de integração](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target=&quot;_blank&quot;}.

## Como enviar a solicitação {#how-to-send-the-request}

* Envie a solicitação SSO, que é uma resposta SAML, para `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Como o URL de público-alvo da controladora de armazenamento. Usar `http://saml.marketo.com/sp`
* Se estiver usando o atributo SPNameQualifier , defina o elemento NameID para Subject como `http://saml.marketo.com/sp`
* Se estiver federando várias assinaturas do Marketo para o mesmo provedor de SSO, você poderá usar urls de SP exclusivas para cada sub do Marketo com o formato `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>O Marketo suporta apenas o inicializado pelo Provedor de identidade (também conhecido como iniciado pelo IdP), no qual o usuário inicia a página de logon do Idp pela primeira vez, é autenticado e navega até Meu Marketo.

## Observações adicionais {#additional-notes}

* **Tempo de sincronização** - Para um novo usuário, há um atraso de cerca de 10 minutos antes que uma solicitação SSO inicial seja processada.
* **Provisionamento de usuário** - Os usuários são provisionados manualmente pela Marketo.
* **Autorização** - As permissões do usuário são mantidas no Marketo.
* **Suporte a OAuth** - No momento, a Marketo não é compatível com OAuth.
* **Propagação automática de usuário** - Também conhecido como &quot;Just in Time Provisioning&quot; (Provisionamento em tempo justo), é quando o primeiro logon SAML de um usuário é capaz de criar o usuário em qualquer aplicativo da Web que ele esteja acessando (por exemplo, Marketo) e nenhuma ação de administrador manual é necessária. No momento, a Marketo não oferece suporte a isso.
* **Criptografia** - No momento, a Marketo não oferece suporte à criptografia.

>[!NOTE]
>
>Antes de começar, tenha seu Certificado de provedor de identidade no formato X.509 e na extensão .crt, .der ou .cer.

## Atualizar configurações do SAML {#update-saml-settings}

O SSO é desativado por padrão. Siga estas etapas para habilitar o SAML e configurá-lo.

1. Vá para o **Administrador** área.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Clique em **Logon único**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Se você não vir **Logon único** under **Administrador**, contato [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}.

1. Em **Configurações de SAML** seção , clique em **Editar**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Alterar **Logon único SAML** para **Ativado**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Insira seu **ID do emissor**, **ID da entidade**, selecione o **Localização da ID de usuário**, depois clique em **Procurar**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Selecione seu **Certificado do Provedor de Identidade** arquivo.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Clique em **Salvar**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Atualizar configurações da página de redirecionamento {#update-redirect-page-settings}

1. Em **Redirecionar páginas** seção , clique em **Editar**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Os clientes que usam a ID universal, juntamente com o SSO, devem inserir o URL de logon do Provedor de identidade na **URL de logon** campo.

1. Insira um **URL de logout**. Esse é o URL para o qual você deseja que o usuário seja direcionado ao sair do Marketo.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Insira um **URL de erro**. Esse é o URL ao qual você deseja que o usuário seja direcionado caso ocorra uma falha no logon no Marketo. Clique em **Salvar**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Ambas as páginas devem estar disponíveis publicamente.

>[!MORELIKETHIS]
>
>* [Uso de uma ID universal para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target=&quot;_blank&quot;}
>* [Restringir logon de usuário somente ao SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target=&quot;_blank&quot;}
>* [Convidar usuários do Marketo para duas instâncias com ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target=&quot;_blank&quot;}

