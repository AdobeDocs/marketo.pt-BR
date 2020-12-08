---
unique-page-id: 2359798
description: Adicionar CNAMEs de Landing page adicionais - Documentos de marketing - Documentação do produto
title: Adicionar CNAMEs de Landing page adicionais
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Adicionar CNAMEs de Landing page adicionais {#add-additional-landing-page-cnames}

Você pode adicionar CNAMEs de landing page para permitir URLs diferentes para apontar para suas landings page de marketing. Siga as etapas abaixo para ajudá-lo a gerenciar vários domínios.

>[!CAUTION]
>
>Os cookies não podem ser compartilhados entre domínios.

>[!TIP]
>
>**Mesmo domínio de nível superior - Bom! Os cookies são shared.go**.mycompany.com > **info**.mycompany.**comDomínios de nível superior diferentes - Ruins! Os cookies não são compartilhados.**
>vá.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Encontre a sequência da sua conta {#find-your-account-string}

1. Vá para a área **Admin** e clique em **Landing page**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copie a string **da** conta na seção **Configurações** .

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anote-o para o próximo passo.

## Enviar solicitação para TI {#send-request-to-it}

1. Solicite ao departamento de TI que configure o seguinte CNAME: (Substitua a palavra [CNAME] pelo CNAME de sua escolha e pela STRING [de] CONTA pelo texto da etapa anterior).

   [CNAME].YourCompany.com > STRING [de]CONTA.mktoweb.com

## Adicionar um novo CNAME {#add-a-new-cname}

1. Depois que o departamento de TI tiver criado o CNAME, vá para **Admin** e clique em **Landing page**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Clique em **Novo** e selecione **Novo alias** de domínio.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Insira seu alias **de domínio.** A Página **** padrão será exibida se o visitante não colocar um URL. Digite para onde eles devem ir nesse caso.

   >[!NOTE]
   >
   >Para a Página padrão, você pode selecionar uma landing page ou um URL externo, como seu site público.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Digite sua Página **** padrão e clique em **Criar**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Legal! Agora você sabe o que fazer se quiser adicionar um CNAME.
