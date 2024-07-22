---
unique-page-id: 2359798
description: Adicionar outros CNAMEs de página inicial - Documentação do Marketo - Documentação do produto
title: Adicionar outros CNAMEs de página inicial
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Adicionar outros CNAMEs de página inicial {#add-additional-landing-page-cnames}

Você pode adicionar CNAMEs de página de aterrissagem para permitir que URLs diferentes apontem para suas páginas de aterrissagem do Marketo. Seguir as etapas abaixo ajudará você a gerenciar vários domínios.

>[!CAUTION]
>
>Os cookies não podem ser compartilhados entre domínios.

>[!TIP]
>
>**Mesmo domínio de nível superior - Ótimo! Cookies são compartilhados**.<br/> **ir**.mycompany.com > **informações**.mycompany.com
>
>**Domínios de nível superior diferentes - Incorreto! Os cookies são _não_ compartilhados**.<br/> vá.**minhaempresa**.com > vá.**minhanovaempresa**.com

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área **Administrador**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Clique em **Minha conta**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Role para baixo até &quot;Informações de suporte&quot; e copie sua ID do Munchkin.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Enviar solicitação para TI {#send-request-to-it}

1. Peça ao seu departamento de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] pelo CNAME de sua escolha e [ID do Munchkin] pelo texto da etapa anterior).

   [CNAME].YourCompany.com > [ID do Munchkin].mktoweb.com

## Adicionar um novo CNAME {#add-a-new-cname}

1. Depois que o departamento de TI criar o CNAME, vá para a área **Administrador**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Clique em **Landing Pages**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Clique em **Novo** e selecione **Novo alias de domínio**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Insira seu Alias de Domínio **.** A **Página Padrão** será exibida se o visitante não colocar uma URL. Digite para onde eles devem ir nesse caso.

   >[!NOTE]
   >
   >Para a Página padrão, é possível selecionar uma página de aterrissagem ou um URL externo, como o site público.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Insira sua **Página padrão** e clique em **Criar**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Legal! Agora você sabe o que fazer se quiser adicionar um CNAME.
