---
unique-page-id: 2359746
description: Personalize seus URLs de Landing page com um CNAME - Documentos do Marketing - Documentação do produto
title: Personalize seus URLs de Landing page com um CNAME
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Personalize seus URLs de Landing page com um CNAME {#customize-your-landing-page-urls-with-a-cname}

Embora o Marketo hospede suas landings page, o URL pode ser totalmente personalizado. Como ele se parece sem um CNAME:

`http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

A aparência:

`http://go.YourCompany.com/UnsubscribePage.html`

## Escolha um CNAME {#choose-a-cname}

Escolha uma palavra para acessar o início do URL de suas landings page. É apenas uma palavra e deve ser relativamente curta. Exemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, então anote isso.

## Localize a sua cadeia de caracteres de conta {#find-your-account-string}

1. Vá para a área **Admin** e clique em **Landing page**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Permissões de administrador necessárias**

1. Na guia **Página inicial** **Páginas**, copie a **Conta** **Cadeia** da seção **Definições**.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Você precisará mais tarde, então anote isso.

## Enviar solicitação para TI {#send-request-to-it}

Solicite à equipe de TI que configure o seguinte CNAME: (Substitua as palavras [CNAME] e [STRING DE CONTAS] pelo texto da etapa anterior.)

[CNAME].YourCompany.com > STRING [ de ]CONTA.mktoweb.com

## Concluir Configuração CNAME {#complete-cname-setup}

1. Depois que a TI tiver criado o CNAME, vá para **Admin** e clique em **Landing page**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Na seção **Configurações**, clique em **Editar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Insira seu CNAME em **Nome do domínio para Landing page**, digite sua **página de fallback**, digite sua **Página inicial** e clique em **Salvar**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Sua página de fallback será a página para a qual os clientes potenciais serão redirecionados se sua Landing page de marketing não estiver disponível.

Bom trabalho! Suas landings page agora têm sua marca de domínio de empresa.
