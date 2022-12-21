---
unique-page-id: 2360189
description: Personalize os URLs de sua página de aterrissagem com um CNAME (Administração) - Documentos do Marketo - Documentação do produto
title: Personalize os URLs de página de aterrissagem com um CNAME (Administração)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 3%

---

# Personalize os URLs de página de aterrissagem com um CNAME (Administração) {#customize-your-landing-page-urls-with-a-cname-administration}

Mesmo que o Marketo hospede suas landing pages, o URL deve ser personalizado para sua empresa.

>[!NOTE]
>
>Sem CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marca:
>
>https://go.**Sua empresa**.com/UnsuscribePage.html

>[!NOTE]
>
>**Permissões de administrador necessárias**

Vamos definir suas configurações!

1. Escolha um CNAME.

   É a parte frontal do URL. Exemplos:

   * **go**.YourCompany.com/NameOfPage.html
   * **informações**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, portanto anote isso.

1. Encontre sua sequência de caracteres da conta.

1. Vá para o **Administrador** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Em **Páginas de aterrissagem** , copie a Sequência de caracteres da conta na seção Configurações .

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Você também precisará disso mais tarde, portanto anote isso.

1. Enviar solicitação para TI.

1. Solicite que sua equipe de TI configure o seguinte CNAME (substitua a palavra [CNAME] e [STRING DE CONTA] com o texto da etapa anterior):

   [CNAME].YourCompany.com > [STRING DE CONTA].mktoweb.com

1. Conclua a configuração CNAME.

1. Depois que a TI criar o CNAME, acesse **Administrador** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Em **Configurações** seção , clique em **Editar**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Insira seu CNAME em **Nome do domínio para páginas de aterrissagem**, insira **Página de fallback**, insira **Página inicial** e clique em **Salvar**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

Sua página de fallback é onde as pessoas serão redirecionadas se a página de aterrissagem do Marketo não estiver disponível.

Excelente! Suas páginas de aterrissagem agora são marcadas com o domínio de sua empresa.
