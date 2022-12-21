---
unique-page-id: 2359798
description: Adicionar outros CNAMEs de página de aterrissagem - Documentos do Marketo - Documentação do produto
title: Adicionar outros CNAMEs de página inicial
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Adicionar outros CNAMEs de página inicial {#add-additional-landing-page-cnames}

Você pode adicionar CNAMEs de página de aterrissagem para permitir URLs diferentes para apontar para suas páginas de aterrissagem do Marketo. As etapas abaixo ajudarão você a gerenciar vários domínios.

>[!CAUTION]
>
>Os cookies não podem ser compartilhados entre domínios.

>[!TIP]
>
>**Mesmo domínio de nível superior - Bom! Os cookies são compartilhados**.<br/> **go**.mycompany.com > **informações**.mycompany.com
>
>**Domínios de nível superior diferentes - Ruim! Os cookies são _not_ compartilhado**.<br/> vá.**mycompany**.com > ir.**mynewcompany**.com

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Encontre sua sequência de caracteres da conta {#find-your-account-string}

1. Vá para o **Administrador** e clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copie o **Sequência de caracteres da conta** do **Configurações** seção.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Anote-o para a próxima etapa.

## Enviar solicitação para TI {#send-request-to-it}

1. Peça ao departamento de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] com o CNAME de sua escolha e [STRING DE CONTA] com o texto da etapa anterior).

   [CNAME].YourCompany.com > [STRING DE CONTA].mktoweb.com

## Adicionar um novo CNAME {#add-a-new-cname}

1. Depois que o departamento de TI criar o CNAME, acesse **Administrador** em seguida, clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Clique em **Novo** em seguida, selecione **Novo Alias de Domínio**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Insira seu **Alias de Domínio.** O **Página Padrão** é exibido se o visitante não colocar um URL. Insira para onde eles devem ir nesse caso.

   >[!NOTE]
   >
   >Para a Página padrão, você pode selecionar uma página de aterrissagem ou um URL externo, como seu site público.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Insira seu **Página Padrão** e clique em **Criar**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Legal! Agora você sabe o que fazer se quiser adicionar um CNAME.
