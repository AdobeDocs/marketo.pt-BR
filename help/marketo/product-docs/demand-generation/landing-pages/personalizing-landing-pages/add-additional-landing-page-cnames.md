---
unique-page-id: 2359798
description: Adicionar outros CNAMEs de página de aterrissagem - Documentos do Marketo - Documentação do produto
title: Adicionar outros CNAMEs de página inicial
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
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

1. Vá para o **Administrador** área.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Clique em **Minha conta**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Role para baixo até &quot;Informações de suporte&quot; e copie a ID do Munchkin.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Enviar solicitação para TI {#send-request-to-it}

1. Peça ao departamento de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] com o CNAME de sua escolha e [Munchkin ID] com o texto da etapa anterior).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Adicionar um novo CNAME {#add-a-new-cname}

1. Depois que o departamento de TI criar o CNAME, acesse **Administrador** área.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Clique em **Novo** em seguida, selecione **Novo Alias de Domínio**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Insira seu **Alias de Domínio.** O **Página Padrão** é exibido se o visitante não colocar um URL. Insira para onde eles devem ir nesse caso.

   >[!NOTE]
   >
   >Para a Página padrão, você pode selecionar uma página de aterrissagem ou um URL externo, como seu site público.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Insira seu **Página Padrão** e clique em **Criar**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Legal! Agora você sabe o que fazer se quiser adicionar um CNAME.
