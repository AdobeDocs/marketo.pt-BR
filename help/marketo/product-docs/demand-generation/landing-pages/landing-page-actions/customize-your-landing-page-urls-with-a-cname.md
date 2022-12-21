---
unique-page-id: 2359746
description: Personalize seus URLs de página de aterrissagem com um CNAME - Documentos do Marketo - Documentação do produto
title: Personalize seus URLs de página inicial com um CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# Personalize seus URLs de página inicial com um CNAME {#customize-your-landing-page-urls-with-a-cname}

Mesmo que o Marketo hospede suas páginas de aterrissagem, o URL pode ser totalmente personalizado. Como é sem um CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

A aparência:

`https://go.YourCompany.com/UnsubscribePage.html`

## Escolha um CNAME {#choose-a-cname}

Escolha uma palavra para ir no início do URL de suas landing pages. É apenas uma palavra e deve ser relativamente curta. Exemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, então anote isso.

## Encontre sua sequência de caracteres da conta {#find-your-account-string}

1. Vá para o **Administrador** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Permissões de administrador necessárias**

1. Em **Aterrissagem** **Páginas** , copie a **Conta** **String** do **Configurações** seção.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Você precisará mais tarde, portanto anote isso.

## Enviar solicitação para TI {#send-request-to-it}

Peça à equipe de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] e [STRING DE CONTA] com o texto da etapa anterior.)

[CNAME].YourCompany.com > [STRING DE CONTA].mktoweb.com

## Concluir configuração CNAME {#complete-cname-setup}

1. Depois que a TI criar o CNAME, acesse **Administrador** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Em **Configurações** , clique em **Editar**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Insira seu CNAME em **Nome do domínio para páginas de aterrissagem**, insira **Página de fallback**, insira **Página inicial** e clique em **Salvar**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Sua página de fallback será a página para a qual os leads serão redirecionados se sua Página de aterrissagem do Marketo não estiver disponível.

Excelente! Suas páginas de aterrissagem agora são marcadas com o domínio de sua empresa.
