---
unique-page-id: 2360189
description: Personalize os URLs de sua página de aterrissagem com um CNAME (Administração) - Documentos do Marketo - Documentação do produto
title: Personalize os URLs de página de aterrissagem com um CNAME (Administração)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 3%

---

# Personalize seus URLs de página de aterrissagem com um CNAME (Administração) {#customize-your-landing-page-urls-with-a-cname-administration}

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

   * **acesse**.YourCompany.com/NameOfPage.html
   * **informações**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, portanto anote isso.

1. Encontre sua sequência de caracteres da conta.

1. Vá para a área **Admin** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Na guia **Landing Pages** , copie a string da conta na seção Configurações .

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Você também precisará disso mais tarde, portanto anote isso.

1. Enviar solicitação para TI.

1. Peça à equipe de TI para configurar o seguinte CNAME (substitua a palavra [CNAME] e [CADEIA DE CARACTERES DE CONTA] pelo texto da etapa anterior):

   [CNAME].YourCompany.com > STRING  [DE CONTA].mktoweb.com

1. Conclua a configuração CNAME.

1. Depois que a TI criar o CNAME, vá para **Admin** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Na seção **Settings**, clique em **Edit**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Insira seu CNAME em **Domain name for Landing Pages**, digite a **Fallback page**, insira a **Homepage** e clique em **Salvar**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

Sua página de fallback é onde as pessoas serão redirecionadas se a página de aterrissagem do Marketo não estiver disponível.

Excelente! Suas páginas de aterrissagem agora são marcadas com o domínio de sua empresa.
